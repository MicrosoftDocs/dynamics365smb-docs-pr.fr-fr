---
title: Procédure d'archivage des bordereaux paiement
description: Lorsqu'un bordereau paiement a été entièrement traité, vous pouvez le séparer des bordereaux paiement actifs en l'archivant.
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
ms.openlocfilehash: edbe0eb00dc69c0a7d2d22f0a10c43e604b33802
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5776580"
---
# <a name="archive-payment-slips"></a>Archiver les bordereaux de paiement
Lorsqu'un bordereau paiement a été entièrement traité, vous pouvez le séparer des bordereaux paiement actifs en l'archivant.  

Vous pouvez archiver le bordereau paiement à l'aide des méthodes suivantes :  

- Manuellement pour des bordereaux paiement individuels.  
- Automatiquement pour un lot de bordereaux paiement.  

## <a name="to-archive-a-payment-slip"></a>Pour archiver un bordereau paiement  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Bordereaux de paiement**, puis choisissez le lien approprié.  
2.  Sélectionnez le bordereau paiement concerné, puis cliquez sur l'action **Modifier**.  
3.  Sur la page **Bordereau paiement**, sélectionnez **Archiver**.  
4.  Cliquez sur le bouton **Oui** pour archiver le bordereau paiement.  

    > [!NOTE]  
    >  Si le statut actuel du bordereau paiement n'autorise pas l'archivage, un message s'affiche.  

## <a name="to-archive-a-batch-of-payment-slips"></a>Pour archiver un lot de bordereaux paiement  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Archiver les bordereaux de paiement**, puis choisissez le lien approprié.  
2.  Sur la page **Archiver les bordereaux de paiement**, sur le raccourci **En-tête bordereau**, sélectionnez les filtres appropriés.  
3.  Cliquez sur le bouton **OK**.  

Les bordereaux paiement sont archivés.  

> [!NOTE]  
>  Ce traitement par lots archive uniquement les bordereaux paiement dont la case **Archivage autorisé** est cochée sur la page **Statut règlement**. Pour plus d'informations, voir [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md).  

## <a name="see-also"></a>Voir aussi  
 [Gestion des paiements](payment-management.md)   
 [Paramétrer des types de règlement](how-to-set-up-payment-classes.md)   
 [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md)   
 [Paramétrer des étapes règlement](how-to-set-up-payment-steps.md)   
 [Configurer des adresses de paiement](how-to-set-up-payment-addresses.md)   
 [Créer bordereaux paiement](how-to-create-payment-slips.md)   
 [Valider des bordereaux paiement](how-to-post-payment-slips.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]