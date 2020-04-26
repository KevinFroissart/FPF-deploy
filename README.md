# Activer le déploiement continu

La version en video : https://video.ploud.fr/videos/watch/5fd4bb72-693a-49ce-9a6e-7e80a320e12c

## Créer un projet sur deliverous

Rendez-vous sur https://deliverous.com/manager/ pour créer un nouveau projet. Appelez le `IUT2020 Nom du projet` Il est important qu'il commence par IUT2020.

* **Repository**, renseignez l'url de votre projet `deploy`
* Générez une nouvelle clé ssh pour donner accès à votre dépôt `deploy`, gardez-là, nous en aurons besoin plus tard.
* **Triggers**, ajoutez un trigger pour permettre à gitlab de déclencher le déploiement, gardez l'URL, nous en aurons besoin plus tard.
* **IPs**, ajoutez 1 IP, gardez la, vous en aurez besoin.

## Sur votre sous-dossier de groupe

* dans CI/CD settings, ajoutez une variable `DELIVEROUS_TRIGGER` avec le tocken présent à la fin de l'URL de trigger

## Nom de domaine

* Ajoutez une issue sur votre projet deploy pour me demander de renseigner dans les DNS l'IP que vous avez.
* Mettez à jour le fichier [Deliverous](Deliverous) avec la bonne IP
* Renommez puis mettez à jour le fichier [skeleton.azae.eu.conf](skeleton.azae.eu.conf)

## Projet android

* rendez les "gitlab pages" accessibles à tous
