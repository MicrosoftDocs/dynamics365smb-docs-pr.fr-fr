---
title: "Procédure de définition des périodes de validation"
description: "En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 25552d10a453541863719e6b03710e618bbd9827
ms.contentlocale: fr-fr
ms.lasthandoff: 03/22/2018

---
# <a name="specify-posting-periods"></a>Définir des périodes de validation
En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée.  

## <a name="to-specify-posting-periods"></a>Pour définir des périodes de validation  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres comptabilité**, puis sélectionnez le lien connexe.  
2.  Dans la fenêtre **Paramètres comptabilité**, sous l'onglet **Général**, dans le champ **Début période validation**, spécifiez la date de début de la période de validation.  
3.  Dans le champ **Fin période validation**, spécifiez la date de fin de la période de validation.  

    Les dates sont validées dans les plages de validation autorisées pour garantir leur appartenance aux exercices comptables ouverts. Pour plus d'informations, voir Plage de validation autorisée.  

4.  Pour vérifier quelle est la plage de validation autorisée, choisissez l'action **Extraire plage de validation autorisée**.  

Les dates définies ici s'appliquent à l'ensemble de la société, c'est-à-dire à tous les utilisateurs.  

> [!NOTE]  
>  Vous pouvez définir différentes périodes de comptabilisation pour divers utilisateurs et appliquer une période de validation à un utilisateur dans la fenêtre **Paramètres utilisateur**.

Si vous entrez des dates ici, les dates entrées sous l'onglet **Général** de la fenêtre **Paramètres comptabilité** ne s'appliquent pas à ces utilisateurs.  

## <a name="see-also"></a>Voir aussi  
 [Périodes fiscales et exercices comptables](fiscal-periods-and-fiscal-years.md)

