---
title: Configuration des relations d&quot;affaires pour des contacts | Microsoft Docs
description: "Décrit les relations d&quot;affaires pour les contacts dans Financials"
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, prospect, contact, client, customer
ms.date: 03/28/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: f6719ac45f298d6c952427c871eaf818cb7480c3
ms.contentlocale: fr-fr
ms.lasthandoff: 05/04/2017


---
# <a name="setting-up-business-relations-on-contact-companies"></a>Configuration des relations d'affaires sur des sociétés contact
Les relations d'affaires vous permettent d'indiquer les rapports établis avec vos contacts, tels que les prospects, les banques, les consultants, les prestataires de services, et ainsi de suite.

L'utilisation des relations d'affaires sur les contacts processus en deux étapes. Tout d'abord, vous définissez le code relation d'affaires. Vous ne devez effectuer cette étape qu'une seule fois pour chaque relation d'affaires. Une fois que vous disposez d'un code relation d'affaires, vous pouvez commencer à affecter le code aux sociétés contact.

**Remarque** : si vous prévoyez de synchroniser vos contacts avec des fournisseurs, des clients ou des comptes bancaires dans d'autres parties de l'application, vous pouvez configurer pour eux une relation d'affaires.

## <a name="to-define-a-business-relation-code"></a>Pour définir un code relation d'affaires
Le code relation d'affaires définit une catégorie ou un type de relation d'affaires, telles que BANQUE ou Avocat. Vous pouvez disposer de plusieurs codes relation d'affaires. Pour définir la relation d'affaires, vous utilisez la fenêtre **Relations d'affaires**.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche** ![Page ou état pour la recherche](media/ui-search/search_small.png "Icône Page ou état pour la recherche"), entrez **Relations d'affaires**, puis sélectionnez le lien associé.
2. Sélectionnez l'action **Nouveau**, et entrez un code et une désignation. Vous pouvez saisir pour le code un maximum de 11 caractères, et toute combinaison de chiffres et des lettres.

## <a name="AssignBusRelContact"></a> Pour affecter des relations d'affaires à un contact
Vous ne pouvez pas affecter de relations d'affaires à un individu, mais uniquement à des sociétés.

1. Ouvrez le contact.
2. Sélectionnez l'action **Société**, puis l'action **Relations d'affaires**.

    La fenêtre **Relations d'affaires contact** s'ouvre.
3. Dans le champ **Code relation d'affaires**, sélectionnez la relation d'affaires à affecter.

Répétez ces étapes pour chaque relation d'affaires à affecter. Vous pouvez également affecter des relations d'affaires à partir de la liste des contacts en suivant la même procédure.

Le nombre de relations d'affaires que vous avez affectées au contact s'affiche dans le champ **Nbre relations d'affaires** de la section **Segmentation** de la fenêtre **Contact**.

Une fois que vous avez affecté des relations d'affaires à vos contacts, vous pouvez utiliser ces informations pour sélectionner des contacts pour vos segments. Pour plus d'informations, reportez-vous à [Procédure : ajouter des contacts à des segments](marketing-add-contact-segment.md).

## <a name="see-also"></a>Voir aussi
[Création de sociétés contact](marketing-create-contact-companies.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
