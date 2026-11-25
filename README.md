# Alunissage

Jeu d'alunissage pour Android : module lunaire, trois commandes (gauche, poussée, droite), relief régénéré à chaque partie, physique lunaire réaliste, niveaux, astres, sons, vibration et score.

## Obtenir l'APK

1. Créer un dépôt GitHub vide (par exemple `alunissage`) et y envoyer le contenu de ce dossier, branche `main`.
2. L'envoi déclenche automatiquement la compilation (onglet "Actions", environ 3 à 5 minutes).
3. L'APK apparaît ensuite dans l'onglet "Releases" du dépôt, sous le nom `Alunissage.apk`.
4. Sur le téléphone : ouvrir ce lien, télécharger l'APK, autoriser l'installation depuis cette source si Android le demande.

Chaque nouvel envoi sur `main` produit une nouvelle version, installable par-dessus la précédente (la clé de signature est fixe et fournie dans `app/debug.keystore`).

## Structure

- `app/src/main/assets/index.html` : le jeu (HTML, CSS, JavaScript), polices incluses, fonctionne hors ligne.
- `app/src/main/java/.../MainActivity.java` : conteneur plein écran, écran maintenu allumé, pause automatique quand l'appli passe en arrière-plan, pont de vibration natif.
- `.github/workflows/build.yml` : compilation et publication automatiques.

## Note sur la signature

La clé fournie convient à un usage personnel et à une diffusion directe. Pour une publication sur le Play Store, il faudra générer une clé privée dédiée et la stocker dans les secrets du dépôt.
