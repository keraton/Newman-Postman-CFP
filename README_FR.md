# Postman & Newman pour vos CICD

## Pour les audiences

Postman est un outil qui permet aux utilisateurs d'appeler simplement et rapidement des APIs. Son interface intuitive, la possibilité de sauvegarder et partager ses collections de requêtes, ainsi que les différentes autres fonctionnalités ont rendu cet outil très populaire parmi les développeurs. Ce que vous ne savez pas peut-être pas, c'est que Postman a maintenant un compagnon CLI appelé Newman. Newman est un client interface en ligne de commande (open source) permettant de lancer des collections Postman. L'intégration de collections Postman au CICD est alors devenue possible.

Lors de cette session, nous allons vous montrer comment créer une collection Postman à partir d'une spécification OpenAPI afin de l'utiliser dans un processus CICD avec Newman. Nous couvrirons les techniques pour traiter différents cas d'utilisation (synchrone, asynchrone, workflow, etc..). Enfin, Newman est aussi une librairie nodejs, ce qui ouvre les possibilités d'extension et de personnalisation. En sortant de cette conférence, vous verrez Postman d'une manière différente, car en plus d'être un excellent outil pour tester manuellement ses APIs il permet de réutiliser les collections que vous avez créées dans votre cycle d'intégration et livraison continue.

## Pour le membre du jury

Utilisateur de Postman depuis bien assez longtemps, je viens de decouvrir le projet Newman. Je souhaite donc partager cette combinaison Postman et Newman que je trouve très pratique. Nous pouvons maintenant facilement exécuter les mêmes tests depuis nos postes ou dans notre pipeline CICD. La présentation sera composée de :
- Slides d'introduction sur Postman et Newman (fonctionnalités principales)
- Démonstration de la création d'une collection à partir d'une spécification OpenAPI (ex Swagger) jusqu'à son intégration dans une pipeline Jenkins
- Démonstration de plusieurs use-cases : Synchrone, Asynchrone et Workflow. 

Voici les contenus provisoire de la conférence en détails :
- Introduction Postman
  - Postman collections
  - Postman environments  
  - Request + Runner
  - Pre-request + Test
  - Autres fonctionnalités : workspace, partage en équipe, sandbox/mock, monitoring
  
- Introduction Newman
  - ClI Postman
  - Librairie nodejs (npm)
  
- Démonstration
  - Contexte : Tester une application exposant une API REST (OpenAPI)
  - Importer la spécification OpenAPI sur Postman
  - Créer des environments
  - Gestion de l'authentication
  - Création de tests
  - Tester le cas asynchrone
  - Tester la mise en place de workflow de test
  - Utiliser le Runner sur Postman
  - Exporter la collection et les environements
  - Lancer le runner en utilisant Newman
  - Intégrer Newman dans le CICD (Jenkins pipeline)
  - Montrer le rapport de Newman
  - Montrer comment utilser la librairie Newman en Serverless pour faire du monitoring/alerting
  
 - Conclusion : 
    - Points positifs : Les gens utilisent déjà Postman, on facilite donc la création de tests automatisés (pas la peine de faire appel à un autre langage/framework comme Cucumber/Karate)
    - Points négatifs : Pas de gestion de secrets intégrés. Partage de collections limité

## Références :
- https://www.getpostman.com/downloads/
- https://github.com/postmanlabs/newman
- https://www.npmjs.com/package/newman
- https://github.com/keraton/flight-service : demo project
  

