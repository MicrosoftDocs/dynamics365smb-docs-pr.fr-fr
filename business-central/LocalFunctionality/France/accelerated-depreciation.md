---
title: Amortissement accéléré
description: L'amortissement accéléré est calculé sur la base des différences entre la loi d'amortissement comptable et la loi d'amortissement fiscal, sur toute la durée de vie de l'immobilisation.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 269c8e12cb5a9d2f5f255f2b0cf9c6a5536a90bf
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/01/2020
ms.locfileid: "3181211"
---
# <a name="accelerated-depreciation"></a>Amortissement accéléré
L'amortissement accéléré est calculé sur la base des différences entre la loi d'amortissement comptable et la loi d'amortissement fiscal, sur toute la durée de vie de l'immobilisation.  

Les immobilisations qui ont un amortissement fiscal plus élevé et un amortissement comptable plus faible sont amorties à l'aide de la méthode d'amortissement accéléré, comme l'autorisent les administrations fiscales.  

Les sociétés doivent utiliser la méthode d'amortissement accéléré pour valider les montants de taxe supplémentaires si elles remplissent au moins deux des critères suivants :  

- Elles ont plus de 50 salariés.  
- Elles ont au moins deux millions d'euros d'actifs.  
- Elles ont au moins quatre millions d'euros de chiffre d'affaires.  

## <a name="depreciation-book"></a>Loi d'amortissement  
La méthode d'amortissement accéléré vous permet de calculer et de valider les différences entre les montants d'amortissement fiscal et les montants d'amortissement comptable autorisés pour les immobilisations. Pour calculer l'amortissement accéléré pour les immobilisations, les lois d'amortissement suivantes doivent être configurées :  

- la loi d'amortissement comptable (intégrée à la comptabilité) ;  
- la loi d'amortissement fiscal (non intégrée à la comptabilité).  

Vous devez configurer la loi d'amortissement fiscal en tant que loi dérogatoire à l'aide d'un paramètre d'amortissement accéléré. Si ce paramètre est défini, les différences entre la loi d'amortissement fiscal et la loi d'amortissement comptable sont calculées et validées en tant que montants d'amortissement accéléré. Pour en savoir plus, voir [Paramétrer l'amortissement accéléré](how-to-set-up-accelerated-depreciation.md).  

### <a name="example"></a>Exemple :  
 Si vous avez une immobilisation d'une valeur de 1 000 euros qui est amortie dans la loi d'amortissement comptable sur cinq ans, et amortie dans la loi d'amortissement fiscal sur trois ans, l'amortissement comptable pour la première année est de 200 euros (1 000/5) et l'amortissement fiscal pour la première année est de 333,33 euros (1 000/3). Le montant d'amortissement accéléré est la différence entre ces deux montants : 133,33 euros (333,33 - 200).  

## <a name="accelerated-depreciation-accounts"></a>Montants d'amortissement accéléré  
L'amortissement accéléré utilise le type de comptabilisation immobilisation dérogatoire. Les statistiques et les états utilisent ce type de comptabilisation pour déclarer le calcul de l'amortissement accéléré. Pour en savoir plus, voir [Configurer l'amortissement d'immobilisation](../../fa-how-setup-depreciation.md).  

Deux comptes doivent être configurés pour les montants dérogatoires :  

- Montants d'amortissement accéléré positifs (augmentation de l'amortissement accéléré) :  

    - Compte dérogatoire  
    - Compte frais dérogatoire  
    - Montants d'amortissement accéléré négatifs (réduction de l'amortissement accéléré) :  
    - Compte dérogatoire sur cession  
    - Compte de contrepartie dérogatoire sur cession  

Si vous validez une acquisition, un amortissement ou une cession pour la loi d'amortissement comptable, la transaction est automatiquement dupliquée et validée dans la loi d'amortissement fiscal lorsque la feuille est validée.  

Après avoir configuré la loi d'amortissement fiscal et la loi d'amortissement comptable, l'amortissement accéléré est calculé automatiquement pour les immobilisations à l'aide du traitement par lots Calculer amortissement dans la loi d'amortissement comptable. Pour en savoir plus, voir [Calculer l'amortissement accéléré](how-to-calculate-accelerated-depreciation.md).  

## <a name="see-also"></a>Voir aussi  
 [Paramétrer l'amortissement accéléré](how-to-set-up-accelerated-depreciation.md)   
 [Calculer l'amortissement accéléré](how-to-calculate-accelerated-depreciation.md)   
 [Configurer un amortissement immobilisation](../../fa-how-setup-depreciation.md)   
[COMPTES D'IMMOBILISATIONS](../../fa-manage.md)  
 [Fonctionnalité locale, France](france-local-functionality.md)
