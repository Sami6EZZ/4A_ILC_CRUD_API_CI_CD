<p align="center">
<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&width=435&lines=PROJECT+API+CI%2FCD+WITH+PYTHON.+ILC" alt="Typing SVG" /></a>
  </P>
  
## Le projet qu'on souhaite réaliser est un projet guidé pour la gestion CRUD d'un système de transaction, où on mettra en place ce que nous avons appris cette année avec le module de CI/CD

   ![Badge1](https://www.plunge.cloud/hs-fs/hubfs/cycle-devopsea2b.png?width=600&name=cycle-devops.png)



## Noms et prénoms du binôme : 
  WALY Mouad et EL YOUSFI Mohammed.


## Spécialité : 
  ILC.

## Le langage que nous souhaitons utiliser est :
  Python parce que, qui n'aime pas python!
  
## Fonctionnalités :

-Initialisation de l'application Flask

-Création d'une classe Personne qui permet de créer des objets Personne avec un nom et un sodle. Les objets Personne peuvent être converties en objets JSON, avoir des méthodes pour débiter ou créditer un compte, effectuer une transaction entre deux personnes.

-Méthode pour importer un fichier CSV de personnes

-Route pour afficher toutes les personnes et les transactions

-Route pour affichier les transactions sauvegargdées dans un fichier csv entre 2 personnes.

-Route pour afficher les personnes recupérées du fichier csv.

-Route pour ajouter/supprimer une personne de la liste persons.

-Route pour affichier le solde d'une personne donnée.

-Route pour afficher les transactions d'une personne donnée.


## Utilisation :

-Installation de flask avec :
    pip install flask
   
-Utilisez la route '/' pour afficher toutes les personnes et les transactions. 
    Dans un navigateur web : http://localhost:5000/ 
    Dans une commande CURL : ``curl -X GET "http://localhost:5000/"``
    
-Utilisez la route'/transactions' qui affiche la liste des transactions effectuées qui sont été lises du fichier transactions.csv.
    Dans un navigateur web : http://localhost:5000/transactions
    Dans une commande CURL : ``curl -X GET "http://localhost:5000/transactions"``
    
-Utilisez la route'/persons' qui affiche la liste des personnes crées et leurs soldes apres avoir chargé les transactions du fichier csv.
    Dans un navigateur web : http://localhost:5000/persons
    Dans une commande CURL : ``curl -X GET "http://localhost:5000/persons"``
    
     
-Utlisiez la route '/person' qui permet d'ajouter une personne de type Person ayant un nom: name et un solde: balance.
     Executez cette fonction avec la commande CURL suivante :
              ``curl -X POST -d "name=Jerome&balance=5" http://localhost:5000/person``
              
-Utilisez la route 'person/id' qui permet de supprimer une personne en donnant son id
     Executez cette fonction avec la commande CURL suivante :
          ``curl -X DELETE http://localhost:5000/person/1``

-Utlisiez la route '/transaction' qui permet de créer une nouvelle transaction en leur donnant un émetteur, un recepteur et le montant de la transaction.
    Executez cette fonction avec la commande CURL suivante :
                ``curl -X POST -d "sender=Simo&receiver=Mouad&amount=100" http://localhost:5000/transaction``
                !! attention, il faudra bien que le nom du sender our receiver soit dans la liste persons.

 -Utlisize la route '/balance/name' qui peremt d'afficher le solde de la personne donnée dans le parametre name.
    Executer cette fonction avec :
        Navigateur web : ``http://localhost:5000/balance/Mouad ``
        Commande CURL :  ``curl -X GET "http://localhost:5000/balance/Mouad"``
        !!Attention il faudra bien que le nom donné soit dans la liste persons.
        
 -Utlisize la route '/transactions/name' qui peremt d'afficher la liste des transactions de la personne donnée dans le parametre name.
    Executer cette fonction avec :
        Navigateur web : ``http://localhost:5000/transactions/Mouad ``
        Commande CURL :  ``curl -X GET "http://localhost:5000/transactions/Mouad"``
        !!Attention il faudra bien que le nom donné soit dans la liste persons.
        la personne a deja effectué une transaction  sinon cela renvoit une liste vide.

## Vous trouverez ci-dessus les différentes actions dont on a besoin dans ce projet : 

App build :
![Generic badge](https://github.com/mouadw/4A_ILC_CRUD_API_CI_CD/actions/workflows/appBuild.yml/badge.svg)

New push :
![Generic badge](https://github.com/mouadw/4A_ILC_CRUD_API_CI_CD/actions/workflows/newPush.yml/badge.svg)

Build and push tag :
![Generic badge](https://github.com/mouadw/4A_ILC_CRUD_API_CI_CD/actions/workflows/build_push.yml/badge.svg)

Build docker image :
![Generic badge](https://github.com/mouadw/4A_ILC_CRUD_API_CI_CD/actions/workflows/buildDockerImage.yml/badge.svg)

Pull req :
![Generic badge](https://github.com/mouadw/4A_ILC_CRUD_API_CI_CD/actions/workflows/pullReq.yml/badge.svg)


