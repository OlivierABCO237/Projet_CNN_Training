# Projet_CNN_Training
Classification of images of components by edge impulse

### Etape 1: **Récupération des données**
- Images d'un meme type de composants, pris de differentes manières pour former une base de données.
   Ici, nous avons pris 40 samples de chaque label, et 50 de l'arrière plan.
- Division du dataset en données d'entrainement et de test.

### Etape 2: **Création de l'impulse**
- Ajout d'un bloc "image" dans processing bloc et d'un bloc "Classification" dans learning bloc
- Modification des paramètres pour qu'elles correnpondent à la taille des images.
- Sauvegarde et génération des features
- Entrainement des données: Les résultats de l'entrainement sont très bons. 100% sur chaque label.
- Le test du modèle donne aussi des résultats satisfaisants: 93.33%

  ### Etape 3: **Mise en situation**
  - Nous avons collecté d'autres données de test, en prenant des photos via un téléphone portable et en les uploadant sur edge impulse.
  - Le test du modèle donne des résultats moins bon. 78% de précision.
  - Elle aurait sans doute été meilleure si une partie de ces données avait servie pour l'entrainement du modèle, car l'environnement n'est pas exactement le meme que celui des premières données
  - This model can be used and implement for recognising devices images in embedded applications
