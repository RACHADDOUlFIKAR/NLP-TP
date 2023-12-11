### 1 Objectif : Utiliser des expressions régulières pour extraire des informations spécifiques d'un texte.
Exemple : Création d'une regex pour extraire des dates d'un texte donné, permettant une analyse temporelle.
Tokenization :

### 3 Objectif : Diviser une séquence de texte en unités plus petites (tokens).
Exemple : Utilisation de NLTK pour tokeniser une phrase en mots individuels, y compris la gestion des hashtags avec TweetTokenizer.
POS-Tagging (Marquage des Parties du Discours) :

### 4 Objectif : Attribuer une catégorie grammaticale à chaque mot dans une phrase.
Exemple : Utilisation de NLTK pour attribuer des POS-tags à chaque mot, fournissant des informations sur la structure grammaticale.
Stemming et Lemmatisation :

### 5 Objectif : Réduire les mots à leur forme de base.
Exemple : Utilisation du stemmer Porter pour le stemming, et du lemmatiseur WordNet avec POS-tagging pour une lemmatisation améliorée.
Amélioration de la Lemmatisation avec POS-Tagging :

### 6 Objectif : Utiliser le POS-tagging pour améliorer la lemmatisation des verbes.
Exemple : Liaison du POS-tagging avec le lemmatiseur WordNet pour obtenir des lemmes plus précis, notamment pour les verbes.
Ces exemples couvrent des concepts fondamentaux du traitement du langage naturel (NLP), du prétraitement des données, de l'exploration de données, et de la modélisation prédictive dans le contexte financier. Ils illustrent également l'utilisation de bibliothèques populaires telles que NLTK, scikit-learn et Matplotlib pour des tâches spécifiques.
Stemming :

Le stemming est un processus de réduction de mots à leur racine ou base, généralement en supprimant les suffixes. L'objectif principal est de regrouper les mots apparentés pour les considérer comme une seule entité. Cela peut aider à réduire la dimensionnalité des données textuelles et à améliorer la précision dans certaines tâches de traitement du langage naturel. Cependant, le stemming peut produire des formes tronquées qui ne sont pas toujours des mots valides.

Exemple de Stemming :

"Running" → "run"
"Easily" → "easili"
"Jumps" → "jump"
Les algorithmes de stemming, tels que le stemmer de Porter, appliquent des règles heuristiques pour réduire les mots à leur forme de base. Cependant, ils ne tiennent pas compte du contexte ou de la signification du mot.

Lemmatisation :

La lemmatisation est un processus plus sophistiqué qui vise à réduire les mots à leur forme canonique ou lemmatique, en utilisant la connaissance du sens du mot. Contrairement au stemming, la lemmatisation produit des lemmes qui sont des mots valides dans le langage naturel. Pour une lemmatisation précise, il est souvent nécessaire de spécifier la partie du discours (POS) du mot.

Exemple de Lemmatisation :

"Running" → "run"
"Easily" → "easy"
"Jumps" → "jump"
La lemmatisation peut prendre en compte la partie du discours d'un mot pour choisir la forme correcte. Par exemple, le verbe "running" peut être réduit à "run", et l'adjectif "better" peut être réduit à "good". La lemmatisation nécessite souvent des ressources linguistiques telles que des dictionnaires de lemmes.

POS-Tagging (Marquage des Parties du Discours) :

Le POS-tagging consiste à attribuer une catégorie grammaticale (partie du discours) à chaque mot dans une phrase. Les catégories grammaticales incluent des étiquettes telles que nom, verbe, adjectif, adverbe, préposition, etc. Le POS-tagging est souvent utilisé en conjonction avec la lemmatisation pour améliorer la précision, car il fournit des informations sur la fonction grammaticale d'un mot.

Exemple de POS-Tagging :

"The cat is running" → [("The", "DT"), ("cat", "NN"), ("is", "VB"), ("running", "VBG")]
Dans cet exemple, "DT" indique un déterminant, "NN" indique un nom, "VB" indique un verbe, et "VBG" indique un participe présent. Ces tags peuvent être utilisés pour améliorer la lemmatisation, car le lemmatiseur peut choisir la forme correcte en fonction du POS-tag du mot.






