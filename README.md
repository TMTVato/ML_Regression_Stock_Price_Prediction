# Prédiction du Prix des Actions avec LSTM (PyTorch)
<img width="684" height="564" alt="Capture d&#39;écran 2026-02-21 192715" src="https://github.com/user-attachments/assets/3b216ab9-31c1-4bb4-b472-98bde4de2366" />

## Description du Projet

Ce projet implémente un modèle de régression en Machine Learning pour la prédiction du prix des actions basé sur l'architecture Long Short-Term Memory (LSTM), un type de réseau de neurones récurrents (RNN) particulièrement efficace pour les données séquentielles comme les séries temporelles financières. Le modèle est développé en utilisant la bibliothèque PyTorch et est capable de prédire le prix de clôture futur d'une action à partir de ses prix passés.


## Technologies Utilisées

*   **Python**
*   **PyTorch** : Pour la construction et l'entraînement du modèle de réseau de neurones.
*   **NumPy** : Pour les opérations numériques.
*   **Pandas** : Pour la manipulation et l'analyse des données.
*   **Matplotlib** : Pour la visualisation des données.
*   **yfinance** : Pour le téléchargement des données boursières.
*   **scikit-learn** : Pour le prétraitement des données (StandardScaler).

## Configuration et Installation

1.  **Cloner le dépôt GitHub (si applicable) :**
    ```bash
    git clone https://github.com/votre_utilisateur/votre_projet.git
    cd votre_projet
    ```

2.  **Installer les dépendances :**
    ```bash
    !pip install pandas numpy matplotlib yfinance scikit-learn torch
    ```
    (Si vous utilisez Google Colab, la plupart sont déjà installées ou peuvent être installées avec cette commande directement dans une cellule de code.)

## Utilisation

1.  **Ouvrir le Notebook** : Ouvrez le fichier `.ipynb` dans un environnement compatible Jupyter (comme Google Colab, Jupyter Lab, ou Jupyter Notebook).
2.  **Exécuter les Cellules** : Exécutez les cellules du notebook séquentiellement. Le code va :
    *   Télécharger les données pour un ticker spécifié (par défaut `AAPL`).
    *   Prétraiter les données.
    *   Construire et entraîner le modèle LSTM.
    *   Évaluer le modèle et afficher les RMSE.
    *   Afficher les graphiques de prédiction.

## Personnalisation

*   **Changer le Ticker de l'Action** : Modifiez la variable `ticker` (par exemple, `'MSFT'`, `'GOOGL'`) dans la cellule appropriée pour analyser une autre action.
*   **Ajuster la Longueur de Séquence (`seq_length`)** : Vous pouvez modifier la variable `seq_length` pour changer le nombre de jours passés que le modèle utilise pour chaque prédiction.
*   **Paramètres du Modèle LSTM** : Ajustez `hidden_size`, `num_layers`, `num_epochs` ou le `lr` (learning rate) pour expérimenter avec différentes configurations de modèle et d'entraînement.
