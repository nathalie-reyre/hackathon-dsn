### Description

2 millions de personnes éloignées de l'emploi en France, dont beaucoup accompagnées par le service public ou des structures d'insertion. Tous les acteurs de l'insertion partagent un objectif : l'inclusion des personnes qu'ils accompagnent dans des emplois dits durables. 

Les parcours ne sont pas linéaires et les personnes alternent périodes d'emploi oridinaire et chômage ou accompagnement RSA. Les sorties de parcours dites "positives" peuvent masquer des ruptures de contrats au bout de quelques mois, qui fragilisent des personnes qui cumulent déjà souvent les difficultés sociales et professionnelles. Ainsi, sur 100 personnes enregistrées du RSA fin 2010, près de la moitié des personnes ont connu au moins une sortie et un retour au RSA dans la décennie suivante, et 10% ont connu 2 sorties et 2 retours. 

Notre hypothèse : en orientant les personnes en sortie de parcours vers des entreprises identifiées comme "engagées" ou "accueillantes", on sécurise leur insertion, c'est-à-dire qu'on augmente leurs chances d'être recrutées et de conserver leur emploi dans le temps. 

### Solution

Solution : donner accès aux chargés d'insertion professionnelle à une liste dynamique d'entreprises qui se distinguent par leur pratiques RH inclusives, par bassin d'emploi et secteur d'activité

Les données DSN permettent de calculer un score d'engagement. à partir de plusieurs paramètres : 
+ Profils des personnes recrutées (capacité à faire des « paris ») : répartition homme / femmes, embauches de personnes débutantes sur le métier ou sans expérience préalable, de personnes avec des périodes de chômages ou d'arrêts longs, embauches de jeunes ou séniors, de bénéficiaires de l'obligation d'emploi travailleurs handicapé, de personnes issues de l'IAE ou ayant bénéficié de dispostifs d'aide à l'insertion professionnelle (contrats aidés)
+ Types de contrats proposés 
+ Durabilité et environnement de travail :  turn over, accidents de travail

*Quelle est la méthode de création de la solution ?*

On a d'abord identifié les données utiles au calcul du score; Exemples de données appelées : lieu, code NAF, effectifs, type de contrats, etc. 

Ensuite, on calcule un score pour combiner les données selons deux logiques : 
  -> critères positifs : pratiques de recrutement, types de contrat proposés, égalité homme/femme, accueil en stage
  -> critères négatifs : turn over, taux de risque AT/MP

Enfin, on pondère les critères à partir de l'établissement de médianes, en prenant en compte la taille de l'établissement, sa localisation, son secteur d'activité, les métiers pratiqués dans l'entreprise, les contrats proposés dans le secteur/métier

NB : dans le type de contrats proposés, nous avons exclu les contrats à temps partiel car leur interprétation est complexe. Il est en effet impossible de distinguer le temps partiel voulu de celui imposé.  Nous avons intégré  les données liées à l'emploi des détenus mais sans pouvoir les exploiter en raison de leur fraicheur (données ajoutées à la DSN en 2024).
Nous n'avons pas intégré une analyse de la politique salariale pour des questions de temps même si nous pensons que l'ajout de ces données pourrait enrichir le scoring.

### Impact envisagé
*Que permet de faire la solution ?*

**Identifier les entreprises vertueuses et leur attribuer automatiquement un label avec une graduation**

*Qui sont les usagers visés, et qu’en feraient-ils ?*
Plusieurs cibles :
- Cible prioritaire : les conseillers en insertion professionnelle et les opérateurs emploi (France Travail, Milo, ....) pour leur permettre de repérer les entreprises engagées et y orienter en priorité les personnes les plus fragiles qu'ils accompagnent
  - Impact visé : accéder plus rapidement à un emploi et le conserver (hausse du taux de retour  à l'emploi et du maintien dans l'emploi à 6 et 12 mois)
- Cible secondaire : les entreprises pour leur permettre de progresser en matière de politique RH inclusive
  - Impact visé pour les entreprises : accélérer l'adoption de pratiques de recrutement inclusives. Ce que l'on souhaite mesurer : est-ce que l'exposition à un score peut inciter les entreprises à modifier leur comportement de recrutement ? les entreprises qui n'ont pas le label engagée et à qui on a partagé leurs résultats ont-elles un socre qui s'améliore dans le temps ? Plus rapidement que les entreprises comparables qui n'ont pas été exposées à leur résultat. 
  
### Ressources

- [Dico Metriques du Dataset_20240515081257.xlsx](https://github.com/adenoix/hackathon-dsn/blob/main/Dico%20Metriques%20du%20Dataset_20240515081257.xlsx) 
- [Flux de données](https://github.com/adenoix/hackathon-dsn/blob/main/Flux%20Data_20240515081247.pptx) 

### Retours sur la qualité des données exploitées

* *Quelles sont les difficultés que vous avez rencontrées dans l’usage des données ?*
- La table des liens est bizarrement configurée et oblige à mutiplier les jointures
- Des fins de contrat ne sont pas saisies par les employeurs. Cela peut générer des erreurs d'interprétation entre un contrat d'une durée très courte et un CDI.
- Il faut isoler les données liées à l'intermittence spectacle et à l'intérim afin de ne pas fausser le calcul du scoring

