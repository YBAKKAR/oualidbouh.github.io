* Notes préalables
* Objectifs
* Qu'est ce que monilithique ?
  * Présentation
  * Architecture générale
  * Exemples d'application monolithique
  * Avanatges
  * Inconvénient
* Les microservices, une révolution !
  * Présentation
  * Architecture générale
  * Exemples d'application en microservices
  * Avantages 
  * inconvénients
* L'écosystème des microservices
  * Frameworks de développement
  * Outils de déploiement
  * Outils de conteneurisation 
  * Outils de mise en production
  * Outils de monitoring
* Conclusion
* Webographie

# Notes préalables
Ce document écrit constitue le résultat de ma veille technologique que j'ai faite dans le cadre du cours MSO 4.4.
Vous pouvez retrouvez le support de présentation au format ppt et pdf.

Retrouvez mon compte [Twitter](https://twitter.com/oualidbouh) sur lequel j’ai partagé des liens en rapport avec le sujet de ma veille.
# Objectifs
A travers cette veille technologique, j’ai choisi d'expliquer qu'est-ce qu'une architecture microservice, ainsi que les outils utilisés dans l'industrie digitale pour créer des applications très robustes et scalables.

Cette synthèse s’articule en trois grandes parties, Dans la première nous verrons une explication concernant l'architecture d'une application classique dite **monolithique**, avec les avanatges et inconvénients de cette dernière.
Dans la deuxième, nous plongerons ensemble dans l' architecture microservice, nous verrons dans cette parties une défintion de ce style d'application avec ces avantages et inconvénients ainsi que quelques exemples d'applications implémentant cette architecture.
Finalment pour la troisième, nous verrons l'écosystème des microservices du développement jusqu'au déploiement.

# Qu'est ce que monilithique ?
## Présentation
Dans le monde du génie logiciel, une application qui suit l'architecture monolithique à un seul niveau dans laquelle l'interface utilisateur et la logique métier et la couche d'accés aux données sont combinés dans un seul programme avec une seule technologie (un backend avec une seule technologies, ça pourra être du JAVA, PHP) et avec une seule suite de test (unitaire, sécurité, non regression..etc) et avec une seule et unique plateforme de déploiement.
## Architecture monolithique
Voilà à quoi ressemble une application avec l'architecture monolithique : 
![Image of Yaktocat](mono_app_architecture.png)
Géneralement, nous pouvons découpler une application en monolithque en trois couches.
La première est la couche de présentation, cette couche peut être sous la forme d'une application Web ou d'une application Mobile, elle permet d'intercepter les actions de l'utilisateur tel que la saisi et suppression par exemple. la deuxième est la couche applicative, cette dernière contient la logique métier de l'application, elle interégie directement avec la couche précedente à l'aide du protocole **HTTP** donc elle intercepte les actions utilisateurs et les execute.
# Les microservices, une révolution !
