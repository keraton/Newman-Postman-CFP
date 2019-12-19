# Présentation de Newman, le CLI Postman

## Pour les audiences

Postman est un outil qui permet aux utilisateurs d'appeler simplement et rapidement des APIs. Son interface intuitive, la possibilité de sauvegarder et partager ses collections de requêtes, ainsi que les différentes autres fonctionnalités ont rendu cet outil très populaire parmi les développeurs. Ce que vous ne savez pas peut-être pas, c'est que Postman a maintenant un compagnon CLI appelé Newman. Newman est un client interface en ligne de commande (open source) permettant de lancer des collections Postman. L'intégration de collections Postman au CICD est alors devenue possible.

Lors de cette session, nous allons vous montrer une collection Postman utilisant tous ses fonctionnalités afin de l'utiliser dans un processus CICD avec Newman. Nous couvrirons les techniques pour traiter différents cas d'utilisation (synchrone, asynchrone, workflow, etc..). Enfin, Newman est aussi une librairie nodejs, ce qui ouvre les possibilités d'extension et de personnalisation. En sortant de cette conférence, vous verrez Postman d'une manière différente, car en plus d'être un excellent outil pour tester manuellement ses APIs il permet de réutiliser les collections que vous avez créées dans votre cycle d'intégration et livraison continue.

## Pour le membre du jury

Nous avons déjà presenté ce sujet lors de conference de Devoxx Belgium. Nous nous appuirons sur les retours que nous avons eu pour améliorer la présentation. Notamment en ce concentrant d'avantage sur la partie Newman.

Utilisateur de Postman depuis bien assez longtemps, je viens de decouvrir le projet Newman. Je souhaite donc partager cette combinaison Postman et Newman que je trouve très pratique. Nous pouvons maintenant facilement exécuter les mêmes tests depuis nos postes ou dans notre pipeline CICD. La présentation sera composée de :
- Slides d'introduction sur Postman et Newman
- Démonstration d'une collection Postman avec ses fonctionnalités (use-cases : Synchrone, Asynchrone et Workflow)
- Démonstration de plusieurs cas d'usage de Newman: intégration CICD, monitoring
- Comment personnaliser newman via des extensions, Comment l'utiliser en tant que librarie NodeJS

Voici les contenus provisoire de la conférence en détails :
Demonstration
- Contexte : Tester une application exposant une API REST

- Postman
  - Montrer les environments, gestion de l'authentication, les tests et les scripts
  - Tester le cas asynchrone et le workflow de test

- Newman
  - Exporter la collection et les environements
  - Lancer le runner en utilisant Newman
  - Intégrer Newman dans le CICD (Jenkins pipeline)    
  - Montrer les extentions de Newman
  - Montrer comment utilser la librairie Newman en tant que librarie NodeJS pour monitoring/alerting
  - Montrer comment on peut gerer les secrets
  
 - Conclusion : 
  - Est-ce-que vous devez adopter NewmaN ?
    - Le cas idéal si vos équipes utilisent déjà Postman
    - Ou s'il n'y a pas encore des tests
    - Si vos tests ne sont pas maintenable

## Références :
- https://www.getpostman.com/downloads/
- https://github.com/postmanlabs/newman
- https://www.npmjs.com/package/newman
- https://github.com/keraton/flight-service : demo project
  

