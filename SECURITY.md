# Sécurité / Security

[Français](#français) · [English](#english)

## Français

### Signaler une faille

Merci de **ne pas** ouvrir d’« Issue » publique pour une faille de sécurité.

Utilisez le signalement privé de GitHub : onglet **Security** de ce dépôt › **Report a vulnerability**
(« Signaler une vulnérabilité »). Seul l’auteur de SyncSetup voit votre message.

### Quoi indiquer

- La version de SyncSetup (fenêtre **À propos**) et celle de Windows.
- Ce que la faille permet de faire, et dans quelles conditions (droits nécessaires, action de l’utilisateur…).
- Les étapes pour la reproduire, et si possible une preuve de concept minimale.
- Les fichiers ou journaux utiles (**Journal › Journal technique**), **sans** mot de passe, jeton ni donnée
  personnelle.

### Ce qui se passe ensuite

SyncSetup est maintenu par une seule personne, sur son temps libre. Au mieux :

- accusé de réception sous **7 jours** ;
- premier avis (faille confirmée ou non, gravité) sous **30 jours** ;
- correctif publié dans une nouvelle version dès que possible, selon la gravité.

Merci de **ne pas divulguer publiquement** la faille avant la publication du correctif. Si vous le souhaitez,
votre aide sera mentionnée dans les notes de la version corrigée.

### Versions prises en charge

Seule la **dernière version** publiée reçoit des correctifs de sécurité. SyncSetup se met à jour tout seul :
gardez les mises à jour automatiques activées (**Paramètres › Mises à jour et versions**).

### Vérifier un téléchargement

Chaque version publie ses empreintes SHA256 (fichier `SHA256SUMS.txt` et section « Vérification d’intégrité »
des notes). Voir le [README](FR%20-%20README.md#-vérifier-un-téléchargement).

## English

### Reporting a vulnerability

Please **do not** open a public issue for a security vulnerability.

Use GitHub’s private reporting: this repository’s **Security** tab › **Report a vulnerability**. Only the author
of SyncSetup can see your report.

### What to include

- Your SyncSetup version (**About** window) and Windows version.
- What the vulnerability allows, and under which conditions (required rights, user action…).
- Steps to reproduce it and, if possible, a minimal proof of concept.
- Useful files or logs (**Log › Technical log**), **without** passwords, tokens or personal data.

### What happens next

SyncSetup is maintained by one person in their spare time. At best:

- acknowledgement within **7 days**;
- first assessment (confirmed or not, severity) within **30 days**;
- a fix released in a new version as soon as possible, depending on severity.

Please **do not disclose** the vulnerability publicly before the fix is released. If you wish, your help will be
credited in the release notes of the fixed version.

### Supported versions

Only the **latest** released version receives security fixes. SyncSetup updates itself: keep automatic updates
turned on (**Settings › Updates and versions**).

### Verifying a download

Every release publishes its SHA256 hashes (`SHA256SUMS.txt` file and “Integrity check” section of the notes). See
the [README](README.md#-verifying-a-download).
