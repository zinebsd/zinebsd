# Projet de Recherche de Texte et Chatbots

Ce projet propose une application permettant d'effectuer des recherches de texte et de calculer la similarité entre différents documents ou phrases à l'aide de techniques avancées de traitement du langage naturel. L'application inclut aussi deux chatbots, l'un basé sur **Word2Vec** et **TF-IDF**, l'autre sur un modèle de langage large via **API Call (GPT-4)**.

## Fonctionnalités

### 1. Recherche de Texte (Toutes Combinaisons Confondues)
   - **Rechercher un corpus dans d'autres corpus**, un fichier dans un corpus, ou des phrases spécifiques dans des documents.
   - Permet de **chercher et comparer** des textes selon des critères spécifiques définis par l'utilisateur (quels éléments chercher et où).
   - Possibilité de **téléverser des fichiers ou des corpus** personnalisés et d'afficher les documents les plus similaires à la recherche effectuée.

### 2. Calcul de Similarité avec Word2Vec et FastText
   - Utilisation des modèles **Word2Vec** et **FastText** pour la **vectorisation** des mots ou phrases.
   - Comparaison des vecteurs obtenus à l’aide de la **similarité cosinus** pour obtenir les textes les plus proches d'une requête.
   - Fonctionnement du calcul de similarité :  
     - **Prétraitement** (nettoyage du texte, découpage en mots/phrases).
     - **Vectorisation** via **Word2Vec** ou **FastText**.
     - **Calcul de la similarité** par la moyenne des vecteurs des mots et la mesure de la similarité cosinus.

### 3. Chatbot avec Word2Vec et TF-IDF
   - Un chatbot combinant **TF-IDF** et **Word2Vec (CBOW)** pour comprendre à la fois la fréquence des mots et leurs relations sémantiques.
   - Processus :  
     - Prétraitement du texte (stopwords, lemmatisation).
     - Attribution d'un poids à chaque mot via **TF-IDF** et entraînement d'un modèle **Word2Vec**.
     - Utilisation de la **similarité cosinus** pour identifier la réponse la plus proche.

### 4. Chatbot utilisant GPT-4 via API Call
   - Un chatbot basé sur le modèle **GPT-4** via l'API **ChatGPT**.
   - L'utilisateur soumet une question et le modèle génère une réponse en fonction d'un corpus ou d'un contexte spécifique.
   - Ce modèle peut traiter jusqu'à **32 000 tokens**, permettant de gérer des corpus volumineux et de fournir des réponses détaillées et contextuelles.

### 5. Nuage de Mots avec TF-IDF
   - Générateur de nuage de mots interactif, avec des options pour visualiser l'importance des mots selon leur **pondération TF-IDF**.
   - Possibilité de personnaliser l'affichage (couleurs, nombre de mots, etc.).

### 6. Ajout de GloVe et Doc2Vec
   - **GloVe** et **Doc2Vec** sont intégrés pour fournir des **représentations vectorielles des mots et des documents**.
   - Ces méthodes supplémentaires permettent de comparer et de calculer la similarité avec plus de flexibilité.

