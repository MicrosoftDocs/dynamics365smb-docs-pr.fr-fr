---
title: FAQ Power BI
description: Obtenez des réponses à certaines questions courantes sur l’utilisation de Power BI et de Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Power BI, reports, faq, errors
ms.date: 04/22/2021
ms.author: jswymer
ms.openlocfilehash: 939b280e631113d3196f6fbbc90d9bf19b9fc408
ms.sourcegitcommit: a76475f124e79440a5bba20577b335c4d50a2d83
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025832"
---
# <a name="power-bi--faq"></a>FAQ Power BI

Cet article répond à certaines des questions que vous pourriez vous poser sur l’utilisation de Power BI et [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="general"></a>[Général](#tab/general)
<!-- 26 -->
### <a name="ive-selected-a-report-for-my-role-center-in-business-central-if-i-later-make-changes-to-the-reports-visuals-online-will-the-role-center-automatically-update-to-my-changes"></a>J′ai sélectionné un état pour mon tableau de bord dans Business Central. Si j′apporte ultérieurement des modifications aux éléments visuels de l′état en ligne, le tableau de bord sera-t-il automatiquement mis à jour avec mes modifications ?

Oui, parce que les états sont intégrés à partir de Power BI.

<!-- 3 -->
### <a name="are-the-business-central-apps-for-power-bi-available-in-languages-other-than-english"></a>Les applications Business Central pour Power BI sont-elles disponibles dans d′autres langues que l′anglais ?

Non. Ces applications ne sont actuellement disponibles qu′en anglais.

<!-- 24 -->
### <a name="once-a-report-is-published-on-mypowerbicomworkspace-can-i-download-its-pbix"></a>Une fois qu′un état est publié sur mon espace de travail powerbi.com, puis-je télécharger son pbix ? 

Oui. Pour plus d′informations, voir [Télécharger un état du service Power BI vers Power BI Desktop](/power-bi/create-reports/service-export-to-pbix).  

<!-- 27 -->
### <a name="can-i-download-the-apps-as-pbix-files"></a>Puis-je télécharger les applications sous forme de fichiers pbix ? 

Non. Actuellement, nous ne proposons pas le téléchargement des fichiers pbix pour les applications Power BI officielles car elles sont publiées sur AppSource.

## <a name="license"></a>[Licence](#tab/license)

<!-- 14 -->
### <a name="do-i-need-a-power-bi-pro-license-to-publish-reports"></a>Ai-je besoin d′une licence Power BI Pro pour publier des états ? 

<!-- todo What does " or for every user that consults the published report" mean? fixed -->
Non. Une licence Pro n′est pas nécessaire pour publier des états. La licence Power BI standard (gratuite) suffit. Pour plus d’informations, reportez-vous à la rubrique [Gestion des licences Power BI](admin-powerbi-setup.md#license).

<!-- 15 -->
### <a name="is-there-anything-i-cant-do-with-the-free-license"></a>Y a-t-il quelque chose que je ne peux pas faire avec la licence gratuite ?

Vous ne pouvez pas partager d′états ni installer les applications Business Central pour Power BI. En dehors de cela, la licence gratuite permet de créer presque toutes les variations de graphiques et d′états.

<!-- 16 -->
### <a name="if-someone-shares-a-report-with-another-person-then-that-person-needs-a-pro-license-to-see-the-report-are-there-plans-to-make-this-capability-possible-with-the-free-license"></a>Si une personne partage un état avec une autre personne, cette dernière a besoin d′une licence Pro pour afficher l′état. Est-il prévu de rendre cette fonction possible avec la licence gratuite ?

Nous n′avons aucun contrôle sur cette exigence. Cette exigence est définie par Power BI. Pour plus d′informations, voir [Partager les tableaux de bord et les états Power BI avec des collègues et autres](/power-bi/collaborate-share/service-share-dashboards).  

## <a name="designer"></a>[Concepteur](#tab/designer)

<!-- 7 -->
### <a name="does-the-connector-work-with-api-pages"></a>Le connecteur fonctionne-t-il avec les pages API ?

Pas encore. Mais à compter de juin 2021, le nouveau connecteur Power BI prendra en charge à la fois les services Web Business Central et les pages API. Pour plus d′informations, voir [Activer le connecteur Power BI pour utiliser les API Business Central plutôt que les services Web uniquement](/dynamics365-release-plan/2021wave1/smb/dynamics365-business-central/enable-power-bi-connector-work-business-central-apis-instead-web-services-only).

<!-- 11 --> 
### <a name="is-it-possible-to-choose-which-business-central-environment-to-get-data-from-for-power-bi-for-example-like-a-sandbox-or-production-environment"></a>Est-il possible de choisir depuis quel environnement Business Central obtenir les données pour Power BI, comme un bac à sable ou un environnement de production ? 

Oui. Le choix est facile. Lorsque vous vous connectez à Business Central à l′aide du connecteur, vous devez choisir l′environnement et le nom de l′entreprise.

<!-- 6 --> 
### <a name="can-i-merge-data-from-several-production-environments-of-the-same-tenant"></a>Puis-je fusionner les données de plusieurs environnements de production du même abonné ?

Oui. Dans Power BI, exécutez à nouveau l′opération d′obtention des données et choisissez l′environnement souhaité.

<!-- 25 -->
### <a name="which-pages-in-business-central-have-the-power-bi-report-part"></a>Quelles pages de Business Central contiennent la partie État Power BI ?  

Actuellement, plusieurs pages contiennent un Récapitulatif avec une partie **États Power BI** pour afficher un état. 

Sur les pages de liste, la partie **États Power BI** est filtrée pour afficher les états relatifs aux données de la liste. Voici les pages de type liste qui incluent la partie **États Power BI** :

|ID page|Name|
|-------|----|
|22|Liste des clients|
|27|Liste des fournisseurs|
|31|Liste des articles|
|9305|Liste des commandes vente|
|9308|Factures achat|

Voici les autres pages qui contiennent la partie **États Power BI** étendue et non filtrée :

|ID page|Name|
|-------|----|
|1156|Détail société|
|4013|Informations sur Intelligent Cloud |
|9006|Tableau de bord Préparateur de commandes|
|9008|Feuilles d’inventaire Tableau de bord de base|
|9010|Tableau de bord Gestionnaire de production|
|9015|Tableau de bord Chef de projet|
|9016|Tableau de bord Répartiteur de service|
|9022|Tableau de bord Gestionnaire d′activité|
|9024|Tableau de bord Admin. de sécurité|
|9026|Tableau de bord Responsable Vente et Relations|
|9027|Tableau de bord Comptable|

> [!TIP]
> Nous n′avons pas l′intention de l′ajouter à toutes les pages de liste pour le moment. Cependant, vous pouvez créer une extension de page simple qui ajoute la partie **États Power BI** dans un Récapitulatif. Pour plus d’informations, voir [Ajout des parties États Power BI aux pages](/dynamics365/business-central/dev-itpro/developer/devenv-power-bi-report-parts) dans l′aide dédiée aux développeurs et professionnels de l′informatique.

<!-- 5 -->
### <a name="is-there-any-way-to-filter-a-dataset-from-business-central-before-i-pull-it-into-power-bi-instead-of-applying-filters-afterwards"></a>Existe-t-il un moyen de filtrer un ensemble de données à partir de Business Central *avant* de le basculer dans Power BI au lieu d′appliquer ultérieurement des filtres ?

Pour filtrer des ensembles de données plus volumineux, le moyen le plus simple consiste à définir un filtre sur l′état Power BI en modifiant directement la formule Power Query. La plupart des filtres que vous définissez de cette manière sont transmis à Business Central par Query Folding. Voir [Actualisation incrémentielle des ensembles de données](/power-bi/admin/service-premium-incremental-refresh).

Il n′existe actuellement aucun moyen de définir un filtre pour les données d′un service Web à partir de Business Central. Si votre application doit définir un filtre à partir de Business Central, vous devez créer une application Business Central personnalisée à cet effet.

<!-- 8 and 9 -->

### <a name="for-embedding-reports-in-business-central-pages-right-now-its-only-possible-to-get-reports-from-my-workspace-in-power-bi-are-there-plans-to-make-it-possible-to-get-them-from-custom-workspaces"></a>Pour intégrer des états dans les pages Business Central, il n′est actuellement possible d′obtenir des rapports que depuis *Mon espace de travail* dans Power BI. Est-il prévu de les obtenir à partir d′espaces de travail personnalisés ?

Oui. Nous prévoyons d′ajouter la prise en charge des espaces de travail partagés, mais nous n′avons pas encore de calendrier à vous donner.  

<!-- 10 -->
### <a name="from-power-bi-besides-using-a-query-is-there-another-way-to-get-data-from-business-central-tables-that-dont-have-an-associated-page-for-example-like-the-item-attributes-value-mapping-table"></a>Dans Power BI, outre l′utilisation d′une requête, existe-t-il un autre moyen d′obtenir des données à partir des tables Business Central sans page associée ? Comme la table *Correspondance de valeur d′attribut article*.

Non. Pas à ce stade.

<!-- 12 --> 
### <a name="are-published-queries-faster-to-use-than-published-pages"></a>Les requêtes publiées sont-elles plus rapides à utiliser que les pages publiées ?

En ce qui concerne les services Web, les requêtes publiées sont généralement plus rapides que les pages publiées équivalentes. La raison en est que les requêtes sont optimisées pour la lecture des données et ne contiennent pas de déclencheurs coûteux comme OnAfterGetRecord.

Dès que le nouveau connecteur sera disponible en juin 2021, nous vous encourageons à utiliser les pages API plutôt que les requêtes publiées en tant que services Web.

<!-- 13 --> 
### <a name="is-there-a-way-for-an-end-user-to-create-a-web-service-with-a-column-thats-in-a-business-central-table-but-not-a-page-or-will-developer-have-to-create-a-custom-query"></a>Existe-t-il un moyen pour un utilisateur final de créer un service Web avec une colonne qui se trouve dans une table Business Central, mais pas dans une page ? Ou le développeur doit-il créer une requête personnalisée ? 

Pas encore. Mais dès que le nouveau connecteur sera disponible en juin 2021, un développeur pourra créer une nouvelle page API pour répondre à cette exigence. 

<!-- 28 --> 
### <a name="can-i-connect-power-bi-to-a-read-only-database-server-of-business-central-online"></a>Puis-je connecter Power BI à un serveur de base de données en lecture seule de Business Central Online ? 

Non. Mais nous avons cette fonctionnalité sur notre feuille de route à long terme. 

## <a name="performance"></a>[Performances](#tab/performance)

<!-- 17 -->

### <a name="is-it-faster-to-get-data-using-api-pages-than-using-web-services"></a>Est-il plus rapide d′obtenir des données à l′aide des pages API que par les services Web ?

Oui. Nos tests indiquent que les pages API sont jusqu′à 25 % plus performantes que les services Web.

<!-- 18 -->
### <a name="are-there-plans-to-have-a-mirror-on-the-azure-sql-database-instance-which-i-can-connect-to-directly"></a>Est-il prévu d′avoir un miroir sur l′instance Azure SQL Database pour me connecter directement ?

Non. Pas à ce stade. Vous ne pouvez communiquer qu′avec Business Central par les API.

<!-- 19 -->
### <a name="loading-data-from-business-central-web-services-seems-slow-is-there-any-way-to-get-data-directly-from-the-sql-database-table"></a>Le chargement des données à partir des services Web de Business Central semble lent. Existe-t-il un moyen d′obtenir les données directement à partir de la table de base de données SQL ?

Non. L′accès direct à la base de données n′est pas possible, mais le basculement vers les pages API (dès la mise à disposition du nouveau connecteur) aidera grandement.

## <a name="advanced"></a>[Avancé](#tab/advanced)
<!-- 1 -->

### <a name="are-there-plans-for-the-power-bi-connector-to-support-the-incremental-refresh-features-in-the-power-bi-service"></a>Est-il prévu que le connecteur Power BI prenne en charge les fonctionnalités d′actualisation incrémentielle dans le service Power BI ?

Oui. C′est sur notre feuille de route.

<!-- 2 -->
### <a name="if-a-business-central-on-premises-solution-doesnt-have-internet-access-can-i-still-use-power-bi"></a>Si une solution Business Central sur site n′a pas accès à Internet, puis-je continuer à utiliser Power BI ?
<!-- todo: please explain this one-->

Oui. Dans ce cas, utilisez Power BI Desktop localement et connectez-vous à Business Central sur site. Une fois connecté, vous pouvez créer et afficher des états mais vous ne pouvez tout simplement pas les publier sur le service Power BI. 
<!-- 20 -->
### <a name="are-there-any-plans-to-make-it-possible-to-replicate-business-central-online-databases-so-theyre-accessible-for-read-only-sql-queries-this-capability-would-support-incremental-refresh-and-be-a-lot-faster-than-apis-or-web-services"></a>Est-il prévu de rendre possible la réplication des bases de données Business Central Online afin qu′elles soient accessibles pour les requêtes SQL en lecture seule ? Cette fonction prendrait en charge l′actualisation incrémentielle et serait beaucoup plus rapide que les API ou les services Web.

<!-- todo: what does "BC-Saas-DB-replicated DB accessible" mean? fixe-->
Oui. Nous avons cette fonctionnalité sur notre feuille de route à long terme. 

<!-- 21 -->
### <a name="if-i-use-azure-data-factory-to-get-data-from-business-central-and-consume-it-on-power-bi-will-that-help-in-increase-in-performance"></a>Si j′utilise Azure Data Factory pour obtenir les données depuis Business Central et les consommer sur Power BI, cela aidera-t-il à augmenter les performances ? 

Oui. Ce scénario avancé aiderait Business Central à rester performant car l′accès aux données se ferait via Azure Data Factory.

<!-- 22 -->
### <a name="are-there-any-plans-to-support-power-bi-deployment-pipelines-or-a-way-to-build-deployment-pipelines-for-pbi-reports-similar-to-extensions-or-maybe-even-a-simple-api-in-the-business-admin-center"></a>Est-il prévu de prendre en charge les pipelines de déploiement de Power BI, ou un moyen de créer des pipelines de déploiement pour les états PBI, similaires aux extensions ? Ou peut-être même une API simple dans le Centre d′administration ? 

Nous étudions cette fonctionnalité. Power BI propose des API riches pour contrôler les déploiements d′états. Pour plus d′informations, voir [Introduction aux pipelines de déploiement](/power-bi/create-reports/deployment-pipelines-overview).

### <a name="ive-tried-the-preview-of-the-new-connector-which-will-be-live-in-june-2021-i-see-some-values-like-_x0020_-when-connecting-to-api-v20-what-are-these-values"></a>J′ai essayé la version préliminaire du nouveau connecteur qui sera disponible en juin 2021. Je vois des valeurs comme « _x0020_ » lors de la connexion à API v2.0. Quelles sont ces valeurs ?

La prochaine version du connecteur Power BI permet de se connecter aux pages de l′API de Business Central, ce qui inclut API v2.0. Ces pages incluent des champs basés sur les [objets AL Enum](/dynamics365/business-central/dev-itpro/developer/devenv-extensible-enums). Les champs basés sur les objets AL Enum doivent avoir des noms cohérents et toujours identiques afin que les filtres de l′état fonctionnent toujours&mdash;quels que soient la langue ou le système d′exploitation utilisés. Pour cette raison, les champs basés sur AL Enum ne sont pas traduits et sont codés pour éviter tout caractère spécial dont l′espace. En particulier, chaque fois qu′il y a une option vide dans l′objet AL Enum, elle est codée en « _x0020_ ». Vous pouvez toujours appliquer une transformation à vos données sur Power BI pour afficher une valeur différente pour ces champs, par exemple « Vide ».


---

## <a name="see-also"></a>Voir aussi

[Licence Power BI](admin-powerbi-setup.md#license)
[Introduction à Business Central et à Power BI](admin-powerbi.md)  
[Vue d’ensemble de l’intégration Power BI](admin-powerbi-overview.md)  
[Activation de Power BI dans Business Central](admin-powerbi-setup.md)  
[Utiliser les états Power BI dans Business Central](across-working-with-powerbi.md)  
[Utilisation des données Business Central dans Power BI](across-working-with-business-central-in-powerbi.md)  
[Création d′états Power BI pour afficher les données Business Central](across-how-use-financials-data-source-powerbi.md)    
[Documentation Power BI](/power-bi/)  


[!INCLUDE[footer-include](includes/footer-banner.md)]