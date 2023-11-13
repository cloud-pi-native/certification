# Questionnaire certification niveau 1

## Pré-requis 
 - Qu’est-ce que Kubernetes ?
   - Un Hyperviseur de machines virtuelles 
   - Un orchestrateur de Containers
   - Une distribution Linux orienté Containers
   - Un langage de programmation
 - Quelles différences entre OpenShift et K8S d’un point de vue utilisateur ? 

 - Qu’est-ce qu’un POD ? 

 - Comment créer un POD résilient ? 
   - XXX
   - XXX
   - XXX
 - Comment expose-t-on une application en utilisant K8S ? 
   - XXX
   - XXX
   - XXX
 - Comment est géré la persistance d’un POD ?
   - PVC
   - S3
   - NFS
 - Quels sont les opérations après la 1èresynchro repo via console DSO ? 
   - XXX
   - XXX
   - XXX
## Usages 
 - Que doit contenir un repo d’infra pour déployer mon appli sur K8S ? 
   - XXX
   - XXX
   - XXX
 - Quels sont les bonnes pratiques DSO ? 
   - XXX
   - XXX
   - XXX
 - Sur quel cluster trouver une application ?

 - Quelles organisations de repo correspond à un déploiement d’une application en développement spécifique sur DSO ? 
   - 1 Mono Repo (App + Infra)
   - 1 Repo App 
   - 1 Repo Infra (image construite en dehors de DSO)

 - Comment j’initialise une BDD ? 
   - Je crée un ticket 
   - Le déploiement se fait par un JOB / INITCONTAINER
   - L’application gère ses migrations
   - Je fais un port forwarding via Kubectl
   - Le projet expose un service d'accès (type PGADMIN)

 - Comment je mets à jour mon appli ? 
   - Mise à jour du tag de l'image dans le repo infra
   - J’envoie un ticket à la Service Team

 - Quel est le cheminement d’une appli sur DSO ? 
   - Chaîne primaire puis synchro chaine DSO, rebuild de l'image et déploiement
   - Build de l'image directement sur DSO puis déploiement
   - Build de l'image en dehors de DSO et déploiement par DSO sur ma registry privé en dehors de DSO

 - Quelles sont les stratégies de déploiement que l'on peut mettre en oeuvre ? 
   - Blue / Green
   - Orange / Red
   - Rolling Update
   - Canary
   - Pigeon

 - Quels types de IO sont disponibles pour les PVC sur DSO ? 
   - RWO
   - RWM
   - ROM

 - Quelles méthodes peut-on utiliser pour protéger les secrets applicatifs ? 
   - J'utilise le service SOPS
   - J'utilise le service Hashicorp VAULT 
   - J'utilise un KEYPASS partagé avec la ServiceTeam
   - J’envoie mes secrets via un ticket 
   - j'utilise des secrets K8S
   
## Techniques
 - Qu’est ce qui peut expliquer que mon déploiement est bloqué côté MI ? 
   - Absence du label 
   - Absence de requests / limits sur mon déploiement 
   - Absence de readiness / liveness sur mon déploiement 
   - Dépassement de quotas
   - Tag d’image à latest 
   - Remonté de règles KYVERNO non respectés 
   - CVE présentes et remontées par TRIVY sur Harbor

 - Comment je déclare mes ouvertures de flux, CDS, certificat, SSO ? 
   - Je crée un ticket à la Service Team
   - Je contacte le service infrastructure
   - Je le déclare dans la console DSO

 - Comment je garantie le déploiement avec un code de qualité ? 
   - Vérification des remontés SonarQube
   - Vérification des remontés TRIVY
   - Vérification des remontés KYVERNO
   - Je crée un ticket à la Service Team
   - Je demande à Chat GPT
   - Nos consoles corrigent automatiquement les défauts de code
