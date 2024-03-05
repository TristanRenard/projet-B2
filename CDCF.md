# Cahier des charges fonctionnel

## Introduction

Nous sommes une société qui a pour but de vendre à des boutiques la possibilité de se référencer sur notre site web pour
qu'ils puissent atteindre une nouvelle cible qui ne les aurait pas connu autrement. Mais avant de vendre notre
service à des boutiques, nous avons besoin d'un minimum d'utilisateurs pour ensuite pouvoir le commercialiser. Il nous
faut donc une première version de notre site web qui permettra à des utilisateurs de renseigner des adresses avec des
informations les concernant et de les consulter. Les utilisateurs pourront également effectuer des recherches avancées
sur les adresses enregistrées en les filtrant.

Le livrable est donc un site web, correctement documenté et fonctionnel. De plus, le code doit être correctement
organisé et propre dans l'objectif de le maintenir et de sortir des versions futures.

- [Cahier des charges fonctionnel](#cahier-des-charges-fonctionnel)
  - [Introduction](#introduction)
  - [Site map](#site-map)
  - [Layout](#layout)
    - [Le header (Nav bar)](#le-header-nav-bar)
  - [Page d'accueil](#page-daccueil)
  - [Ajout](#ajout)
  - [Détail](#détail)
  - [Modification](#modification)
  - [Suppression](#suppression)
  - [Rendu](#rendu)

## Site map

![siteMap](./images/CDCF/siteMap.png)


---

**La suite du CDCF a pour but de présenter le contenu qui doit absolument être présent dans votre application. Vous
pouvez faire soit comme recommandé dans le CDCF** (c'est très fortement encouragé dans un premier temps)**, des pages
pour chaque action de l'utilisateur, soit des popups ou des side views.**

---

## Layout

Toutes les pages doivent contenir un header :

### Le header (Nav bar)
Doit vous permettre d'accéder à toutes les pages de votre site web depuis n'importe quelle page. Ce header doit absolument être présent sur toutes les pages. Il doit contenir le logo de votre site web à gauche et les liens de navigations : "Liste" (qui devrait être la home page si vous suivez la site map du CDCF) et "Ajout". Vous pouvez évidement ajouter des liens en fonctions des fonctionnalités que vous avez implémentées.

Toutes les pages doivent contenir un header contenant :

- un logo;
- un lien vers la page d'accueil;
- un lien vers la page d'ajout d'adresse.

## Page d'accueil

La page d'accueil doit contenir un tableau ou une liste des adresses enregistrées, avec l'adresse (courte : numero +
rue + ville), le lieu dit (nom du lieu), le pays et le type de lieu (ex: restaurant, bar, etc...). La page devra
également contenir un filtre de recherche avancée pour filtrer les adresses enregistrées : si l'utilisateur filtre les
restaurants, un autre filtre lui proposera les types de cuisine (ex: italien, français, etc...) mais ce filtre ne sera
pas proposé pour un musée par exemple.

Exemple de mockup de la page d'accueil :

![mockup_Home](./images/CDCF/mockup1.png)

## Ajout

Cette page est accessible depuis n'importe quelle page du site. Elle doit contenir un formulaire pour ajouter une
adresse. Le formulaire doit contenir les champs suivants :

- Type de lieu (obligatoire, ex: restaurant, bar, etc.),
- Nom du lieu (obligatoire)
- Adresse (obligatoire)
- Ville (obligatoire)
- Code postal (obligatoire)
- Pays (obligatoire)
- Selon le type de lieu, des champs supplémentaires devront être renseignés (ex: pour un restaurant, le type de cuisine;
  pour un bar, le type de bar; pour un musée s'il est gratuit ou payant; etc...).

> Vous devez avoir obligatoirements les types de lieux suivants : 
> - Restaurant
>   - Type de cuisine (unique choix)
>   - Nombre d'étoiles (de 1 à 3)
>   - Prix moyen (de 1 à 5)
> - Musée
>   - Courant artistique (uniquement un choix)
>   - Type d'art (peinture, sculpture, etc... )
>   - Gratuit ou payant (gratuit ou de 1 à 5)
>   - Prix (facultatif : ne s'affiche que si payant)
> - Bar
>   - Type de bar (ex: bar à vin, bar à cocktail, pub, etc...) q
>   - Prix moyen (de 1 à 5)
> - Parc
>   - Type de parc (ex: parc floral, parc forestier, ...) (unique choix)
>   - Public ou privé (public ou privé)
>   - Gratuit ou payant (gratuit ou de 1 à 5)
>   - Prix (facultatif : ne s'affiche que si payant)

Exemple de mockup de la page d'ajout :
![mockup_add](./images/CDCF/mockup2.png)

## Détail

Cette page est accessible depuis le tableau la page d'accueil en cliquant sur le lieu dont on souhaite les détails. Elle
doit contenir les informations renseignées lors de l'ajout de l'adresse. Elle doit également contenir un bouton pour
modifier l'adresse et un bouton pour supprimer l'adresse.

Exemple de mockup de la page de détail :
![mockup_details](./images/CDCF/mockup3.png)

## Modification

Cette page est accessible depuis la page de détails en cliquant sur le bouton de modification. Elle doit contenir un
formulaire pré-rempli avec les informations de l'adresse. L'utilisateur pourra modifier les informations et valider le
formulaire pour enregistrer les modifications.

> Pro tip : Vous pouvez utiliser la même page et les mêmes compostants que pour l'ajout, en changeant le titre et le
> bouton de validation.

## Suppression

Vous pouvez faire une page pour confirmer la suppression ou un popup pour confirmer la suppression. Vous pouvez
également faire une suppression directe sans confirmation. C'est à vous de voir ce qui est le plus adapté à votre
application.

## Rendu

- [ ] Un repository GIT avec le code du site web;
- [ ] Le code doit être dans son entièreté sans erreur et formaté;
- [ ] le code doit être « propre » et correctement architecturé;
- [ ] Une documentation technique;
- [ ] La date limite de la livraison finale doit être au plus tard 12 semaines après la date de début du projet, délai
  qui pourra être exceptionnellement prolongé par un accord commun entre les deux parties.
