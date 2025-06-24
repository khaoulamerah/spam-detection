#  Email Spam Detection 

##  Objectif du projet
Détecter automatiquement si un e-mail est un **spam** ou **non-spam (ham)** à l'aide d'un modèle d'intelligence artificielle.

---

##  Contenu du projet

- `spam.csv` : Fichier de données contenant des exemples d'e-mails.
- `spam_detection.ipynb` : Notebook Jupyter avec tout le code.
- `model.pkl` : Modèle entraîné pour la détection de spam.
- `README.md` : Description du projet.

---

##  Technologies utilisées

- Python 
- Scikit-learn
- Pandas
- Numpy
- TfidfVectorizer
- Jupyter Notebook

---

##  Étapes principales

1. **Chargement des données**
2. **Prétraitement des textes**
3. **Conversion en vecteurs numériques (TF-IDF)**
4. **Séparation Train/Test**
5. **Entraînement du modèle avec Logistic Regression**
6. **Évaluation du modèle**
7. **Prédiction sur de nouveaux e-mails**

---

##  Exemple de prédiction

```python
email = ["Congratulations! You've won a $1000 gift card."]
prediction = model.predict(vectorizer.transform(email))
print(prediction)  # Résultat : ['spam']
