![Cover](https://kpkfzczpavanzocxzyta.supabase.co/storage/v1/object/public/oc-react/readme-header-oc-react-09.png)

<!-- ∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴ -->

# UNDERCONSTRUCTION

TESTS UNITS JEST

## PROJECT DELIVERIES

| WHAT FOR               | WHEN         |
| :--------------------- | ------------ |
| Deadline MVP           | `18-03-2024` |
| Deadline CERTIFICATION | `15-04-2024` |

## INFORMATIONS

| WHO IS   | FOR             |      COMPANY      | CONTACT | DISCORD |
| :------- | --------------- | :---------------: | ------- | :-----: |
| Nephelim | Head of concept | Underconstruction | #       |   YES   |

## TECHNO

| TECHNO   | SPEC             |
| :------- | ---------------- |
| FRONTEND | `SASS` `VANILLA` |
| TEST     |  `JEST`          |

## PROJECT

| RESSOURCES        | URL                                                                                                                                      |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Le projet OC      | [Scénario](https://openclassrooms.com/fr/paths/516/projects/809/scenario)                                                                |
| Repo BackeND      | [Github Backend](https://github.com/OpenClassrooms-Student-Center/Billed-app-FR-back)                                                    |
| Notion            | [Bug Report](https://openclassrooms.notion.site/a7a612fc166747e78d95aa38106a55ec?v=2a8d3553379c4366b6f66490ab8f0b90)                     |
| Billed Plan       | [DOWNLOAD PDF](./billed-plan.pdf)                                                                                                        |
| COURS OC TEST     | [Testez l'interface de votre site](https://openclassrooms.com/fr/courses/3504461-testez-linterface-de-votre-site)                        |
| COURS OC DEBUG    | [Déboguez l’interface de votre site internet](https://openclassrooms.com/fr/courses/7159296-deboguez-l-interface-de-votre-site-internet) |
| COURS OC TEST APP | [Testez vos app JavaScript](https://openclassrooms.com/fr/courses/7159306-testez-vos-applications-front-end-avec-javascript)             |

## FONCTIONNALITÉS DESCRIBES

| FEATURE                               | DESCRIBES                                                                                                                                                                                                                                                                                                        |
| ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Page Login                            | Possibilité de se connecter en tant qu’employé, ou en tant qu’administrateur RH                                                                                                                                                                                                                                  |
| Connecté en tant qu’employé           | Après s’être connecté sur la page “Login”, l’employé arrive sur la liste des notes de frais qu’il a déjà transmises, avec les données pertinentes notamment le statut de la note de frais. Il peut savoir si sa dernière note de frais a été validée ou non. Il peut voir le justificatif ou télécharger le PDF. |
| Connecté en tant qu’employé           | S’il clique sur “Nouvelle note de frais”, il peut saisir les informations d’une nouvelle note de frais. S’il clique sur “Envoyer”, la note de frais est envoyée aux administrateurs RH.                                                                                                                          |
| Connecté en tant qu’employé           | S’il navigue en arrière, il reste connecté. S’il clique sur le bouton “Se déconnecter”, il est envoyé sur la page Login.                                                                                                                                                                                         |
| Connecté en tant qu’administrateur RH | Après s’être connecté sur la page Login, l’administrateur arrive sur son dashboard. À gauche, un feed avec l’ensemble des notes de frais des employés, regroupées par statut (en attente, acceptées, refusées).                                                                                                  |
| Connecté en tant qu’administrateur RH | S’il clique sur une des notes de frais en statut “pending”, il peut accepter ou refuser la note de frais.                                                                                                                                                                                                        |
| Connecté en tant qu’administrateur RH | S’il clique sur une note de frais déjà traitée, il peut consulter ses informations.                                                                                                                                                                                                                              |
| Connecté en tant qu’administrateur RH | S’il clique sur une note de frais, quel que soit son statut, il peut visualiser le justificatif ou le télécharger.                                                                                                                                                                                               |
| Connecté en tant qu’administrateur RH | S’il navigue en arrière, il reste sur la même page.                                                                                                                                                                                                                                                              |
| Connecté en tant qu’administrateur RH | S’il clique sur le bouton “Se déconnecter”, il est envoyé sur la page Login                                                                                                                                                                                                                                      |

## RUNNING THE APPS

## L'architecture du projet :

Ce projet, dit frontend, est connecté à un service API backend que vous devez aussi lancer en local.

Le projet backend se trouve ici:

## Organiser son espace de travail :

Pour une bonne organization, vous pouvez créer un dossier bill-app dans lequel vous allez cloner le projet backend et par la suite, le projet frontend:

Clonez le projet backend dans le dossier bill-app :

```
$ git clone https://github.com/OpenClassrooms-Student-Center/Billed-app-FR-Back.git
```

```
bill-app/
   - Billed-app-FR-Back
```

Clonez le projet frontend dans le dossier bill-app :

```
$ git clone https://github.com/OpenClassrooms-Student-Center/Billed-app-FR-Front.git
```

```
bill-app/
   - Billed-app-FR-Back
   - Billed-app-FR-Front
```

## Comment lancer l'application en local ?

### étape 1 - Lancer le backend :

Suivez les indications dans le README du projet backend.

### étape 2 - Lancer le frontend :

Allez au repo cloné :

```
$ cd Billed-app-FR-Front
```

Installez les packages npm (décrits dans `package.json`) :

```
$ npm install
```

Installez live-server pour lancer un serveur local :

```
$ npm install -g live-server
```

Lancez l'application :

```
$ live-server
```

Puis allez à l'adresse : `http://127.0.0.1:8080/`

## Comment lancer tous les tests en local avec Jest ?

```
$ npm run test
```

## Comment lancer un seul test ?

Installez jest-cli :

```
$npm i -g jest-cli
$jest src/__tests__/your_test_file.js
```

## Comment voir la couverture de test ?

`http://127.0.0.1:8080/coverage/lcov-report/`

## Comptes et utilisateurs :

Vous pouvez vous connecter en utilisant les comptes:

### administrateur :

```
utilisateur : admin@test.tld
mot de passe : admin
```

### employé :

```
utilisateur : employee@test.tld
mot de passe : employee
```

![Cover](https://kpkfzczpavanzocxzyta.supabase.co/storage/v1/object/public/oc-react/readme-footer-oc-react-09.png)
