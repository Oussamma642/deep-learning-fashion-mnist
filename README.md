# 👕 Classification d'Images : Fashion MNIST avec TensorFlow/Keras

Ce petit projet implémente un réseau de neurones artificiels (Fully Connected Neural Network) pour classifier des images de vêtements issues du célèbre dataset **Fashion MNIST**. 

Il a été développé dans le cadre d'un travaux pratiques en Deep Learning afin de comprendre les mécanismes fondamentaux de la classification d'images, de la préparation des données à l'évaluation du modèle.

## 🎯 Objectifs du Projet
* Préparation et normalisation de données de pixels (Images 2D vers Vecteurs 1D).
* Utilisation de l'encodage One-Hot pour la classification multiclasse.
* Construction d'une architecture de réseau de neurones séquentielle.
* Entraînement avec l'optimiseur Adam et évaluation des performances.
* Visualisation des prédictions avec Matplotlib.

## 🛠️ Technologies Utilisées
* **Python 3**
* **TensorFlow / Keras** (Construction et entraînement du modèle)
* **NumPy** (Manipulation des matrices et tenseurs)
* **Matplotlib** (Visualisation des données et des résultats)

## 🧠 Architecture du Modèle
Le modèle est un réseau de neurones dense (FCNN) construit avec l'API `keras.Sequential`.

1. **Couche d'entrée (Input/Flatten) :** Aplatissement des images $28 \times 28$ en un vecteur de 784 éléments.
2. **Couche cachée (Dense) :** 128 neurones utilisant la fonction d'activation `ReLU` pour capturer les caractéristiques non linéaires.
3. **Couche de sortie (Dense) :** 10 neurones (correspondant aux 10 classes de vêtements) utilisant la fonction d'activation `Softmax` pour générer des probabilités.

* **Fonction de perte :** `categorical_crossentropy`
* **Optimiseur :** `adam`

## 📊 Résultats
Après un entraînement sur 5 epochs avec les 60 000 images d'entraînement, le modèle a été évalué sur 10 000 images de test inédites.

* **Précision (Accuracy) sur le jeu de test :** ~ [Insère ton score ici, ex: 87.5%]
* **Perte (Loss) sur le jeu de test :** ~ [Insère ton score ici, ex: 0.35]

## 👁️ Visualisation des Prédictions
Voici un aperçu des prédictions du modèle comparées aux véritables étiquettes sur un échantillon du jeu de test :

> 🖼️ *(Ajoute ici l'image de ta grille Matplotlib générée à la fin du code ! Tu peux l'enregistrer et la glisser dans ton dépôt GitHub)*

## 🚀 Comment lancer le projet
1. Cloner ce dépôt : `git clone https://github.com/ton-pseudo/nom-du-repo.git`
2. Installer les dépendances : `pip install tensorflow numpy matplotlib`
3. Exécuter le notebook ou le script Python.
