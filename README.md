# Activer le déploiement continue

## Créer un projet sur deliverous

Rendez-vous sur https://deliverous.com/manager/ pour créer un nouveau projet. Appelez le `IUT2020 Nom du projet` Il est important qu'il commance par IUT2020.

* **Repository**, renseignez l'url de votre projet `deploy`
* Générer une nouvelle clé ssh pour donner accès à votre dépot `deploy`, gardez-là, nous en aurons besoins plus tard.
* **Triggers**, ajouter un trigger pour permettre à gitlab de déclencher le déploiement, gardez l'URL, nous en aurons besoins plus tard.
* **IPs**, ajouter 1 IP, gardez la, vous en aurez besoins.

## Sur votre sous-dossier de groupe

* dans CI/CD settings, ajouter une variable `DELIVEROUS_TRIGGER` avec le tocken présent à la fin de l'URL de trigger

## Nom de domain

* Ajouter une issue sur votre projet deploy pour me demander de renseigner dans les DNS l'IP que vous avez.
* Mettre à jour le fichier [Deliverous](Deliverous) avec la bonne IP
* Renomer puis mettre à jour le fichier [skeleton.azae.eu.conf](skeleton.azae.eu.conf)

## Projet android

* rendre les "gitlab pages" accessible à tous
