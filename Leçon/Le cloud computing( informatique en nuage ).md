## Définition

Il s'agit d'un modèle informatique qui permet d'accéder, à la demande, à des ressources informatiques (serveur, stockage, applications,...) via Internet. 
Le **cloud** permet d'utiliser des services info sans devoir avoir les matériels chez soit ou dans l'entreprise. 


> [!NOTE] CRM
> Customer Relationship Management: gestion des **relations clients**

Le **cloud computing** est une manière moderne de consommer de l'informatique, flexible, évolutive et économique basée sur l'**accès à distances** à des ressources via Internet

## Les principaux caractéristique du cloud computing

Le cloud computing présente plusieurs caractéristiques essentiels qui expliquent pourquoi il est largement utilisé aujourd'hui.
- **Accès et à la demande**:
	Avec le cloud les utilisateurs peuvent accéder aux services quand ils le souhaitent et où qu'ils soient, à condition d'avoir une **connexion Internet**

- **Évolutivité ou Élasticité**:
	Les services cloud sont très flexible, c-a-d que nous pouvons ajuster les ressources informatiques en fonction de nos besoins
	Ce principe s'appel aussi la **scalabilité**

- **Paiement à l'utilisation**:
	Avec le cloud, on paye uniquement ce qu'on consomme.
	Ce modèle est **économique**, surtout pour les petites entreprises ou les projets ponctuels. On dit aussi que le cloud est un **service mesurable** 

-  **Mutualisations des ressources** 
	Les fournisseurs de services cloud regroupent et partagent les ressources entre tout leur clients

- **Sécurité et disponibilité**
	Un service cloud fiable doit garantir un haut niveau de sécurité, pour se protéger des cyber-menaces.
	Les équipements sont héberger dans des centres de donné(data-center) conçu pour résister à des incidents comme des inondations, coupures d'électricité et incendie.


## Les types de cloud : Privé, Public, hybride
#### Cloud public
Le cloud pulic est le modèle le plus répondu.
Il repose sur une infrastructure mutualisé, accessible à tous via internet . Dans ce cas, les ressources sont héberger chez un fournisseur tièrs, dans un ou plusieurs data-center. L’infrastructure appartient entièrement au prestataire , qui assure la gestion et la maintenance et la sécurité.

#### Cloud privé
Le cloud privé désigne une infrastructure cloud exclusivement réservé à une seule organisation .
Les ressources sont dédiés et ne sont pas partagé avec d’autres clients garantissant ainsi une meilleur maîtrises de la sécurité , de la confidentialité et de la personnalisation

Ce type de cloud peut être déployer : 
• En interne , dans les logs de l’entreprise  
• Chez un prestataire externe, comme c’est le cas avec  OVH cloud qui propose un cloud privé héberger baser sur des technologie comme **vmwaren** , avec plusieurs hyperviseurs et une console d’administration **Vcenter**. Le cloud privé demande des investissement plus important en therme de matériel, d’hébergement , mais il offre en contre partie un contrôle total sur l’environnement IT avec une possibilité de personnalisation  selon le métier

##### Cloud hybride
Le cloud hybride combine les avantages du cloud public et du cloud privé. Il s’agit d’une architecture mixte dans laquelle l’entreprise utilise à la fois des ressources privé (dédié et sécuriser)et des ressources public, plus flexibles et évolutive


##  MultiCloud

Le **MultiCloud** consiste a utilisé plusieurs fournisseurs des services **Cloud** afin de répondre aux besoins spécifique d'une organisation. Il peut s'agir des plusieurs Cloud publique, privé, hybride. Cette stratégie permet de tirer parti des atout propre à chaque prestataires.

pour les entreprise, les **MultiCloud** présentes des avantages notable en matière de résilience et de capacité d'évolution. Cependant, il introduit également une certaines de complexité notamment dans la gestion des multiples environnement hétérogènes.

## Les modèles de services Cloud

Lorsque vous travailler sur un projet Cloud, Vous faire des rechercher sur une domaines, Vous rencontrez fréquemment les acronymes suivant: (**IaaS**, **PaaS** et **SaaS**)

Ce terme désigne des différences modèles de Cloud :

- **IaaS** (Infrastructure as a Services) : 
	il s'agit d'un modèle qui met à la disposition des utilisateurs des ressources fondamentales tels que des serveurs ou du stockages ou des réseaux. Dans ce modèles, l'utilisateurs disposent des contrôles totales sur infrastructures, ce qui inclut l'installation du système d'exploitation, la configuration du réseau, la gestion des applications et la maintenances globales.
	Parmit les principaux fournisseurs **IaaS**, on retrouve **AWS**(Amazon Web Service), **Microsoft AZUR**, **Google Cloud plateforme, Oracle Cloud et OVH Cloud**


- **PaaS** (Plateforme as a Service) : 
	Ce modèle fournie un environnement complet et prêt à l'emploi pour le développement, les testes et les déploiements d'application. Contrairement à IaaS, les utilisateurs n'ont pas a gérer les infrastructures qui est entièrement pris en charge par le fournisseurs Cloud
	Les **PaaS** permet au développeurs de se concentrer sur les codes et les fonctionnalités des leurs applications sans se soucié de la gestion serveur de la base des Données, du système d'exploitation ou de la mise à l'échelle.
	
	Exemple : **Red Hat OpenShift, Microsoft AZUR App Services et Heroku**

- **SaaS** (Software as a Services) :
	Ce modèle consiste a fournir une application prêt à l'emploi, accessible directement via internet. L'utilisateur n'a rien installer localement, ni à gérer l'infrastructure ou des mise à jours : toute est opéré par les fournisseurs des services
	L'accès se fait généralement via une navigateur Web ou une application dédié, depuis n'importe quel terminal. Les fournisseurs prend en charges l'hébergement, la maintenances, les mise à jours et la sécurité de l'ensemble de l'environnement. les modèles SaaS est aujourd'hui très répandu. Il couvre des nombreuse domaines : messagerie, Stockage en ligne, Collaboration, gestion des projet, CRM (Customer Relation Management), Vidéo Conférence...
	Exemple : Microsoft 365, Google WorkSpace, Dropbox, OneDrive, Zoom, Trello, Canvas, Wrike, DocuSign, Brevo, ServiceNow, CiscoWebex
