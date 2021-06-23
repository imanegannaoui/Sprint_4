# Workshop 2 "Créer une API Rest"

## Prerequisites
* PHP
* MySQL
* Composer
* Postman

## APIs

<table>
    <thead>
        <tr>
            <th align="left">API</th>
            <th align="center">CRUD</th>
            <th align="right">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="left">GET /posts</td>
            <td align="center"><strong>READ</strong></td>
            <td align="right">Get all the Posts from <code>post</code> table</td>
        </tr>
        <tr>
            <td align="left">GET /post/{id}</td>
            <td align="center"><strong>READ</strong></td>
            <td align="right">Get a single Post from <code>post</code> table</td>
        </tr>
        <tr>
            <td align="left">POST /post</td>
            <td align="center"><strong>CREATE</strong></td>
            <td align="right">Create a Post and insert into <code>post</code> table</td>
        </tr>
        <tr>
            <td align="left">PUT /post/{id}</td>
            <td align="center"><strong>UPDATE</strong></td>
            <td align="right">Update the Post in <code>post</code> table</td>
        </tr>
        <tr>
            <td align="left">DELETE /post/{id}</td>
            <td align="center"><strong>DELETE</strong></td>
            <td align="right">Delete a Post from <code>post</code> table</td>
        </tr>
    </tbody>
</table>

## FAQs

Avant de commencer le brief vous devez répondre à certains questions : 
* Qu'est-ce qu'une API ?
* Que signifie REST ?
* Comment fonctionne POSTMAN ?


## Mission

Dans ce brief vous devez traiter les bases de la création d'une API REST, en utilisant l'exemple de l'accès à une base de données de produits.

Lors de la création de votre API, nous devez garder en tête les critères qui en font une API REST. Une API REST se doit d'être :

    * __Sans état :__ le serveur ne fait aucune relation entre les différents appels d'un même client. Il ne connaît pas l'état du client entre ces transactions

    * __Cacheable :__ le client doit être capable de garder vos données en cache pour optimiser les transactions

    * __Orienté client-serveur :__ Il vous faut une architecture client-serveur

    * __Avec une interface uniforme :__ ceci permet à tout composant qui comprend le protocole HTTP de communiquer avec votre API

    * __Avec un système de couches :__ avec des serveurs intermédiaires, le client final ne doit pas savoir si il est connecté au serveur principal ou à un serveur intermédiaire

### La base de données 
Pour votre API, vous allez utiliser une base de données simple, contenant des "categories" et des "produits". Sa modélisation est la suivante:

![Database produits](https://github.com/imanegannaoui/Sprint_4/blob/main/02_API_REST/DB_Produit.png)

### Les méthodes CRUD + API
On vous demanded de créer :
* Créer un produit(POST)
* Lister de tous les produits (GET)
* Lire un seul produit (GET)
* Modifier un produit (PUT)
* Supprimer un produit (DELETE)

Vous devez indiquer le rôle exact de chaque méthode HTTP dans votre API en utilisant les entêtes, puis traiter les données en ``JSON``

Pour tester votre API websrevice vous pouvez utiliser POSTMAN sur Chrome.

Une fois que vous avez créé votre API, il serait bon que vous puissiez l'héberger afin qu'elle soit accessible à tous.

## Pour aller plus loin ! 

Dans notre exemple, on souhaite sécuriser notre API RESTful construite et protéger les échanges entre le client et celle-ci avec :
* Utilisation de HTTPS
* Authentification 
* Token JWT
* Autorisation
* Clé API
* Gestion des identités


