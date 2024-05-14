### Description

2 millions de personnes éloignées de l'emploi en France, dont beaucoup accompagnées par le service public ou des structures d'insertion. Tous les acteurs de l'insertion partagent un objectif : l'inclusion des personnes qu'ils accompagnent dans des emplois dits durables. 

Les parcours ne sont pas linéaires et les personnes alternent périodes d'emploi oridinaire et chômage ou accompagnement RSA. Les sorties de parcours dites "positives" peuvent masquer des ruptures de contrats au bout de quelques mois, qui fragilisent des personnes qui cumulent déjà souvent les difficultés sociales et professionnelles. 

Notre hypothèse : en orientant les personnes en sortie de parcours vers des entreprises identifiées comme "engagées" ou "accueillantes", on sécurise leur insertion, c'est-à-dire qu'on augmente leurs chances d'être recrutées et de conserver leur emploi dans le temps. 

### Solution

Solution : donner accès aux chargés d'insertion professionnelle à une liste dynamque d'entreprises qui se distinguent par leur pratiques RH inclusives, par bassin d'emploi et secteur d'activité

Les données DSN permettent de calculer un score d'engagement. à partir de plusieurs paramètres : 

D'une part, les **profils des personnes recrutés** (on jauge la capacité d'un employeur à faire des « paris ») : répartition homme / femmes, embauches de personnes sans expérience préalables, de personnes avec des périodes de chômages ou d'arrêts longs, embauches de jeunes ou séniors, de bénéficiaires de l'obligation d'emploi travailleurs handicapé

~~D'autre part, la **nature des contrats proposés et les conditions de travail** : durée moyenne et médiane des CDD, type de contrats, etc.~~
+ Profils des personnes recrutées (capacité à faire des « paris ») : répartition homme / femmes, embauches de personnes débutantes sur le métier ou sans expérience préalable, de personnes avec des périodes de chômages ou d'arrêts longs, embauches de jeunes ou séniors, de bénéficiaires de l'obligation d'emploi travailleurs handicapé, de personnes issues de l'IAE ou ayant bénéficié de dispostifs d'aide à l'insertion professionnelle (contrats aidés)
+ Types de contrats proposés 
+ Durabilité et environnement de travail :  turn over, accidents de travail
+ 
~~Du point de vue de la méthode~~: 
~~on est repartis du produit minimum viable (une listing d'entreprises accessible à un accompagnateur~~)
- ~~on a identifié toutes les données qui pourraient servir de signaux d'engagement~~
- ~~xxxxxx~~
- 
- * *Quelle est la méthode de création de la solution ?*
* Données appelées : 
- lieu
- code NAF
- effectif
- nombre de personnes dans les 5 dernières années + nbre de contrats
- type de contrats,  / durée moyenne et médiane des CDD, tranches d'âge, embauches en contrats aidés, embauches de personnes sans expériences, ou profils TH
* Calcul d'un score  en prenant en compte différents critères
  --> critères positifs : pratiques de recrutement, types de contrat proposés, égalité homme/femme, accueil en stage
  --> critères négatifs : turn over, taux de risque AT/MP
  Calcul de la pondération à partir de l'établissement de médianes/ en prenant en compte la taille de l'établissement,  sa localisation, son secteur d'activité, les métiers pratiqués dans l'entreprise, les contrats proposés dans le secteur/métier

  Dans le type de contrats proposés, nous avons exclu les contrats à temps partiel car leur interprétation est complexe. Il est en effet impossible de distinguer le temps partiel voulu de celui imposé.

### Impact envisagé
*Que permet de faire la solution ?*
  Identifier les entreprises vertueuses
  Leur attribuer automatiquement un label avec une graduation

  *Qui sont les usagers visés, et qu’en feraient-ils ?*
 Les conseillers en insertion professionnelle et des opérateurs emploi (France Travail, Milo, ....  - les outiller pour leur permettre de repérer ces entreprises vertueuses et y orienter en priorité les personnes les plus fragiles qu'ils accompagnent
  Enrichir des moteurs de recherche d'emploi ou de stages/immersions.
  Pousser des conseils aux entreprises pour leur permettre de progresser
  
- Impact visé pour les personnes éloignées de l'emploi : accéder plus rapidement à un emploi et le conserver (hausse du taux de retour  à l'emploi et du maintien dans l'emploi à 6 et 12 mois)
- Impact visé pour les entreprises : accélérer l'adoption de pratiques de recrutement inclusives. Ce que l'on souhaite mesurer : est-ce que l'exposition à un score peut inciter les entreprises à modifier leur comportement de recrutement ? les entreprises qui n'ont pas le label engagée et à qui on a partagé leurs résultats ont-elles un socre qui s'améliore dans le temps ? Plus rapidement que les entreprises comparables qui n'ont pas été exposées à leur résultat. 

### Ressources

* *Lien vers la documentation du projet*

### [Facultatif] Retours sur la qualité des données exploitées

* *Quelles sont les difficultés que vous avez rencontrées dans l’usage des données ?*
