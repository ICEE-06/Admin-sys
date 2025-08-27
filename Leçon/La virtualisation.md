## Définition
C'est une technologie qui permet de créer plusieurs environnements virtuels à partir d'**un seul matériel physique**. C'est à dire, elle permet de diviser un seule machine physique en plusieurs machines virtuelles appelées **VM**. 

Chaque machine virtuelle dispose de ses propres ressources virtuelles définit dans sa configuration : **mémoire vive, stockage, réseau, CPU, ....**. Les machines virtuelles sont isolées les unes des autres, mais elles peuvent communiquer entre elles via le **réseau**

La virtualisation s'appuie sur ce que l'on appel un **hyperviseur**. Nous pouvons dire que l'hyperviseur agit comme un chef d'orchestre, car il contrôle le matériel et assure la répartition des ressources entre les VM. Il existe des hyperviseurs de type **1** et **2**

La virtualisation est omniprésente dans les entreprises, et elle est devenue une technologie clé pour le **cloud computing**
Il est bien de noter qu'une autre technologie a émergée: les **conteneurs**. Il offre une alternative à la virtualisation, sauf que l'approche est différente car le **OS hôte** est partagé avec le conteneur, contrairement à une machine virtuelle.

## Avantages et inconvénients de la virtualisation 

### Avantages
- **Optimisation des ressources**
- **Réduction des coûts**(électricité, espace, matériels, ...)
- **Isolation**
- **flexibilité et évolutivité**

### Inconvénients
La virtualisation présente des nombreux avantages, mais elle comporte aussi des inconvénient important qu'il faut bien comprendre avant de se lancé.

Par exemple : Passé d'un ensemble des serveurs Physique a un architecture virtualisé est un projet complexe et coûteux au départ.

Voici quelques inconvénient majeurs à prendre à comptes :
- **Coût initial élevé** : il faut investir dans un serveur physique puissant, capable de supporter plusieurs machines virtuelles ainsi que dans des licences logiciels 
-  **Ressources partagées** : Même si plusieurs VMs peuvent tourner sur un même hôte, chaque VM a besoin de ses propre ressources, ce qui demande une configuration matérielle bien dimensionner.
- **Dépendance à un seul point de défaillance** : Si le serveur physique ou l'hyperviseur tombé en panne, toute les VMs hébergé peuvent être affectés.
-  **Complexité de gestions**: La virtualisation ajoute une couche d'abstraction supplémentaire qui peut rendre la gestion, le dépannage et la sécurité plus complexe

Exemple des virtualisations open-source :
- KVM (Kernel Virtual Machine)
- Xen
- Proxmox VE
- VirtualBox (Oracle )
- QEMU
Exemple des virtualisations proprétaire : 
- VMWare ESX
- Microsoft Hyper-V
- Oracle VM Server
- Nutanix
- Parallèls Desktop

#### Prérequis de la virtualisation

pour mettre en place une serveur de virtualisation, certaine prérequis matérielle et logicielles sont indispensable :
 - Un matérielle compatible : la machine physique doit avoir un processeur compatible avec la virtualisation, cela concerne la plupart des processeur Intel récent (VT-x et VT-d) et AMD (AMD-V et IOMMU). Ces options doit être activer dans le BIOS.
 - Ressources suffisantes : Il faut prévoir assez de RAM et de stockage pour le système hôte, l'Hyperviseur et toute les VMs
 - Logicielle d'hyperviseur : C'est le logicielle qui permet de créer et gérer des VMs
	Le choix dépendra de votre besoin et de votre techniques.

#### Hyperviseur type 1 et 2

Un hyperviseur de type 1 correspond a un système qui s'installe directement sur la couche matérielle du serveur. On parle d'une Hyperviseur **native** .Lorsqu'un Hyperviseur de type 1 est installé sur une machine, la machine ne peut pas servir à autre qu'a faire tourné l'hyperviseur, elle est dédié a cette usage.  

Un hyperviseur de type 2 est un logicielle qui s'installe et s'exécute sur une système d'exploitation qui est déjà en place.On parle un Hyperviseur **hébergé**.