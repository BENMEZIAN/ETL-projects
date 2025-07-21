# ETL-projects

## 📘 Projet 1 : COVID-19 Data ETL avec API

## 🎯 Objectif :
Ce projet consiste à extraire les données COVID-19 depuis une API, les transformer (sélection, nettoyage) et les stocker dans un fichier CSV localement. C'est un exemple basique d’un pipeline ETL (Extract, Transform, Load).

## 🛠️ Outils utilisés :
- Python
- API (disease.sh ou similaire)
- Requests
- Pandas
- CSV

## 🔄 Étapes du pipeline :

1. **Extraction :** appel de l’API pour récupérer les données mondiales COVID.
2. **Transformation :**
   - Sélection de champs utiles (cas, décès, récupérations, pays, date...).
   - Formatage ou renommage des colonnes.
3. **Chargement :** exportation des données finales dans un fichier `covid_data.csv`.

## 🗂️ Aperçu des données :
```
import pandas as pd
df = pd.read_csv("covid_data.csv")
df.head()

📦 Résultat final :
Un fichier covid_data.csv contenant les données COVID triées et prêtes à être analysées.

---

## 🛍️ Projet 2 : Scraping de livres e-commerce

```
# 📚 Projet Web Scraping – Données de livres depuis un site e-commerce

## 🎯 Objectif :
Extraire des données de livres depuis le site [books.toscrape.com](https://books.toscrape.com), les transformer et les enregistrer dans un fichier CSV. C'est un projet pratique pour démontrer la capacité à faire du scraping et de l'automatisation de collecte de données.

## 🛠️ Outils utilisés :
- Python
- Requests
- BeautifulSoup
- Pandas
- CSV

## 🔄 Étapes du pipeline :

1. **Extraction :**
   - Navigation sur plusieurs pages de la boutique.
   - Récupération des titres, prix, stock, note, lien image.
2. **Transformation :**
   - Nettoyage des prix.
   - Conversion de la note sous forme d’étoiles ou score.
   - Ajout d’un horodatage.
3. **Chargement :**
   - Enregistrement dans un fichier `books_data.csv`.

## 🗂️ Aperçu des données :
```
import pandas as pd
df = pd.read_csv("books_data.csv")
df.head()
📦 Résultat final :
Un fichier books_data.csv contenant les détails de plusieurs livres extraits automatiquement depuis le site e-commerce.
