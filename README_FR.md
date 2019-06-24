# Postman & Newman pour vos CICD

## Pour les audiences

Postman est plutôt identique à un outil de test manuel qui permet aux utilisateurs d'appeler un service REST depuis son poste. Son UX design qui est intuitive et la possibilité de sauvegarder et partager ses collections rendre cet outil populaire parmi les développeurs. Ce que vous ne savez pas, c'est à côté de Postman, il y a maintenant Newman, le cli compagnon pour Postman. Newman est un client interface en ligne de commande (en open source) pour lancer les collections Postman. En utilisant Newman, l'intégration de collection Postman au CICD est devenu possible.

Cette séance va vous montrer comment écrire une collection de Postman et utiliser avec Newman dans un processus CICD. Il couvre des techniques pour traiter différents cas d'utilisation (synchrone, asynchrone, workflow etc.). Enfin, le Newman est aussi un lib de nodejs, ceci ouvre la possibilité d'extension et intégration facile avec un code en nodejs.
