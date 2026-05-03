# 🏆 Gestionnaire de Concours Facebook

Un outil gratuit et simple pour gérer vos concours Facebook : vérification des critères, suivi des participants et tirage au sort animé.

**👉 [Accéder à l'application](https://SOSDeratiseur.github.io/concours/)**

---

## ✨ Fonctionnalités

- **Gestion des participants** — Ajoutez les participants un par un ou importez un fichier CSV
- **Vérification des critères** — Cochez pour chaque personne si elle a bien :
  - 👍 Aimé la page
  - 👥 Tagué 3 personnes en commentaire
  - 🔄 Partagé le post en public
- **Tirage au sort animé** — Avec effet roulette et confettis pour le gagnant
- **Tirages multiples** — Les gagnants précédents sont automatiquement exclus
- **Sauvegarde automatique** — Les données sont conservées dans votre navigateur (localStorage)
- **Import / Export CSV** — Gérez vos participants dans Excel ou Google Sheets
- **Mode API Facebook** — Importez automatiquement les commentaires via l'API Graph

---

## 🚀 Utilisation

1. Ouvrez l'application dans votre navigateur
2. Renseignez le **nom de votre page** au premier lancement
3. Ajoutez les participants et cochez leurs critères
4. Lancez le tirage au sort !

> Aucune installation, aucun compte, aucun serveur requis. Tout fonctionne dans le navigateur.

---

## 🤖 Mode Automatique (API Facebook)

Pour importer automatiquement les commentaires de votre post :

1. Créez une application sur [developers.facebook.com](https://developers.facebook.com)
2. Allez dans **Outils → Explorateur d'API Graph**
3. Générez un token avec les permissions :
   - `pages_read_engagement`
   - `pages_read_user_content`
4. Collez le token dans l'application au démarrage

> **Note :** En raison des restrictions de l'API Facebook (depuis 2018), les *likes de page* et les *partages publics* ne peuvent pas être vérifiés automatiquement. Ces deux critères restent à cocher manuellement.

---

## 📁 Format du fichier CSV

Pour importer des participants via CSV, utilisez ce format :

```
Nom,A aimé la page,A tagué 3 personnes,A partagé publiquement
Marie Dupont,Oui,Oui,Oui
Jean Martin,Non,Oui,Non
Sophie Bernard,Oui,Oui,Oui
```

Les valeurs acceptées : `Oui` / `Non` — ou `1` / `0`

---

## 🛠 Héberger votre propre version

1. Forkez ce repository
2. Allez dans **Settings → Pages**
3. Sélectionnez la branche `main` comme source
4. Votre version sera disponible sur `https://VOTRE-NOM.github.io/concours/`

---

## 📄 Licence

Projet open source — libre d'utilisation et de modification.
