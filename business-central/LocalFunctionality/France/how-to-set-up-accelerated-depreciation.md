---
title: Procédure de paramétrage de l'amortissement accéléré
description: Pour utiliser la fonction de calcul de l'amortissement accéléré, vous devez configurer les lois d'amortissement pour les immobilisations.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 21c83ca14e498b4866939923044583a1e129f7c2
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5774377"
---
# <a name="set-up-accelerated-depreciation"></a>Paramétrer l'amortissement accéléré
Pour utiliser la fonction de calcul de l'amortissement accéléré, vous devez configurer les lois d'amortissement suivantes pour les immobilisations :  

- la loi d'amortissement comptable (intégrée à la comptabilité) ;  
- la loi d'amortissement fiscal (non intégrée à la comptabilité).  

> [!NOTE]  
>  Lorsque vous validez une acquisition, un amortissement ou une cession pour la loi d'amortissement comptable, la transaction est automatiquement dupliquée et validée dans la loi d'amortissement fiscal lorsque la feuille immobilisation est validée.  

## <a name="to-set-up-the-accounting-depreciation-book"></a>Pour configurer la loi d'amortissement comptable  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Lois d'amortissement**, puis choisissez le lien approprié.  
2.  Sur la page **Liste de la loi d'amortissement**, sélectionnez l'action **Nouveau**.  
3.  Sous le raccourci **Général**, renseignez les champs obligatoires comme indiqué dans le tableau ci-dessous.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Code d'identification unique de la loi d'amortissement comptable. Vous pouvez entrer 10 caractères alphanumériques maximum.|  
    |**Description**|Description des lois d'amortissement.|  

    > [!IMPORTANT]  
    >  Laissez le champ **Calcul dérogatoire** vide.  

4.  Dans le raccourci **Intégration**, sélectionnez la case à cocher **Dérogatoire** pour intégrer l'amortissement accéléré dans la comptabilité.  

    Pour en savoir plus, voir [Configurer l'amortissement d'immobilisation](../../fa-how-setup-depreciation.md).  

5.  Cliquez sur le bouton **OK**.  

## <a name="to-set-up-the-tax-depreciation-book"></a>Pour configurer la loi d'amortissement fiscal  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Lois d'amortissement**, puis choisissez le lien approprié.  
2.  Sur la page **Liste de la loi d'amortissement**, sélectionnez l'action **Nouveau**.  
3.  Sous le raccourci **Général**, renseignez les champs obligatoires comme indiqué dans le tableau ci-dessous.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Code d'identification unique de la loi d'amortissement fiscal. Vous pouvez entrer 10 caractères alphanumériques maximum.|  
    |**Description**|Description des lois d'amortissement fiscal.|  

4.  Dans le champ **Calcul dérogatoire**, sélectionnez une loi d'amortissement comptable pour indiquer qu'il s'agit d'une loi d'amortissement fiscal pour le calcul de l'amortissement dérogatoire.  

    Pour en savoir plus, voir [Configurer l'amortissement d'immobilisation](../../fa-how-setup-depreciation.md).  

5.  Cliquez sur le bouton **OK**.  

Le champ **Utilisé avec la loi dérogatoire** dans la loi d'amortissement comptable est mis à jour avec le code de la loi d'amortissement fiscal.  

## <a name="see-also"></a>Voir aussi  
 [Amortissement accéléré](accelerated-depreciation.md)   
 [Calculer l'amortissement accéléré](how-to-calculate-accelerated-depreciation.md)   
[Configurer un amortissement immobilisation](../../fa-how-setup-depreciation.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]