# First Demonstration

  * Date: 19.03.21
  * Examiners: Philippe Collet, Salah Damoul Guilhem Molines, Anne-Marie Pinna, Nikita Rousseau

## Planning

  * Constraints: 
    * 15 minutes for the team, 15 minutes from the jury;
    * No "all slides" presentation (slides are only accepted to show the architecture and the scenario paths)
    * Video demonstration by shared screen    
  * The evaluation will take into account the fact that teams presenting in the afternoon have more time to produce and prepare their demo.

| Timeslot      | Jury 1 + 2    |
|---------------|---------------|
| 08:00 - 08:30 | Team  K       | 

| Timeslot      | Jury 1  | 
|---------------|---------| 
| 08:45 - 09:15 | Team  A |
| 09:15 - 09:45 | Team  B |
| 09:45 - 10:15 | Team  C |
| 10:15 - 10:45 | Team  D | 
| 10:45 - 11:00 | Break   | 
| 11:00 - 11:30 | Team  J |
| 11:30 - 12:00 | Team  L |
| 12:00 - 12:30 | Team  M |
| 12:30 - 13:00 | Team  O |

| Timeslot      | Jury 2  | 
|---------------|---------| 
| 08:45 - 09:15 | Team  E |
| 09:15 - 09:45 | Team  F |
| 09:45 - 10:15 | Team  G |
| 10:15 - 10:45 | Team  H | 
| 10:45 - 11:00 | Break   | 
| 11:00 - 11:30 | Team  I |
| 11:30 - 12:00 | Team  N |
| 12:00 - 12:30 | Team  P |
| 12:30 - 13:00 | Team  Q |

## Expectations

You have to demonstrate a single product, covering both ISA & DevOps course contents. This single demo will be evaluated according to these two dimensions, leading to two different marks. *However*, the two courses expect the project to respect the _CastexSki_ call for bids and implement features related to this project.

### French version

* Partie ISA pour le MVP nous attendons que vous dérouliez un scénario sur la partie du coeur de l'application qui va d'un client vers un service externe minimum en passant par plusieurs composants EJBs (au moins 2) et si possible qui interagissent entre eux (l'interaction interne entre 2 EJBs sera valorisée). **Attention, si vous pouvez récupérer des composants de TCF (panier, gestion des clients) pour faciliter votre démarrage du développement, les 2 composants EJB de la phrase précédente correspondent à des composants nouveaux de votre architecture pour la gestion de la station de ski.** Pour la partie techno vous pouvez avoir un client minimaliste qui se contente de récupérer les parametres des services et de les appeler et pour le service externe mocker un Service .net en partant du code de TCF. Si l'imlémentation .net vous pose trop de difficultés; attaquez au minimum le même service externe que TCF.

* Pour le MVP partie DevOps, on aimerait voir que chaque composant est peut être construit en ne connaissant que des binaires de ceux dont il dépend, et sans les sources. Binaires récupérés depuis une repository Artifactory. On voudrait voir que si on composant ne compile/test plus, le build des autres composants en aval n’est pas affecté. On voudrait aussi que les interfaces entre les composants soient testées. Enfin on voudrait voir la structure choisie pour les sources et leurs dépendances, et que vous expliquiez vos choix. On souhaite aussi voir comment vous avez organisé le code en modules git. Pour cette première soutenance, il n’est pas imposé de démontrer des plans de build dans Jenkins, cependant on accordera volontiers un bonus aux groupes qui y seront parvenus.

Les éléments pour une bonne démo en ISA :
- montrer un schéma d'architecture de ce qui est prévu / fait actuellement
- donner les grandes justifications des responsabilités des composants implémentés, des choix effectués
- présenter à l'avance le ou les scénarios qui vont s'exécuter : une manière de faire cela, un peu coûteuse mais idéale, est de reprendre le schéma d'architecture et de surligner le chemin couvert par le scénario entre les composants (de la CLI au back end et systèmes externes)
- exécuter les scénarios depuis le front (CLI ou postman par exemple) en montrant en même temps des traces intéressantes dans le back-end (des passages dans les différents composants interconnectés par exemple), voire même jusqu'au système externe si c'est le cas. Pour démontrer cela, même si vous êtes à distance, l'écran partagé devrait donc être découpé en plusieurs fenêtres pour front, back et systèmes externes en même temps. C'est plus compliqué à distance, mais vous pourriez aussi garder à l'écran le schéma de l'architecture avec la trace du scénario à travers les composants pour que l'on puisse bien voir la communication entre composants graphiquement et dans les logs.

<p align="center">
  <img src="https://raw.githubusercontent.com/collet/isa-devops/master/demos/scenariodemo1.png"/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/collet/isa-devops/master/demos/scenariodemo2.png"/>
</p>

Les éléments pour une bonne démo en DevOps :
- montrer un schéma de dépendance des modules
- expliquer comment sont structurés vos POM
- démontrer que vous êtes capables de compiler un module B qui dépend d’un module A sans avoir le code source de A
- montrer que vous avez des tests, et qu’ils servent à quelquechose, par exemple en forçant l’échec d’un test pour montrer les conséquences.


