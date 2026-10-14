# classinus-updates

Dépôt public qui sert les mises à jour OTA de l'appli Classinus installée sur Android. Il permet de mettre à jour le code web de l'appli sans réinstaller l'APK.

Il ne contient aucun code source de l'appli, seulement les bundles compilés.

- `latest.json` : décrit la dernière version disponible (identifiant, adresse du zip, empreinte de vérification, numéro d'APK minimum, heure de construction). L'appli le lit à chaque ouverture.
- Releases : un `bundle.zip` par version. Seules les dernières versions sont gardées.

Rien ne se modifie à la main ici. Tout est publié automatiquement par le workflow `.github/workflows/ota.yml` du dépôt `classinus-frontend`, à chaque push sur sa branche `main`.
