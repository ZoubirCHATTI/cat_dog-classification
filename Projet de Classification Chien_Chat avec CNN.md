# Projet de Classification Chien/Chat avec CNN

Ce projet implémente un réseau de neurones convolutif (CNN) pour classer des images de chiens et de chats. Il utilise la bibliothèque TensorFlow Keras pour la construction du modèle et la préparation des données.

## Structure du Projet

Le projet est principalement contenu dans un notebook Jupyter (ou un script Python dérivé) qui effectue les étapes suivantes :

1.  **Préparation des Données** : Utilisation de `ImageDataGenerator` pour le prétraitement et l'augmentation des images.
2.  **Chargement des Données** : Les images sont chargées à partir de répertoires spécifiés (entraînement, validation, test).
3.  **Construction du Modèle CNN** : Définition d'une architecture CNN séquentielle avec des couches convolutives, de pooling, de flattening et d'une couche dense de sortie.
4.  **Compilation du Modèle** : Configuration de l'optimiseur, de la fonction de perte et des métriques.
5.  **Entraînement du Modèle** : Entraînement du CNN sur les données d'entraînement et de validation.
6.  **Visualisation des Résultats** : Tracé de la précision d'entraînement et de validation au fil des époques.
7.  **Évaluation du Modèle** : Évaluation des performances du modèle sur l'ensemble de données de test.

## Exigences

Pour exécuter ce projet, vous aurez besoin des bibliothèques Python suivantes :

-   `tensorflow` (version 2.x recommandée)
-   `keras` (généralement inclus avec TensorFlow)
-   `matplotlib`
-   `numpy` (généralement inclus avec TensorFlow/Keras)

### Configuration de l'Environnement

Il est recommandé d'utiliser un environnement virtuel pour gérer les dépendances. Vous pouvez créer et activer un environnement virtuel comme suit :

```bash
python3 -m venv env
source env/bin/activate
```

Installez les dépendances requises :

```bash
pip install tensorflow matplotlib
```

### Structure des Données

Le projet suppose que vos données d'image sont organisées dans la structure de répertoires suivante :

```
/path/to/your/dataset/
├── train/
│   ├── dogs/
│   └── cats/
├── validation/
│   ├── dogs/
│   └── cats/
└── test/
    ├── dogs/
    └── cats/
```

Assurez-vous que les chemins `train_path`, `validation_path` et `test_path` dans le code (`dog_cat_CNN_commented.py` ou le notebook original) sont correctement définis pour pointer vers l'emplacement de votre jeu de données.

## Utilisation

1.  **Téléchargez le code** : Obtenez le fichier `dog_cat_CNN_commented.py` (ou le notebook original `dog_cat_CNN.ipynb`).
2.  **Préparez votre jeu de données** : Organisez vos images de chiens et de chats dans la structure de répertoires spécifiée ci-dessus.
3.  **Mettez à jour les chemins d'accès aux données** : Modifiez les variables `train_path`, `validation_path` et `test_path` dans le script pour qu'elles correspondent à l'emplacement de votre jeu de données.
4.  **Exécutez le script** :
    ```bash
    python dog_cat_CNN_commented.py
    ```
    Si vous utilisez le notebook Jupyter, ouvrez-le et exécutez les cellules séquentiellement.
##Exécution
pour exécuter le code, appuyer sur:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ZoubirCHATTI/cat_dog-classification/main?filepath=notebook/dog_cat_CNN.ipynb)

## Résultats

Le script affichera la précision d'entraînement et de validation à la fin de chaque époque. Un graphique montrant l'évolution de la précision sera également généré.

## Auteur

[Votre Nom/Organisation]


