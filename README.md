# WORK IN PROGRESS
# ViewFanPopup
Documentation d'intégration de ViewFan Popup

Ce guide a pour objectif de vous guider dans la mise en place du widget JS ViewFan Popup dans votre site web.

Pour rappel, ViewFan est une solution de micro-paiement par l'attention publicitaire, qui permet à l'utilisateur de soutenir le site de son choix en regardant une publicité. ViewFan Popup a été fait pour aider les utilisateurs qui le souhaitent à soutenir leurs éditeurs favoris.

Voici un exemple de déblocage d'article avec Viewpay : 

![sample](https://github.com/TechViewpay/ViewPay-iOS/blob/master/DocImages/parcours_vp_mobile3.png?raw=true)

## Chargement du Javascript
```html
<script type="text/javascript" src="https://cdn.jokerly.com/scripts/ViewFanPopup.js?id=[yourViewPaySiteID]&nb=[frequency]"></script>
```
Le fichier ViewFanPopup.js est le seul fichier nécessaire à appeler, celui-ci fera ensuite le travail afin d'appeler les éléments nécessaires pour un moment donné.
Ce fichier est installé sur notre CDN afin de vous garantir d'avoir toujours la dernière version.
NB: Il faut placer le script le plus haut possible dans la page afin d’optimiser son temps de chargement.

## Paramètres du fichier JS

yourViewPaySiteID : est le site ID que votre contact ViewPay vous aura transmis, ou que vous aurez récupéré dans votre compte le cas échéant.

nb : est la fréquence d'apparition de la popup qui propose à l'utilisateur de soutenir le site. 
Exemple : "nb=2" signifie que la popup s'affichera toutes les 2 pages vues par le même utilisateur.
