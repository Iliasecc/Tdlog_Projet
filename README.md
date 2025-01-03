# Burnout Guard

## Guide d'Installation et d'Exécution

Pour exécuter et tester l'application en local, suivez les étapes ci-dessous :

### **Prérequis**
voir le fichier requirements.txt

### **Étapes**
1. **Cloner le projet**  
   Téléchargez ou clonez le projet dans un répertoire local :
   ```bash
   git clone <url_du_dépôt>
   cd Tdlog_Projet
   
 2.**pip install -r requirements.txt**

 3.**Ajouter dans le fichier app.py la clé openai fourni et puis exécutez le fichier app.py qui se trouve dans le folder tdlog_project**
 
 4.**Naviguer dans l'application en vous imaginant un Employé et puis un RH**
 ---------------
##**Plateforme de bien-être des employés** :

Bienvenue sur **Burnout Guard**, une plateforme réactive dédiée au bien-être des employés. Notre mission est d'aider les entreprises à prévenir le burnout et à améliorer la qualité de vie au travail. La plateforme utilise des données calculées chaque fin de mois pour déterminer le **burnout rate** des employés et propose des solutions personnalisées en fonction de ce taux. Et en plus elle propose des solutions préventives au burnout comme un psy virtuel et des activités pour le bien-être

## Fonctionnalités principales :

### 1. **Suivi du burnout rate :**
   - **Calcul du burnout rate** : Chaque employé saisit des informations sur son travail et son état mental. Ces données sont utilisées pour calculer un score mensuel de **burnout**.
   - **Solutions proposées** : En fonction du pourcentage de burnout, la plateforme recommande des actions comme des semaines réduites ou des congés, permettant de mieux gérer la charge de travail et prévenir le burnout.

### 2. **Eden - Psychologue virtuel :**
   - **Eden**, notre psy virtuel, est là pour écouter et répondre à toutes les préoccupations des employés. En cas de besoin, Eden peut organiser des séances avec des psychologues professionnels pour un accompagnement plus approfondi.

### 3. **Gamification et activités bien-être :**
   - **Activités individuelles** : Les employés peuvent participer à des activités bien-être proposées par l'entreprise. Lorsqu'ils les complètent, ils soumettent un justificatif à la RH. Si l'activité est validée, l'employé gagne des points.
   - **Activités collectives** : Les employés peuventproposer des activités collectives (comme un match de football, un dîner, etc.). S'ils participent à ces activités, ils gagnent également des poin ts.
   - **Proposition d'activités** : Chaque employé peut proposer des activités bien-être à l'ensemble de l'entreprise. Si l'activité est concrétisée, l'employé obtient encore plus de points.

### 4. **Tableau de bord pour les DRH :**
   - Les responsables des ressources humaines peuvent suivre les scores de burnout des employés, valider les activités soumises, et ajuster les horaires ou accorder des congés en fonction des recommandations basées sur les données.

## Fonctionnalités supplémentaires :

- **Saisie de données** : Les employés renseignent leurs informations professionnelles et personnelles via un formulaire simple.
- **Analyse des données** : Un algorithme analyse les données collectées pour évaluer le burnout rate de chaque employé et suggère des actions corre Un tableau de bord moderne permet aux responsables des ressources humaines de suivre et de gérer facilement le bien-être de leurs employésctives adaptées.
- **Interface intuitive** :.


## Structure du Projet

Le projet **TDLOG** est une application web qui utilise Flask pour le backend, un modèle de machine learning pour certaines fonctionnalités, et une interface utilisateur construite avec HTML, CSS, et JavaScript. Voici une description détaillée de l'organisation du projet :

### **Dossier Principal : `tdlog`**
Le dossier `tdlog` contient tous les fichiers nécessaires pour l'application, organisés comme suit :

- **`app.py`** : Le backend de l'application développé avec Flask. Il gère la logique des routes, les appels au modèle de machine learning, et les interactions avec les données.
- **Modèles Machine Learning** :
  - `model1.pkl` : Le modèle de machine learning entraîné.
  - `scaler.pkl` : Le scaler utilisé pour le prétraitement des données.
- **Dossier `templates/`** : Contient les pages HTML de l'application.
  - `employé.html` : Tableau de bord de l'employé.
  - `rh.html` : Tableau de bord des responsables RH.
  - `psyvirtuel.html` : Page de chat avec l'IA Eden, un psy virtuel pour les employés.
  - `activite.html` : Propositions d'activités et gamification pour le bien-être des employés.
  - `validation.html` : Page permettant aux RH de valider les justificatifs d'activités déposés par les employés.
  - `profile.html` : Profil utilisateur pour les employés.
  - `profiler.html` : Profil utilisateur pour les responsables RH.
- **Dossier `static/`** : Contient les ressources statiques utilisées par l'application.
  - `img/` : Toutes les images utilisées dans les pages web.
  - `css/` : Les fichiers CSS pour styliser les pages.
  - `js/` : Les fichiers JavaScript pour ajouter des fonctionnalités.
  - `lib/` : Bibliothèques graphiques utilisées pour les visualisations.
  - `scss/` : Fichiers Bootstrap pour la mise en forme des pages.

### **Fichiers à la Racine du Projet**
En dehors du dossier `tdlog`, les fichiers suivants sont présents :
- **`tdlog.ipynb`** : Un notebook Jupyter contenant le modèle machine learning entraîné et les analyses associées.
- **`employees.json`** : Base de données contenant les informations des employés après qu'ils ont rempli leurs tableaux de bord.
- **`grouped_employee.json`** : Fichier regroupant les employés en fonction des semaines réduites.

---

## Contribution :

Les contributions sont les bienvenues ! Si vous souhaitez améliorer le projet, proposer de nouvelles fonctionnalités, corriger des bugs ou améliorer la documentation, n'hésitez pas à soumettre une **pull request**.

