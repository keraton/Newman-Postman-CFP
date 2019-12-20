# Présentation de Newman, le CLI Postman

## Pour les audiences

Postman est un outil qui permet aux utilisateurs d'appeler simplement et rapidement des APIs. Son interface intuitive, la possibilité de sauvegarder et partager ses collections de requêtes, ainsi que les différentes autres fonctionnalités ont rendu cet outil très populaire parmi les développeurs. Ce que vous ne savez pas peut-être pas, c'est que Postman a maintenant un compagnon CLI appelé Newman. Newman est un client interface en ligne de commande (open source) permettant de lancer des collections Postman. L'intégration de collections Postman au CICD est alors devenue possible.

Lors de cette session, nous allons vous présenter une collection Postman utilisant toutes les fonctionnalités disponibles afin de l'intégrer dans le processus CICD en utilisant Newman. Nous couvrirons les techniques pour traiter différents cas d'utilisation (appels synchrones, asynchrones, workflows, etc..). Enfin, Newman est aussi une librairie nodejs, ce qui ouvre les possibilités d'extension et de personnalisation. En sortant de cette conférence, vous verrez Postman d'une manière différente, car en plus d'être un excellent outil pour tester et développer manuellement ses APIs, il permet de réutiliser les collections que vous avez créées dans votre cycle d'intégration et livraison continue.

## Pour le membre du jury

Nous avons déjà presenté ce sujet lors de la conférence Devoxx Belgium. Nous nous appuirons sur les retours que nous avons eu pour améliorer la présentation. Notamment en ce concentrant d'avantage sur la partie Newman.

Utilisateur de Postman depuis bien assez longtemps, je viens de decouvrir le projet Newman. Je souhaite donc partager cette combinaison Postman et Newman que je trouve très pratique. Nous pouvons maintenant facilement exécuter les mêmes tests depuis nos postes ou dans notre pipeline CICD. La présentation sera composée de :
- Slides d'introduction sur Postman et Newman
- Revue d'une collection Postman et des différentes fonctionnalités disponibles (scénarios de tests: synchrones, asynchrones et workflows)
- Démonstration de plusieurs cas d'utilisation de Newman: intégration CICD puis monitoring
- Comment personnaliser newman via des extensions, Comment l'utiliser en tant que librarie NodeJS

Voici les contenus provisoires de la conférence en détails :
Démonstration
- Contexte : Tester une application exposant une API REST

- Postman
  - Présenter les environments, la gestion de l'authentication, les tests et les scripts chaijs
  - Tester les cas synchrones, asynchrones et les workflows de test

- Newman
  - Exporter collections et environements
  - Utilisation du runner Newman
  - Intégrer Newman dans le CICD (Jenkins pipeline)    
  - Montrer les extentions Newman
  - Présenter comment utilser la librairie Newman en tant que paquet NodeJS pour faire du monitoring/alerting
  - Comment on peut gérer les secrets
  
 - Conclusion : 
  - Devez-vous adopter Newman ? Comparaisons avec d'autres solutions disponibles
    - Le cas idéal, votre équipe utilise déjà Postman et n'a pas encore de tests d'acceptation automatique
    - Vous n'avez pas encore automatisé vos tests d'acceptation
    - Vos tests sont difficilement maintenable et vous voulez vous concentrer sur votre métier

## Références :
- https://www.getpostman.com/downloads/
- https://github.com/postmanlabs/newman
- https://www.npmjs.com/package/newman
- https://github.com/keraton/flight-service : demo project
  

