![Cover](https://kpkfzczpavanzocxzyta.supabase.co/storage/v1/object/public/oc-react/readme-header-oc-react-09.png)

<!-- ∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴∵ ƸӜƷ ∴ -->

# BILLED E2E - BDD - TDD

**Jerkin** Method by NephaCode // Parcours employé.e

Il est important dans le cadre des nouvelles phases de tests de mettre à jour l'ensemble des vérifications vers un outil ou framework plus modernes. voici la liste ci-dessous de la veille pour choisir de concerver les tests ou bien de procéder à une migration partielle ou totale.

| FRAMEWORK  | TYPE                                          | URL                                | DESCRIPTION                                                                                                                                                                                            |
| ---------- | --------------------------------------------- | ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Jest       | Tests unitaires, d'intégration et de snapshot | [Jest]()                           | Framework actuel, bonne couverture des tests, plutôt lent pas très ergonomique                                                                                                                         |
| Vitest     | Tests unitaires et d'intégration                                           | [Vitest by Vite]()                 | Un framework de test conçu pour les projets utilisant Vite. Il est extrêmement rapide et utilise une syntaxe similaire à Jest.                                                                         |
| Cypress    | Tests end-to-end (E2E), tests d'intégration   | [Cypress](https://www.cypress.io/)                                                                                                                                                                                                | Un framework moderne conçu pour les tests end-to-end des applications web. Il fonctionne directement dans le navigateur et propose une interface interactive pour visualiser les tests en temps réel. **Points forts :** Facile à configurer et à utiliser pour les _tests d’interface utilisateur_. **Capture d’écran et vidéos automatiques** pour faciliter le débogage.
| Playwright | Tests end-to-end (E2E).                       |    [playwright.dev](https://playwright.dev/)                                | Un outil puissant pour les tests end-to-end qui supporte plusieurs navigateurs (Chromium, Firefox, WebKit). Il permet de simuler différents environnements et de capturer des tests multi-navigateurs. |

![Framework](https://kpkfzczpavanzocxzyta.supabase.co/storage/v1/object/public/oc-react/oc-19-frameworktest.png)

## Scénario 1

- **Given** Je suis un visiteur (non connecté.e)
- **When** Je ne remplis pas le champ e-mail ou le champ password du login employé et je clique sur le bouton `Se connecter`
- **Then** Je reste sur la page `Login` et je suis invité à remplir le champ manquant

## Scénario 2

- **Given** Je suis un visiteur (non connecté.e)
- **When** Je remplis le champ e-mail du login employé au mauvais format _sans_ la forme `address@domain.tld`
- **And** Je clique sur le bouton `Se connecter`
- **Then** Je reste sur la page Login et je suis invité à remplir le champ e-mail au bon format

## Scénario 3

- **Given** Je suis un visiteur (non connecté.e)
- **When** Je remplis le champ e-mail du login employé au bon format sous la forme `address@domain.tld`, le champ password du login employé.e
- **And** Je clique sur le bouton `Se connecter`
- **Then** Je suis envoyée sur la page Bills

## Scénario 4

- **Given** Je suis connectée en tant qu’employé.e
- **When** Je suis sur la page Bills
- **Then** La liste de mes notes de frais apparaît, triées de la plus récente à la plus ancienne

## Scénario 5

- **Given** Je suis connectée en tant qu’employé.e
- **And** Je suis sur la page `Bills`
- **When** Je clique sur le bouton _« nouvelle note de frais »_
- **Then** Je suis envoyé sur la page `NewBill`

## Scénario 6

- **Given** Je suis connectée en tant qu’employé.e
- **And** Je suis sur la page `Bills`
- **When** Je clique sur le bouton `retour` du navigateur
- **Then** Je reste connectée sur la page `Bills`

## Scénario 7

- **Given** Je suis connectée en tant qu’employé.e
- **And** Je suis sur la page `Bills`
- **When** Je clique sur le bouton `déconnexion`
- **Then** Je suis déconnecté et envoyé sur la page `login`

## Scénario 8

- **Given** Je suis connectée en tant qu’employé.e
- **And** Je suis sur la page Bills
- **When** Je clique sur `l’icône œil`
- **Then** Une fenêtre modal s’ouvre avec le justificatif

## Scénario 9 > Logout

- **Given** Je suis connectée en tant qu’employé.e
- **And** Je suis sur la page Bills et j’ai ouvert la modale
- **When** Je clique sur le bouton `quitter`
- **Then** La modale se ferme

## Scénario 10

- **Given** Je suis connectée en tant qu’employé.e
- **And** Je suis sur la page `Bills`
- **When** Je clique sur le bouton `Parcourir`
- **Then** Le fichier `` du justificatif est chargé

## Scénario 11

- **Given** Je suis connectée en tant qu’employé.e
- **And** je suis sur la page `NewBill`
- **When** Je clique sur le bouton retour du navigateur
- **Then** Je suis envoyée à la page `Bills`

## Scénario 12

- **Given** Je suis connectée en tant qu’employé.e
- **And** je suis sur la page `NewBill`
- **When** Je ne rempli pas les champs correctement 
- **And** je clique sur `envoyer`
- **Then** Je reste sur la page `NewBill` et des messages m’indiquent mes erreurs

## Scénario 13

- **Given** Je suis connectée en tant qu’employé.e
- **And** Je suis sur la page `NewBill`
- **When** Je rempli pas les champs correctement et je clique sur envoyer
- **Then** Je suis envoyé à la page Bills et ma nouvelle note de frais apparait

![Cover](https://kpkfzczpavanzocxzyta.supabase.co/storage/v1/object/public/oc-react/readme-footer-oc-react-09.png)
