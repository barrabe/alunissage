# Alunissage

Jeu d'alunissage pour Android : module lunaire, trois commandes (gauche, poussée, droite), relief régénéré à chaque partie, physique lunaire réaliste, niveaux, astres, sons, vibration et score.

## Structure

- `app/src/main/assets/index.html` : le jeu (HTML, CSS, JavaScript), polices incluses, fonctionne hors ligne.
- `app/src/main/java/.../MainActivity.java` : conteneur plein écran, écran maintenu allumé, pause automatique quand l'appli passe en arrière-plan, pont de vibration natif.
- `.github/workflows/build.yml` : compilation et publication automatiques.

## Note sur la signature

La clé fournie convient à un usage personnel et à une diffusion directe. Pour une publication sur le Play Store, il faudra générer une clé privée dédiée et la stocker dans les secrets du dépôt.
