# Scraping and NLP Pipeline

Brief description of the project.

## Table of Contents
1. [Objective](#objective)
2. [Overview of Work](#overview-of-work)
3. [Usage](#usage)
4. [Conclusion](#conclusion)

# Web Scraping and NLP Pipeline with MongoDB

## Objective
L'objectif de ce projet était de démontrer l'utilisation des techniques d'extraction de données web pour extraire des articles d'un site d'actualités, puis de traiter le texte à l'aide d'un pipeline de traitement du langage naturel (NLP). Les données extraites ont été stockées dans une base de données MongoDB pour une analyse ultérieure.

## Overview of Work
1. **Web Scraping**: Nous avons utilisé la bibliothèque `requests` pour envoyer des requêtes HTTP au site d'actualités et la bibliothèque `BeautifulSoup` pour analyser le contenu HTML et extraire les titres, liens et résumés des articles.

2. **NLP Pipeline**: Nous avons mis en place un pipeline NLP en utilisant les bibliothèques `nltk` et `spacy` pour tokenizer et lemmatizer le texte en arabe des articles. Nous avons également utilisé `ISRIStemmer` de `nltk` pour le stemming.

3. **MongoDB Integration**: Nous nous sommes connectés à une base de données MongoDB en utilisant la bibliothèque `pymongo` et avons inséré les articles extraits dans une collection.

4. **Normalization**: Nous avons appliqué le pipeline NLP pour normaliser le texte des articles, générant une liste de tokens lemmatisés, et avons mis à jour les documents MongoDB avec ces données normalisées.

## Usage
1. Installer les bibliothèques requises :
   ```bash
   pip install requests beautifulsoup4 pymongo nltk spacy

2. Vérifier la base de données MongoDB pour les articles extraits et leurs tokens normalisés.

## Conclusion
En conclusion, ce projet a démontré le processus d'extraction de données web pour extraire des articles d'un site d'actualités, suivi de la mise en œuvre d'un pipeline NLP pour traiter le texte. Le stockage des données extraites dans une base de données MongoDB permet un accès facile et une analyse du contenu des articles. Ce projet offre une base pour une exploration et une analyse ultérieures des données textuelles en utilisant des techniques d'extraction de données web et de NLP.
