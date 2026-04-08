# 🚀 GUIDE DE DÉPLOIEMENT OVH

Voici la procédure pour déployer votre site sur OVH en toute sécurité.

## ÉTAPE 1 : Préparer les fichiers

1. Dans le dossier du projet, lancer la construction :
   
   npm run build
   
2. Cela crée le dossier **`dist`** (c'est votre site).

---

## ÉTAPE 2 : Connexion FileZilla

### 1. Ouvrir FileZilla
Lance le logiciel FileZilla sur votre ordinateur.

### 2. Remplir les champs en haut
En haut de la fenêtre, vous avez une barre "Connexion rapide". Remplis avec les infos de votre compte OVH:
- **Hôte** : `ftp.cluster015.hosting.ovh.net` (exemple, mettez le vrai !)
- **Identifiant** : `konli-admin` (exemple)
- **Mot de passe** : `******`
- **Port** : `21` (ou laisser vide)

Cliquez sur **"Connexion rapide"**.

### 3. Comprendre l'écran
- **Gauche** = VOTRE ordinateur (chercher votre dossier `dist` ici).
- **Droite** = LE SERVEUR OVH (c'est ici que vous envoyer les fichiers).

### 4. Se placer au bon endroit
- Dans la fenêtre de **droite** (Serveur), vous devez voir un dossier **`www`**.


## ÉTAPE 3 : Envoyer le site

1. Maintenant, double-cliquer sur le dossier **`www`** pour rentrer dedans.
2. Vider le contenu (supprimer tout sauf `.ovhconfig` s'il y est).
3. Ouvrer votre dossier **`dist`** sur votre ordinateur.
4. Sélectionner TOUT le contenu de `dist` (`index.html`, `assets`, `api`, etc.).
5. Glisser tout dans le dossier **`www`**.

---

## ÉTAPE 4 : Vérification

1. allez sur votre site.