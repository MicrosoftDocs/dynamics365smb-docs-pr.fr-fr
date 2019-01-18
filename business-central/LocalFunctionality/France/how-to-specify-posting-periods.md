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
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: ff2982d2d5811da8fcd0ddea853789c03d04fba7
ms.contentlocale: fr-fr
ms.lasthandoff: 11/26/2018

---
# <a name="specify-posting-periods"></a>Définir des périodes de validation
En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée.  

## <a name="to-specify-posting-periods"></a>Pour définir des périodes de validation  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres comptabilité**, puis sélectionnez le lien connexe.  
2.  Sur la page **Paramètres comptabilité**, sous l'onglet **Général**, dans le champ **Début période validation**, spécifiez la date de début de la période de validation.  
3.  Dans le champ **Fin période validation**, spécifiez la date de fin de la période de validation.  

    Les dates sont validées dans les plages de validation autorisées pour garantir leur appartenance aux exercices comptables ouverts. Pour plus d'informations, voir Plage de validation autorisée.  

4.  Pour vérifier quelle est la plage de validation autorisée, choisissez l'action **Extraire plage de validation autorisée**.  

Les dates définies ici s'appliquent à l'ensemble de la société, c'est-à-dire à tous les utilisateurs.  

> [!NOTE]  
>  Vous pouvez définir différentes périodes de comptabilisation pour divers utilisateurs et appliquer une période de validation à un utilisateur sur la page **Paramètres utilisateur**.

Si vous entrez des dates ici, les dates entrées sous l'onglet **Général** sur la page **Paramètres comptabilité** ne s'appliquent pas à ces utilisateurs.  

## <a name="see-also"></a>Voir aussi  
 [Périodes fiscales et exercices comptables](fiscal-periods-and-fiscal-years.md)

