# Postman & Newman pour vos CICD

## Pour les audiences

Postman est plutôt identique à un outil de test manuel qui permet aux utilisateurs d'appeler un service REST depuis son poste. Son UX design qui est intuitive et la possibilité de sauvegarder et partager ses collections rendre cet outil populaire parmi les développeurs. Ce que vous ne savez pas, c'est à côté de Postman, il y a maintenant Newman, le cli compagnon pour Postman. Newman est un client interface en ligne de commande (en open source) pour lancer les collections Postman. En utilisant Newman, l'intégration de collection Postman au CICD est devenu possible.

Cette séance va vous montrer comment écrire une collection de Postman et utiliser avec Newman dans un processus CICD. Il couvre des techniques pour traiter différents cas d'utilisation (synchrone, asynchrone, workflow etc.). Enfin, le Newman est aussi un lib de nodejs, ceci ouvre la possibilité d'extension et personnalissation selon vos besoin. Sortant de cette conférence, vous allez penser à traiter Postman différemment et réutiliser cette fois-ci pour CICD.

## Pour le membre du jury

Utilisateur de Postman depuis bien assez long temps, je viens de decouvrir le projet Newman. Je souhaite donc partager cette combination de Postman et Newman que je trouve très pratiques car maintenant on peut facilement executer les mêmes test depuis notre poste ou depuis CICD. La présentation sera composé de 
- Des slides sur l'introduction de Postman et Newman (sur leur features)
- Demo qui montre la création d'une collection à partir de Open API (Swagger) jusqu'a le deployment sur Jenkins Pipeline
- Demo sur plusieurs use case : Synchrone, Asynchrone et Workflow. 

Voici les contenu provisoire de conférence en détail :
