---
title: Analyse des données de rapport avec Excel
description: Découvrez comment utiliser Excel pour analyser un jeu de données de rapport.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process, report, print, schedule, save, Excel, PDF, Word, dataset
ms.date: 02/09/2022
ms.author: jswymer
ms.openlocfilehash: 60b28db92c6788b67aa1c290df800551515f1be7
ms.sourcegitcommit: 2c972dfc94d27245eaa99efcf638d030dedafb22
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/09/2022
ms.locfileid: "8104181"
---
# <a name="analyzing-report-data-with-excel"></a>Analyse des données de rapport avec Excel

[!INCLUDE[2021_releasewave2](includes/2021_releasewave2.md)]

En tant que développeur ou utilisateur avancé, il est utile d’inspecter les données générées pour un jeu de données de rapport donné lorsque vous créez des rapports ou modifiez des rapports existants. Pour prendre en charge cette fonctionnalité, vous pouvez exporter un jeu de données de rapport sous forme de données brutes vers une feuille de calcul Excel, directement à partir de la page de demande de rapport dans le client. Dans Excel, vous pouvez ensuite effectuer une analyse ad hoc des données et diagnostiquer les problèmes.

## <a name="get-started"></a>Démarrer

Pour exporter un jeu de données de rapport, ouvrez le rapport dans le client, puis sur la page de demande, sélectionnez **Envoyer à** > **Document Microsoft Excel (données uniquement)**. 

L’option **Document Microsoft Excel (données uniquement)** exporte les résultats du rapport et les critères qui ont été utilisés pour les générer, mais il n’inclut pas la mise en page du rapport. Le fichier Excel comprendra l’ensemble de données complet, sous forme de données brutes, disposées en lignes et en colonnes. Toutes les colonnes de données de l’ensemble de données du rapport sont incluses, qu’elles soient ou non utilisées dans la présentation du rapport.

Une fois que vous avez le fichier Excel, vous pouvez commencer à analyser les données. Par exemple, vous pourriez filtrer les données et utiliser Power Pivot pour les afficher.

Chaque fois que vous exportez des résultats, une feuille de calcul est créée. En utilisant l’option **Document Microsoft Excel (données uniquement)**, vous pouvez exécuter le même rapport et réutiliser les modifications apportées à la mise en forme. Par exemple, pour Power Pivot, vous pouvez réexécuter le rapport pour une autre période, copier les résultats dans la feuille de calcul, puis actualiser la feuille de calcul. Vous pouvez trouver une application de création de rapports sur [AppSource](https://appsource.microsoft.com/).

> [!NOTE]
> Vous ne pouvez pas exporter un rapport contenant plus de 1 048 576 lignes ou 16 384 colonnes. Avec Business Central sur site, le nombre maximal de lignes exportées peut être encore inférieur. Business Central Server inclut un paramètre de configuration, appelé **Nombre maximal de lignes de données autorisées à envoyer vers Excel**, pour diminuer la limite à partir de la valeur maximale. Pour plus d’informations, consultez [Configuration de Business Central Server](/dynamics365/business-central/dev-itpro/administration/configure-server-instance#General) ou contactez votre administrateur.

## <a name="for-administrators"></a>Pour les administrateurs

- **Microsoft Excel Document (données uniquement)** a été introduite en tant que fonctionnalité facultative dans la première vague de version 2021, mise à jour 18.3. Pour permettre aux utilisateurs d’accéder à cette fonction pendant l’exécution de la 1re vague de lancement 2021, activez la mise à jour de la fonction **Enregistrer l’ensemble de données du rapport dans le document Microsoft Excel** dans **Gestion des fonctionnalités**. Pour plus d’informations, consultez [Activer les fonctionnalités à venir à l’avance](/dynamics365/business-central/dev-itpro/administration/feature-management). Dans la 2e vague de lancement 2021, cette fonctionnalité est devenue permanente, vous n’aurez donc pas à l’activer.

- Pour utiliser **Document Microsoft Excel(données uniquement)**, les comptes d’utilisateurs ont besoin de l’autorisation **Autoriser l’action Exporter le jeu de données du rapport vers Excel**. Vous pouvez accorder cette autorisation aux utilisateurs en attribuant soit l’ensemble d’autorisations **Outils de dépannage** ou **Exporter le rapport Excel**. Pour plus d’informations, voir [Attribuer des autorisations aux utilisateurs et aux groupes](ui-define-granular-permissions.md).  

## <a name="for-developers-and-advanced-users"></a>Pour les développeurs et les utilisateurs avancés

L’option **Microsoft Excel Document (données uniquement)** exporte toutes les colonnes, y compris les colonnes contenant des filtres et des instructions de formatage pour d’autres valeurs. Voici quelques points d’intérêt :

- Les données binaires d’un champ, comme une image, ne sont pas exportées.

  Dans les colonnes contenant des données binaires, les champs incluront le texte **Données binaires ({0} octets)**, où **{0}** indique le nombre d’octets.
- À partir de la deuxième vague de la version 2 de Business Central 2021, le fichier Excel comprend également la feuille de calcul **Métadonnées de l’état**.

  Cette feuille de calcul montre les filtres appliqués à l’état et les propriétés générales de l’état, comme le nom, l’ID et les détails de l’extension. Les filtres sont affichés dans la colonne **Filtre (DataItem::Table::FilterGroupNo::FieldName)**. Les filtres de cette colonne incluent des filtres définis sur la page de demande de l’état. Elle comprend également des filtres définis dans le code AL, par exemple, par la [propriété DataItemLink](/dynamics365/business-central/dev-itpro/developer/properties/devenv-dataitemlink-reports-property) et la [propriété DataItemTableView](/dynamics365/business-central/dev-itpro/developer/properties/devenv-dataitemtableview-property).

Pour plus d’informations sur la conception d’états, voir [Aperçu de l’état](/dynamics365/business-central/dev-itpro/developer/devenv-reports).

## <a name="see-also"></a>Voir aussi

[Utilisation des états](ui-work-report.md)  
[Gestion des présentations d’état et de document](ui-manage-report-layouts.md)  
[Attribuer des autorisations aux utilisateurs et aux groupes](ui-define-granular-permissions.md)  
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]