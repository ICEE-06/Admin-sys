
## Installation MariaDB,  Apache, et PHP

```
sudo apt install apache2 mariadb-server libapache2-mod-php -y
sudo apt install php php-mysql php-gd php-xml php-mbstring php-curl php-zip php-intl php-bcmath unzip wget -y

```

## Création de la base de données NextCloud

```
CREATE DATABASE nextcloud;
CREATE USER 'nextclouduser'@'localhost' IDENTIFIED BY 'NextCloudPass@';
GRANT ALL PRIVILEGES ON nextcloud.* TO 'nextclouduser'@'localhost';
FLUSH PRIVILEGES;
EXIT;

```

## Télécharger NextCloud

```
cd /tmp
wget https://download.nextcloud.com/server/releases/nextcloud-29.0.5.zip
unzip nextcloud-29.0.5.zip
sudo mv nextcloud /var/www/html/
sudo chown -R www-data:www-data /var/www/html/nextcloud

```

## Configuration de Apache

- **Création fichier config**
```
sudo nano /etc/apache2/sites-available/nextcloud.conf
```

- **Ajouter**:
```
<VirtualHost *:80>
    ServerAdmin admin@exemple.com
    DocumentRoot /var/www/html/nextcloud
    ServerName cloud.exemple.com

    <Directory /var/www/html/nextcloud/>
        Options +FollowSymlinks
        AllowOverride All
        Require all granted
        <IfModule mod_dav.c>
            Dav off
        </IfModule>
    </Directory>

    ErrorLog ${APACHE_LOG_DIR}/nextcloud_error.log
    CustomLog ${APACHE_LOG_DIR}/nextcloud_access.log combined
</VirtualHost>

```

- **Activer le configs**:
```
sudo a2ensite nextcloud.conf
sudo a2enmod rewrite headers env dir mime
sudo systemctl reload apache2
```

## Accéder à NextCloud

Ouvrir un navigateur et y accéder via: `http://[IP_Serveur]/nextcloud`

Remplir les informations et taper `installer`

## Création Groupes et Utilisateurs


- **Création groupe**:
![[Groupe.png]]

- **Création Utilisateurs**
![[copmte10.png]]

![[compte11.png]]