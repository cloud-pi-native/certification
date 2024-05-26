# Certification Cloud Pi Native (travail préliminaire)

Inventaire des compétences nécessaires en vue d'obtenir la certification Cloud Pi Native et modalité de validation des compétences.
Nous sommes à votre écoute pour toute suggestion, critique et apport de contenu. ( via pull request ou directement )
Cette certification met en oeuvre un principe d'amélioration continue, le contenu évoluera dans le temps.

Le matériel pédagogique proposé en open-source permet simultanément de former les experts et également ainsi que leurs fournir des outils permettant d'aider à définir le plan d'accompagnement et de formation des équipes *enabling*, pouvant parfois être appelées DevOps ou SRE. 
(cf. Team topologies)

Le contenu est présenté ci-dessous, sous la forme des compétences minimales à acquérir, il peut donner lieu à de la formation théorique, en continue, sans nécessiter de passer la certification.

Les formateurs en charge de dispenser des formations préalable sont invités pour développer l'autonomie des stagiaires, à mettre en place une démarche de learning inversé, le formateur partageant les grands objectifs à atteidnre, le pourquoi et selon l'intérêt du groupe, il propose quelques thèmes à approfondir en laissant au stagiaire un temps de recherche et il organise ensuite des sessions de partage et apporte la précision utile. Il peut selon le temps disponible organiser des exercices de mise en pratique.

Le passage de la certification s'adresse principalement à des coachs / accompagnants d'équipes de développement ayant déjà une pratique professionnelle soit en tant de dévelopeur ayant mis en oeuvre des déploiement ou personnels en charge d'infrastructure évoluant vers l'accompagnement des équiqes de développement.
Les candidats à la certification devront démontrer leur compétence par un examen théorique(qcm), une mise en pratique et un entretien oral.

Compétences initiales recommandées pour la certification :
- Il recommandé de maitriser suffisement kubernetes, le gitops, l'agilité, le CNCF, les architectures cloud native, 12 factors, la topologie des équipes, le kraftmanship et le lean-agile ;
 
Pour vous permettre de créer une culture générale nous vous recommandons :
- La lecture de la série de livres suivant est un plus :
  - Robert C Martin (Ucle bob) tel que Clean : software, architecture, agile, software kraftmanship ;
  - Team topologies ;
  - Ceux écrit par Gene Kim ;
- La maitrises suffisante des technologies tel que Helm, Vault, Argo, les opérators tel que cnpg, kafka, istio, SOPS, ODK / Openshift ;
- La maitrise suffisantes des offres des grands clouds providers ;
- De vous appuyer sur des parcours de formation existant : tels que Certified Kubernetes Application Developer (CKAD), Certified Kubernetes Administrator (CKA), SAFe ;
- une compétence en sécurité est un plus.

**Module « base et vision numérique de demain » :**
Objectif : mettre l'équipe en condition pour démarrer, développer, maintenir en conditions de sécurite et déployer une solution Cloud Native

- Accéder aux ressources documentaires existantes : githubs, charts helms, le CCT et la liste des exigences Cloud Pi Native
- Comprendre la vision associée à Cloud Pi Native, le raci d'ensemble ;
- Comprendre l'offre, l'organisation ministérielle et le processus d'approvisionnement des ressources d'infrastructure;
- Comprendre la spécificité de Kubernetes, l’architecture d’intégration, l’architecture facilitant l'agilité ;
- Comprendre le landscape cncf, choisir les produits, opérateurs ;
- Comprendre la topologie des équipes ;
- Comprendre l'isomorphisme des organisations et l'impact sur le logiciel : la loi de Conway ;
- Les profils des developpeurs; 
- Maitriser la conduite du changement, l'impact des neuroscience ;
- S'organiser pour réduire la charge cognitive des équipes et des développeurs,la répartition de la capacité d’une équipe build / run / refactorisation ;
- L'éthique et la responsabilité des developpeurs et des architectes, la vrai genèse du manifeste agile ;
- Comprendre les principes fondateurs d'un logiciel "cloud natif"  :
     - comprendre et maitriser les impacts de la "séparation of concern" et clean architecture (solid) ;
     - monolithe, monolithe distribué, micro service.chercher à mettre en place un découplage technique et organisationnel;
     - soutenir l'agilité, concevoir des architectures permettant le blue/green et la release on demand de feature ;
