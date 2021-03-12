# First Demonstration

  * Date: 19.03.21
  * Examiners: TBD

## Planning

  * Constraints: 
    * 15 minutes for the team, 15 minutes from the jury;
    * No slides;
    * Video demonstration by shared screen    
  * The evaluation will take into account the fact that teams presenting in the afternoon have more time to produce and prepare their demo.

| Timeslot      | Jury X |
|---------------|---------------|
| 08:00 - 08:30 | Team  ...     | 



## Expectations

You have to demonstrate a single product, covering both ISA & DevOps course contents. This single demo will be evaluated according to these two dimensions, leading to two different marks. *However*, the two courses expect the project to respect the _CastexSki_ call for bids and implement features related to this project.

### French version

* Partie ISA pour le MVP nous attendons que vous dérouliez un scénario sur la partie du coeur de l'application qui va d'un client vers un service externe minimum en passant par plusieurs composants EJBs (au moins 2) et si possible qui interagissent entre eux (l'interaction interne entre 2 EJBs sera valorisée). **Attention, si vous pouvez récupérer des composants de TCF (panier, gestion des clients) pour faciliter votre démarrage du développement, les 2 composants EJB de la phrase précédente correspondent à des composants nouveaux de votre architecture pour la gestion de la station de ski.** Pour la partie techno vous pouvez avoir un client minimaliste qui se contente de récupérer les parametres des services et de les appeler et pour le service externe mocker un Service .net en partant du code de TCF. Si l'imlémentation .net vous pose trop de difficultés; attaquez au minimum le même service externe que TCF.

* Pour le MVP partie DevOps, on aimerait voir que chaque composant est peut être construit en ne connaissant que des binaires de ceux dont il dépend, et sans les sources. Binaires récupérés depuis une repository Artifactory. On voudrait voir que si on composant ne compile/test plus, le build des autres composants en aval n’est pas affecté. On voudrait aussi que les interfaces entre les composants soient testées. Enfin on voudrait voir la structure choisie pour les sources et leurs dépendances, et que vous expliquiez vos choix. Pour cette première soutenance, il n’est pas imposé de démontrer des plans de build dans Jenkins, cependant on accordera volontiers un bonus aux groupes qui y seront parvenus.
