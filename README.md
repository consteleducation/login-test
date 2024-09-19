# **Test Technique**

## Mise en place de tests automatisés avec Cypress sur une page de connexion en JavaScript

### **Objectif du Test**

Évaluer votre capacité à :

- Comprendre et analyser une application web existante.
- Mettre en place un environnement de test avec Cypress.
- Écrire des tests automatisés efficaces pour une page de connexion.
- Suivre les bonnes pratiques en matière de tests automatisés.

### **Instructions pour le Candidat**

Vous devrez :

1. **Cloner le dépôt GitHub contenant l'application de connexion :**

   - Clonez le dépôt GitHub à l'adresse suivante : [**https://github.com/consteleducation/login-test.git**](https://github.com/consteleducation/login-test.git).

     ```bash
     git clone https://github.com/consteleducation/login-test.git
     ```

2. **Créer une nouvelle branche :**

   - Déplacez-vous dans le répertoire du projet :

     ```bash
     cd nom_du_repertoire
     ```

   - Créez une nouvelle branche pour votre travail :

     ```bash
     git checkout -b test-cypress-votre_nom
     ```

3. **Mettre en place l'application :**

   - Vérifiez que l'application fonctionne en ouvrant `index.html` dans un navigateur.

4. **Mettre en place l'environnement de test :**

   - Ouvrez un terminal à la racine du projet.
   - Initialisez un projet Node.js (si ce n'est pas déjà fait) :

     ```bash
     npm init -y
     ```

   - Installez Cypress en tant que dépendance de développement :

     ```bash
     npm install cypress --save-dev
     ```

5. **Écrire des tests avec Cypress pour les scénarios suivants :**

   - **Connexion réussie :**

     - Lorsque l'utilisateur entre un nom d'utilisateur et un mot de passe valides, un message de bienvenue s'affiche.

   - **Échec de connexion :**

     - Si l'utilisateur entre un nom d'utilisateur ou un mot de passe incorrect, un message d'erreur approprié s'affiche.

   - **Champs obligatoires :**

     - Vérifier que des messages d'erreur s'affichent si les champs "nom d'utilisateur" ou "mot de passe" sont laissés vides.

   - **Sécurité basique :**

     - S'assurer que le mot de passe n'est pas visible en clair lorsqu'il est saisi.

6. **Écrire les tests :**

   - Créez un dossier `cypress/integration` si ce n'est pas déjà fait.
   - Dans ce dossier, créez un fichier pour vos tests, par exemple `login.spec.js`.
   - Écrivez des tests couvrant les scénarios décrits ci-dessus.

7. **Exécuter les tests :**

   - Ajoutez un script dans votre `package.json` pour faciliter l'exécution des tests :

     ```json
     "scripts": {
       "test": "cypress open"
     }
     ```

   - Lancez les tests en exécutant :

     ```bash
     npm run test
     ```

8. **Documentation :**

   - Rédigez un fichier `README.md` ou une section dans ce fichier expliquant :

     - Comment installer et exécuter les tests.
     - Votre approche pour écrire les tests.
     - Tout problème rencontré et comment vous l'avez résolu.

9. **Pousser le code sur GitHub :**

   - Ajoutez les fichiers modifiés :

     ```bash
     git add .
     ```

   - Commitez vos changements :

     ```bash
     git commit -m "Ajout des tests Cypress"
     ```

   - Poussez votre branche sur le dépôt distant :

     ```bash
     git push origin test-cypress-votre_nom
     ```

   - Créez une **Pull Request** vers la branche principale du dépôt via l'interface GitHub.

### **Critères d'Évaluation**

- **Exactitude des Tests :**

  - Les tests couvrent-ils tous les scénarios demandés ?
  - Détectent-ils correctement les erreurs ?

- **Qualité du Code :**

  - Le code des tests est-il propre et bien structuré ?
  - Respecte-t-il les conventions de codage ?

- **Documentation :**

  - Les instructions sont-elles claires ?
  - Permettent-elles de reproduire les tests facilement ?

- **Bonnes Pratiques :**

  - Utilisation appropriée des sélecteurs.
  - Gestion correcte des promesses et des attentes asynchrones.

### **Durée du Test**

- Il est recommandé de réaliser ce test en 2 à 3 jours.

### **Livrables Attendus**

- Le code des tests Cypress poussé sur le dépôt GitHub dans une nouvelle branche.
- Une Pull Request vers la branche principale du dépôt.
- Une courte documentation ou un fichier `README.md` expliquant comment installer et exécuter les tests.
- Vos commentaires sur les améliorations possibles ou les défis rencontrés.

### **Optionnel**

- **Extension du Test :**

  - Vous pouvez ajouter des tests supplémentaires que vous jugez pertinents.
  - Implémenter des tests pour différents navigateurs ou tailles d'écran (responsive design).

---

**Nous vous souhaitons bon courage et sommes impatients de découvrir votre travail !**
