# Lovano — Guide pour transformer le site en vraie application

Ce dossier contient le projet prêt à devenir une application Android et iOS,
à partir du site Lovano déjà en ligne.

## Étape 1 — Installer Node.js sur ton ordinateur (une seule fois)

1. Va sur https://nodejs.org
2. Télécharge la version "LTS" (recommandée) pour Windows
3. Installe-la comme n'importe quel programme (Suivant, Suivant, Terminer)
4. Vérifie que ça a marché : ouvre l'invite de commande (touche Windows, tape "cmd", Entrée)
   et tape : `node -v` → ça doit afficher un numéro de version (ex: v20.11.0)

## Étape 2 — Créer un compte GitHub (une seule fois)

1. Va sur https://github.com et crée un compte gratuit
2. Crée un nouveau "repository" (dépôt) — appelle-le par exemple `lovano-app`
3. Laisse-le "Public" ou "Private", peu importe pour l'instant

## Étape 3 — Envoyer ce dossier sur GitHub

Dans l'invite de commande, déplace-toi dans ce dossier (remplace le chemin par le tien) :

```
cd chemin\vers\lovano-app
git init
git add .
git commit -m "Premier envoi de Lovano app"
git branch -M main
git remote add origin https://github.com/TON-NOM-UTILISATEUR/lovano-app.git
git push -u origin main
```

(Remplace `TON-NOM-UTILISATEUR` par ton vrai nom d'utilisateur GitHub)

## Étape 4 — Créer un compte Codemagic

1. Va sur https://codemagic.io et crée un compte gratuit (connexion via GitHub, le plus simple)
2. Clique sur "Add application" et sélectionne ton dépôt `lovano-app`
3. Codemagic va détecter automatiquement le fichier `codemagic.yaml` déjà présent dans ce dossier
4. Lance le workflow "Lovano - Android" d'abord (plus simple, pas besoin de compte Apple pour tester)
5. Une fois que ça fonctionne, configure tes identifiants Apple Developer et Google Play
   dans Codemagic (menu "Distribution") pour publier automatiquement

## Étape 5 — Comptes développeur

- Google Play Developer : https://play.google.com/console (25$ une fois)
- Apple Developer : https://developer.apple.com/programs (99$/an)

## Besoin d'aide à une étape ?

Reviens dans la conversation avec Claude, décris où tu bloques (avec une capture
d'écran si possible), et demande de l'aide pour cette étape précise.
