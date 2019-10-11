# FiftyInTech

## Le projet

outil de visualisation d’un profil utilisateur avec inscription et authentification, email / mot de passe.
Votre application sera simple mais ergonomique.

## Consignes
Le back end doit être en NodeJs et utiliser le micro-framework Express.
Le front end sera développé dans la technologie de votre choix mais utiliser Angular est un plus.
L’authentification, l’enregistrement et la récupération des informations se fera via une API
Le choix de la base de données est libre.

Nous serons particulièrement attentifs à la facilité d’utilisation et à la sécurité.

Le formulaire d’inscription devra comprendre les champs suivants:
* nom
* prénom
* email
* mot de passe
* photo de profil
* compétences professionnelles
* genre (homme / femme)

Une fois connecté, l’utilisateur doit pouvoir éditer son profil.

BONUS: création d’un interface administrateur qui pourra visualiser tous les profils créés et les modifier.

## Realisation

Le projet a été realisé avec Angular CLI et AWS Amplify.

Le backend utilise AWS Cognito pour l'authentification, Dynamodb pour la base utilisateurs et S3 pour le stockage des images utilisateur.

L'utilisation de Amplify permet une architecture serverless ainsi que une approche mobile first.

Les choix technologiques ont été faites avec les objectifs suivants:

* Conformité aux consignes
* Developpement rapide (RAD)
* Securité
* Maturité des solutions
* Minimisation de la dette

## Informations importantes

* Le username doit etre une email valide.
* Le mot de passe doit contenir majuscules, minuscules, chiffres et caracteres speciaux et compter au moins 8 caracteres
* L'URL pour acceder au service est: http://iftynech-20191011015329-hostingbucket-dev.s3-website-eu-west-1.amazonaws.com

## Bugs

Les bugs connus:
* echec de telechargement de l'image par cause de droits d'acces S3
* information sur le genre n'est pas affichée

## Usual stuff

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.3.8.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
