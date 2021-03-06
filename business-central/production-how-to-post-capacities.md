---
title: Procédure de validation des capacités | Microsoft Docs
description: La feuille capacité vous permet de valider les capacités consommées qui ne sont pas affectées à l’ordre de fabrication. Par exemple, les travaux de maintenance doivent être affectés à une capacité, mais non à un ordre de fabrication.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 8f41a5033c79ec500a635d27f8296d01d895ed27
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5787926"
---
# <a name="post-capacities"></a>Valider les capacités
La feuille capacité vous permet de valider les capacités consommées qui ne sont pas affectées à l’ordre de fabrication. Par exemple, les travaux de maintenance doivent être affectés à une capacité, mais non à un ordre de fabrication.  

## <a name="to-post-capacities"></a>Pour valider les capacités  
1.  Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Feuilles capacité**, puis sélectionnez le lien associé.  
2.  Renseignez les champs **Date comptabilisation** et **N° document**.  
3.  Dans le champ **Type**, entrez le type de capacité, **Poste de charge** ou **Centre de charge**, que vous validez.  
4.  Dans le champ **N°**, saisissez le nom du centre de charge ou du poste de charge.  
5.  Entrez les données nécessaires dans les autres champs, tels que **Heure début**, **Heure fin**, **Quantité**, et **Rebut**.  
6.  Choisissez l’action **Valider** pour valider les capacités.  

## <a name="to-view-work-center-ledger-entries"></a>Pour afficher les écritures comptables centre de charge  
Sur les pages **Fiche centre de charge** et **Fiche poste de charge**, vous pouvez afficher les capacités validées en tant que résultat des ordres de fabrication terminés.    
1.  Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Centres de charge**, puis sélectionnez le lien associé.  
2.  Ouvrez la fiche **Centre de charge** appropriée dans la liste, puis choisissez l’action **Écritures comptables capacité**.  

La page **Écritures comptables capacité** affiche les écritures validées relatives au centre de charge dans l’ordre de leur validation.   

## <a name="see-also"></a>Voir aussi  
[Production](production-manage-manufacturing.md)    
[Paramétrage de la production](production-configure-production-processes.md)  
[Planifié](production-planning.md)      
[Stock](inventory-manage-inventory.md)  
[Achats](purchasing-manage-purchasing.md)  
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]