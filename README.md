# Data Science


## Introduction
Dans le cadre de notre cours de data sciences, nous avons choisi d’étudier un DataSet répertoriant les crimes reportés par la police de Boston entre 2015 et 2018. Le but de ce cours est de trouver une problématique lié au DataSet choisi, de l'analyser et d'y apporter des conclusions au travers d'un dashboard visuel. 

### Sujet de l'étude 
A travers les différentes problématiques liés a la criminalité, nous avons choisi de chercher une solution pour améliorer la sécurité des citoyens. A partir de ce sujet, nous avons pu définir une problématique : **Comment pouvons nous prédir les crimes à venir? Quels outils pouvons nous utilisés afin de mieux répondre à notre question?** 

## Étude

Tout d'abord il a été crucial de comprendre les données présentent dans le DataSet. Ensuite, nous avons opter pour un logiciel de Data Visualisation adapté à notre volumétrie de données, sa gratuité mais aussi pour son partage de dashboard en ligne: Tableau. 
De plus, nous utilisons Python pour traiter les données en amont: effectuer les calculs ou requêtes dans notre DataSet.

Pour effectuer la prédiction des crimes à Boston à partir de notre DataSet, nous avons opter pour le modèle de régression **(PK? manque de détail)**. Pour cela, nous utilisons les données existante de temps pour pouvoir appréhender le futur.

### Analyse en fonction des heures

Dans un premier temps, nous nous sommes intéressé à la criminalité au travers des différentes heures de la journée. D'après notre graphique, le moment de la journée ou le moins de crimes a été répertorié est au alentours de 4h et 5h du matin, une tranche horaire paraissant plus ou moins logique du fait que les criminels restent des êtres humains et dorment la nuit. A l'inverse, la tranche horaire la plus affluente pour la criminalité est situé entre 16h et 18h.

![Crimes par heure](https://raw.githubusercontent.com/LucienDoustaly/Boston_Policing/master/Crimes_per_hour.PNG)

### Analyse en fonction des jours

Nous avons ensuite étudié l'activité criminelle en fonction des jours de la semaine. A travers le graphique ci-dessous, nous pouvons voir que le nombre de crimes est majoritaire durant la semaine, lorsque la majorité de la population est active, qui augmente logiquement la probabilité d'un crime. Cette hypothèse peut se confirmer avec les chiffres observés durant le weekend ou l'on peut voir une activité nettement réduite.

![Crimes par jour](https://raw.githubusercontent.com/LucienDoustaly/Boston_Policing/master/Crimes_per_day.PNG)

On se rends aussi compte que le nombre de crimes augmente en fonction de la période estival de l'année. Ce semble logique car les gens sortent plus a cette période de l'année.

![Crimes par mois](https://raw.githubusercontent.com/LucienDoustaly/Boston_Policing/master/Crimes_per_month.PNG)

### Prédiction des crimes

Nous avons ensuite crée un modèle de prédiction afin de pouvoir anticiper un type de crime, en fonction de plusieurs facteurs: 
* Moment qui défini le moment de la journée (matin, après-midi, soir) en fonction des heures  afin de simplifier le traitement. 
* La zone
* Le jour
* Le mois

![Modeler Flow](https://raw.githubusercontent.com/LucienDoustaly/Boston_Policing/master/ModelerFlow.png)

![Prédiction](https://raw.githubusercontent.com/LucienDoustaly/Boston_Policing/master/Prediction.png)

On peut voir que la précision de notre prédiction n'est pas acceptable (<2%), pour améliorer cette précision il faudrait créer un model avec plus de paramètres.  

Il faut cependant garder en tête que l'on essaie de prévoir un comportement humain. Certains chercheurs du MIT on reussi a créer une IA qui a une précision de 43% seulement lorsqu'il s'agit de prévoir le comportement humain sur des vidéos de youtube. Ce sont des chiffres positifs quand on sait que même l’être humain, pourtant généralement aguerri par l’expérience de vie, n’anticipe la bonne interaction que 71 % du temps sur ces vidéos.

Essayer de prédire des crimes semble plus compliqués car il faudrait aussi avoir des informations personelles sur la population, tel que le casier judiciaire, un bilan psychologique, les antécédents familiaux, etc...


[Source prédiction IA MIT](https://atelier.bnpparibas/smart-city/article/l-ai-affine-prediction-comportements-humains)

### Analyse en fonction de la position

D'après notre carte, on peut voir que la répartition du crime a travers Boston reste distribuée, une analyse supplémentaire répertoriant les differentes zone en fonction des crimes aurait pu être une piste d'amélioration afin de préciser cette étude. 

Sur notre dashboard sous Tableau, nous pouvons voir l'évolution des crimes dans le temps avec le type de crime, son compte et son emplacement. Le dashboard développé permet une meilleure lecture des données. Seul le curseur est déplaçable pour faire évoluer son état dans le temps.


## Conclusion

D'après les résultats obtenus, on observe que la criminalité est influé par la periode et le lieu, ou l'on peut remarquer que celles-ci correspondent à des tranches horaires et zone où la population dans les rues est élevé. Finalement, une solution pour augmenter sa propre sécurité serait d'éviter les heures affluentes.

## Technologies

* Tableau
* Jupyter Notebook

## Annexes

[Lien Tableau](https://public.tableau.com/profile/roulin#!/)

[Lien Jupyter notebook](https://github.com/LucienDoustaly/Boston_Policing/blob/master/Predictive-Policing.ipynb)


## Collaborateurs

* DOUSTALY Lucien</3
* JOLY Axel <<<<<<<33333333
* ROULIN Alexis <3 <3 <3
