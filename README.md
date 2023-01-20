# Application-Jeu-QUI-EST-CE ?
1) - Choix du langage : 
- Python comme choix de langage de programmation, car il est open source, polyvalent et de haut niveau avec une syntaxe facile à utiliser et une sémantique dynamique.

2) - Fonctionnalités de l’application : interactions possibles de l’utilisateur :
1. Le bouton START : c’est le bouton qui permet à l’utilisateur l’accés à l’application.
2. Le bouton ENTRER LE NOM DU PERSONNAGE : Ce bouton ouvre une nouvelle page permettant a
l’utilisateur de tenter de gagner en entrant le nom du personnage qu’il soupçonnne dans le "entry"(zone
texte) dédiée.
3. Le bouton VALIDER : Ce bouton dispose de deux fonctionnalités selon le mode de jeu (mode normal et mode triche). Avec le MODE NORMAL, le bouton "valider" ne fait que tester si la question posé est vraie (resp) (ou fausse (resp)), en répondant "True" (ou "False"), et ce via un Label. Avec le MODE TRICHE, le bouton valider renvoie également une réponse a la question tout en éliminant les personnages automatiquement (sans que l’utilisateur n’est a "barré" les images...). Par ailleurs, le processuspeut s’enchaîner jusqu’à ce qu’il reste au plus deux personnages.
4. Le bouton MODE TRICHE : On peut aussi l’appeler le mode facile, c’est une option d’aide pour l’utilisateur et comme son nom l’indique ce mode permet de calculer le nombre de personnages à éliminer avant de cliquez sur "valider". Par exemple, si le personnage recherché est "Lucas" qui est un homme
au cheveux roux, alors si on configure dans la combobox l’information "cheveux roux", et on clique sur avec le Mode triche, le nombre de personnages à éliminer apparaît sous forme d’un texte (via un label) tel que : "Élimination : 18 sur 24", et cochent automatiquement après validation tout les personnages n’ayant pas les cheveux roux.
5. Les boutons REJOUER et QUITTER LE JEU : Le bouton rejouer est relié à la fonction "rejouer" qui permet tout simplement de lancer une nouvelle partie sans devoir quitter complètement le jeu, en ce qui concerne le bouton quitter le jeu, c’est exactement l’inverse, ce bouton est relié à la fonction "quitter" qui permet de quitter le jeu, et ce, grâce à la méthode destroy() qui détruit le widget sur lequel cette méthode s’applique, dans notre cas, c’est la fenêtre principale de l’application ce qui provoque l’arrêt de toute l’application.

3) - Format du fichier JSON, contraintes éventuelles :
Description du format JSON : Le format de données JSON gère deux structures de données dans notre cas :
1. Une collection de paires nom / valeur et ce qu’on appelle objet, par exemple dans notre fichier personnage.json, on retrouve plusieurs paires telles que "images" :"personnages/","ligne" : "3", "colonne" : "8", "nbCara" : "4".
2. Une liste ordonnée des valeurs, c’est ce qu’on appelle un tableau, dans notre cas il y a deux tableaux :
"caracteristique" : [...] et "possibilites" : [...].

