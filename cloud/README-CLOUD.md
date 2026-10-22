<div align="center">

# Compte SyncSetup · SyncSetup account

**Serveur de synchronisation des profils · Profile sync server**

[Français](#-français) · [English](#-english)

</div>

---

## 🇫🇷 Français

### À quoi sert le compte SyncSetup ?

Il garde vos **profils** (vos listes de logiciels) identiques sur tous vos PC, en continu : un profil modifié sur un
PC l’est aussi sur les autres. Il est **facultatif** : SyncSetup fonctionne entièrement sans compte.

> Vous voulez seulement retrouver vos logiciels après une réinstallation de Windows ? La **sauvegarde GitHub**
> (page Compte › Sauvegarde GitHub) suffit et n’a besoin d’aucun serveur.

Le serveur ne connaît que votre adresse e-mail et vos profils. Il ne reçoit jamais la liste de vos logiciels
installés, votre matériel, le nom de votre PC ni vos fichiers. Le mot de passe n’est jamais stocké en clair (seule une empreinte PBKDF2 est gardée) ; tous les échanges
passent en HTTPS.

### « Serveur non configuré » : que faire ?

**Cas 1 — Serveur officiel.** Quand le serveur officiel de SyncSetup est disponible, il est déjà réglé dans
l’application : la page Compte affiche directement « Se connecter / Créer un compte ». Si vous voyez encore
« Serveur non configuré », mettez SyncSetup à jour (Paramètres › Mises à jour et versions).

**Cas 2 — Votre propre serveur (gratuit, environ 10 minutes).** Le serveur est un « Worker » Cloudflare : un petit
programme hébergé gratuitement par Cloudflare, avec sa base de données.

1. Créez un compte gratuit sur [dash.cloudflare.com](https://dash.cloudflare.com) et installez
   [Node.js](https://nodejs.org).
2. Téléchargez ce dossier `cloud` (bouton **Code › Download ZIP** du dépôt), décompressez-le, puis ouvrez un
   terminal dans le dossier `cloud` :

   ```bash
   npm install
   npx wrangler login
   npx wrangler d1 create syncsetup-db
   ```

3. Copiez le `database_id` affiché et collez-le dans `wrangler.toml`, à la ligne `database_id`.
4. Créez les tables, puis mettez le serveur en ligne :

   ```bash
   npm run db:remote
   npm run deploy
   ```

5. Copiez l’adresse affichée (`https://syncsetup-cloud.…workers.dev`), collez-la dans SyncSetup (Compte › Compte
   SyncSetup › adresse du serveur), cliquez sur **Enregistrer**, puis créez votre compte.

Utilisez la même adresse sur tous vos PC. Aucune clé ni mot de passe n’est à écrire dans les fichiers : `wrangler
login` s’occupe de l’accès à votre compte Cloudflare.

---

## 🇬🇧 English

### What is the SyncSetup account for?

It keeps your **profiles** (your software lists) identical on all your PCs, continuously: a profile changed on one
PC is changed on the others too. It is **optional**: SyncSetup works fully without an account.

> Only want your software back after reinstalling Windows? The **GitHub backup** (Account page › GitHub backup) is
> enough and needs no server.

The server only knows your email address and your profiles. It never receives the list of your installed
software, your hardware, your PC’s name or your files. The password is never stored in plain text (only a PBKDF2 hash is kept); everything goes over HTTPS.

### “Server not configured”: what should I do?

**Case 1 — Official server.** When the official SyncSetup server is available, it is already set in the app: the
Account page directly shows “Sign in / Create an account”. If you still see “Server not configured”, update
SyncSetup (Settings › Updates and versions).

**Case 2 — Your own server (free, about 10 minutes).** The server is a Cloudflare “Worker”: a small program
hosted for free by Cloudflare, with its database.

1. Create a free account on [dash.cloudflare.com](https://dash.cloudflare.com) and install
   [Node.js](https://nodejs.org).
2. Download this `cloud` folder (**Code › Download ZIP** button of the repository), unzip it, then open a terminal
   in the `cloud` folder:

   ```bash
   npm install
   npx wrangler login
   npx wrangler d1 create syncsetup-db
   ```

3. Copy the `database_id` shown and paste it into `wrangler.toml`, on the `database_id` line.
4. Create the tables, then put the server online:

   ```bash
   npm run db:remote
   npm run deploy
   ```

5. Copy the address shown (`https://syncsetup-cloud.…workers.dev`), paste it into SyncSetup (Account › SyncSetup
   account › server address), click **Save**, then create your account.

Use the same address on all your PCs. No key or password has to be written in the files: `wrangler login` handles
access to your Cloudflare account.
