# Classification automatique des inscriptions grecques antiques par vision par ordinateur

## Objectif du projet

L’objectif principal de ce projet est de concevoir un modèle de classification automatique capable d’identifier différents types d’inscriptions grecques antiques à partir d’images. Ces inscriptions, issues de contextes variés (dédicatoires, honorifiques, impériales, poétiques, religieuses, etc.), remplissaient des fonctions multiples dans la société grecque antique : certaines étaient destinées à un usage politique (décrets), d’autres à des communications impériales (édits), à des pratiques religieuses (prières), ou encore à des finalités esthétiques et commémoratives (poèmes, épitaphes).

Contrairement aux approches traditionnelles basées sur la reconnaissance textuelle ou l’analyse paléographique des formes d’écriture, notre démarche fait le choix de ne pas exploiter le contenu linguistique. Nous nous concentrons exclusivement sur les caractéristiques visuelles globales des inscriptions (mise en page, formes, encadrements, éléments décoratifs) afin de déterminer leur type. Le défi central est que les images utilisées ne comportent aucune annotation textuelle : le modèle doit apprendre à différencier les types d’inscriptions uniquement à partir des traits visuels.

## Approches utilisées

- **Modèle YOLO** 
- **Modèle Vision Transformer (ViT)** : voici le lien du projet, exécuté dans google Collab [Accéder au projet](https://drive.google.com/drive/folders/18009w-2fo-mFo1M276ckUg0cfyGuziM2?usp=drive_link)
## Constitution de la base de données

Le corpus utilisé est la base *Inscriptions of Aphrodisias* ([https://insaph.kcl.ac.uk/insaph/](https://insaph.kcl.ac.uk/insaph/)). Il s’agit d’un recueil électronique d’inscriptions grecques gravées sur pierre provenant du site archéologique d’Aphrodisias (Asie Mineure), couvrant une période allant du IIe siècle av. J.-C. au VIIe siècle apr. J.-C.
 Les images ont été nettoyées, les doublons supprimés (basés sur le hash MD5 des fichiers).

 ### Répartition des tâches

| Étape                                  | Description                                          | Membres responsables                     |
|----------------------------------------|------------------------------------------------------|-------------------------------------------|
| Constitution de la base de données     | Sélection des images et classification manuelle     | Mathieu, Thomas                           |
| Pré-traitement des données             | Scraping, nettoyage et suppression des doublons     | Alexandre, Émilie                         |
| Tâches computationnelles (modélisation)| Entraînement et évaluation des modèles YOLO et ViT  | Alexandre, Émilie                         |