- Industrialiser et standardiser la production logicielle, simplifier, réduire le coût de possession, less is more, the thinest possible platform.
- Comprendre la maintenabilité d’un produit numérique, la nécessite de refactoring ;
- Déployer et maintenir à l'état de l'art : comprendre la configuration drift et les "12 factors" ;
- Good enough is good : l'amélioration continue, ne pas chercher à atteindre la lune tout de suite ;
- Le modèle de sécurité associé à l'offre cloud pi native, sast/dast, MCS et shift-left ;
- Comprendre la démarche d'homologation de sécurité au sein de l'état et bonne pratiques;
- se former, accès à des ressources en-ligne.

  Validation des acquis par : 
  - QCM
  - Travail pratique possible : élaborer une architecture logicielle cloud native compatible avec cloud pi native.

**Module « practitioner Cloud pi native» :**
Objectif : mettre l'équipe en condition pour démarrer, développer, maintenir en conditions de sécurite et déployer une solution Cloud Native

- (rappel): 
    - Comprendre l'offre, l'organisation ministérielle et le processus d'approvisionnement des ressources d'infrastructure;
    - Identifier les besoin de ressources nécessaires / quotas. Comprendre et utiliser les outils.
- Comprendre la console et l'utiliser  ;
- Mettre en oeuvre le pipeline d'ensemble, chaine primaire et secondaire ;
- Mettre en place un premier déploiement et le premier build / déploiement ;
- Construire un conteneur sécurisé (rootless, filesystem majoritairement readonly )
- Mettre en oeuvre une mecanisme blue/green d'argo cd de fonctionner et facile à superviser.
- Comprendre et Maitriser les ingress controlers, maitriser les certificats et la chaine de service.
- les spécificités du miom sur l'exposition réseau, les FIPs internet et RIE ,
- Le gitops, Helm et Argo CD ;
- L'observabilité et le dashboard "ma sécurité"; 
- la gestion des secrets SOPS ;
- Crash recovery, les sauvegardes restaurations ;
- Trucs et astuces, quels sont les pratiques gagnantes et les points spécifiques à connaitre au quotidien ;
- accélérer, accéder aux accélérateurs disponibles ;
- contribuer à l'offre, la communauté, la Roadmap ;
- se former, accès à des ressources en-ligne.

  Validation des acquis par :
      travaux pratiques : 
        faire une démonstration de la maîtrise d’un déploiement sur cloud pi et d'un debogage ( sur plateforme simulée )
        faire un PR, contribution.
      à l'oral : explication du chemin parcours

  - QCM
  - Capacité d'appel à la communauté d'échange de pratiques

**Module « la posture, coacher une équipe de développment pour les aider à mener avec succès leur projet » :**

Good enough is good ;
Mettre en place les fondamentaux et accompagner des équipes produits numériques au démarrage ;
Mettre en place des pratiques d'améliorations continue, le peer programming, la refactorisation et la gestion de la dette ;
Mettre en place une organisation en charge de faire du tutoriat, mettre en place les parcours de formation nécessaire ;
Maîtriser le repository github, comprendre les exigences du CCT cloud pi native ;
Accompagner à l'approvisionnement des ressources d'infrastructures ;
Maitriser l’organisationnel associé à un produit numérique, Conway, clean architecture, etc... ;
Maitrise la topologie des équipes (teams topologies) ;
Comprendre les interactions d'organisation et l'impact des couplages organisationnels et techniques et comment les éviter ;
Maitriser la soutenabilité de maintenance d’un produit numérique, les bonnes pratiques, l'usage éventuels des copilotes IA ;
Augmenter la qualité intraséques des logiciels,l'usager au centre, favoriser l'agilité et le release on demand ;
Comprendre les profils des developpeurs ;
Maitriser la conduite du changement, les neurosciences ;
Travailler en réseau de pratique, l'animation interne au sein de son organisation ;
Créer sa propre valise de formation.

Validation des acquis par : 
    échange oral ;
    monter un plan de formation d’une équipe à partir des ressources accessibles.

**Module animation de communautés internes:**

- Capacité à mobiliser les énergies au sein de sa communauté ;
- Les challenges de faire vivre une communauté ;
- Animer un débat autour des tendances ;
- Contribuer à la réflexion de l'offre.

  Validation des acquis par :
  - QCM
  - Evaluation pratique : présentation d'un petit mémoire démontrant la compréhension des les enjeux, quelles sont les tendances IT, les grands sujet de fond pour permettre de produire un produit numérique de qualité, soutenable et qui répond aux besoins.
