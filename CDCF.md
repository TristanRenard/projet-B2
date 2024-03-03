# Cahier des charges fonctionnel

## Introduction

Nous sommes une société qui a pour but de vendre à des boutiques la possibilité de se référencer sur notre site web pour qu'ils puissent attiendre une nouvelle cible qui ne les auraient pas connu autrement. Mais avant de vendre notre service, à des boutiques nous avons besoin d'un minimum d'utilisateurs, pour ensuite pouvoir commercialiser notre service. Il nous faut donc une première version de notre site web qui permettra à des utilisateurs de renseigner des adresses avec des informations les concernants et de les consulter. Les utilisateurs pourront également effectuer des recherches avancées sur les adresses enregistrées en les filtrants.

Le livrable est donc un site web, correctement documenté et fonctionnel. De plus le code doit être correctement organisé et propre dans l'objectif de le maintenir et de sortir des versions futures.


- [Cahier des charges fonctionnel](#cahier-des-charges-fonctionnel)
  - [Introduction](#introduction)
  - [Site map](#site-map)
  - [Layout](#layout)
    - [Le header](#le-header)
  - [Page d'accueil](#page-daccueil)
  - [Ajout](#ajout)
  - [Détail](#détail)
  - [Modification](#modification)
  - [Suppression](#suppression)
  - [Rendu](#rendu)


## Site map

![siteMap](./images/CDCF/siteMap.png)


---

**La suite du CDCF à pour but de présenter le contenu qui doit absolument être présent dans votre application. Vous pouvez faire soit comme recommandé dans le CDCF** (c'est très fortement encouragé dans un premier temps)**, en faisant des pages pour chaque action de l'utilisateur, soit en faisant des popups ou des side views.**

---


## Layout
Toutes les pages doivent contenir un header :

### Le header
doit vous permettre d'accéder à toutes les pages de votre site web depuis n'importe quelle page. et doit absolument être présent sur toutes les pages. Il doit également contenir le logo de votre site web.


## Page d'accueil
La page d'accueil doit contenir un tableau ou une liste des adresses enregistrées, avec l'adresse (courte : numero + rue + ville)
, le lieu dit (nom du lieu), le pays et le type de lieu (ex: restaurant, bar, etc...).
La page devra également contenir un filtre de recherche avancée pour filtrer les adresses enregistrées :
Si L'utilisateur filtre les restaurants, un autre filtre lui proposera les types de cuisine (ex: italien, français, etc...) mais ce filtre ne sera pas proposé pour un musée par exemple.

Exemple de mockup de la page d'accueil :

![mockup_Home](./images/CDCF/mockup1.png)

## Ajout
Cette page est accessible depuis n'importe quelle page du site. Elle doit contenir un formulaire pour ajouter une adresse. Le formulaire doit contenir les champs suivants :
- Type de lieu (obligatoire, e.g: restaurant, bar, etc.),
- Nom du lieu (obligatoire)
- Adresse (obligatoire)
- Ville (obligatoire)
- Code postal (obligatoire)
- Pays (obligatoire)
- Selon le type de lieu, des champs supplémentaires devront être renseignés (ex: pour un restaurant, le type de cuisine, pour un bar, le type de bar, pour un musée si il est gratuit ou payant, etc...).

> Vous devez avoir obligatoirements les types de lieux suivants : 
> - Restaurant
>   - Type de cuisine
>   - Nombre d'étoiles
>   - Prix moyen
> - Musée
>   - Courant artistique
>   - Type d'art (peinture, sculpture, etc... )
>   - Gratuit ou payant
>   - Prix
> - Bar
>   - Type de bar (ex: bar à vin, bar à cocktail, pub, etc...)
>   - Prix moyen
> - Parc
>   - Type de parc (ex: parc floral, parc forestier, ...)
>   - Public ou privé
>   - Prix

Exemple de mockup de la page d'ajout :
![mockup_add](./images/CDCF/mockup2.png)

## Détail
Cette page est accessible depuis le tableau la page d'accueil en cliquant sur le lieu dont on souhaite les détails. Elle doit contenir les informations renseignées lors de l'ajout de l'adresse. Elle doit également contenir un bouton pour modifier l'adresse et un bouton pour supprimer l'adresse.

Exemple de mockup de la page de détail :
![mockup_details](./images/CDCF/mockup3.png)

## Modification
Cette page est accessible depuis la page de détail en cliquant sur le bouton de modification. Elle doit contenir un formulaire pré-rempli avec les informations de l'adresse. L'utilisateur pourra modifier les informations et valider le formulaire pour enregistrer les modifications.

> Pro tip : Vous pouvez utiliser la même page et les mêmes compostants que pour l'ajout, en changeant le titre et le bouton de validation.


## Suppression
Vous pouvez faire une page pour confirmer la suppression ou un popup pour confirmer la suppression. Vous pouvez également faire une suppression directe sans confirmation. C'est à vous de voir ce qui est le plus adapté à votre application.


## Rendu
- [ ] Un repository GIT avec le code du site web.
- [ ] le code doit être dans son entièreté sans erreur et formaté ;
- [ ] le code doit être « propre » et correctement architecturé,
- [ ] une documentation technique ;
- [ ] la date limite de la livraison finale doit être au plus 12 semaines après la date de début du projet, délai qui pourra être exceptionnellement prolongé par un accord commun entre les deux parties.
