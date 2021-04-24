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
# <a name="archive-payment-slips"></a><span data-ttu-id="84af9-103">Archiver les bordereaux de paiement</span><span class="sxs-lookup"><span data-stu-id="84af9-103">Archive Payment Slips</span></span>
<span data-ttu-id="84af9-104">Lorsqu'un bordereau paiement a été entièrement traité, vous pouvez le séparer des bordereaux paiement actifs en l'archivant.</span><span class="sxs-lookup"><span data-stu-id="84af9-104">When a payment slip has been processed, you can separate it from the active payment slips by archiving it.</span></span>  

<span data-ttu-id="84af9-105">Vous pouvez archiver le bordereau paiement à l'aide des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="84af9-105">You can archive the payment slip by using the following methods:</span></span>  

- <span data-ttu-id="84af9-106">Manuellement pour des bordereaux paiement individuels.</span><span class="sxs-lookup"><span data-stu-id="84af9-106">Manually – for individual payment slips.</span></span>  
- <span data-ttu-id="84af9-107">Automatiquement pour un lot de bordereaux paiement.</span><span class="sxs-lookup"><span data-stu-id="84af9-107">Automatically – for a batch of payment slips.</span></span>  

## <a name="to-archive-a-payment-slip"></a><span data-ttu-id="84af9-108">Pour archiver un bordereau paiement</span><span class="sxs-lookup"><span data-stu-id="84af9-108">To archive a payment slip</span></span>  

1.  <span data-ttu-id="84af9-109">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Bordereaux de paiement**, puis choisissez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="84af9-109">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Slips**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="84af9-110">Sélectionnez le bordereau paiement concerné, puis cliquez sur l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="84af9-110">Select the relevant payment slip, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="84af9-111">Sur la page **Bordereau paiement**, sélectionnez **Archiver**.</span><span class="sxs-lookup"><span data-stu-id="84af9-111">On the **Payment Slip** page, choose the **Archive** action.</span></span>  
4.  <span data-ttu-id="84af9-112">Cliquez sur le bouton **Oui** pour archiver le bordereau paiement.</span><span class="sxs-lookup"><span data-stu-id="84af9-112">Choose the **Yes** button to archive the payment slip.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="84af9-113">Si le statut actuel du bordereau paiement n'autorise pas l'archivage, un message s'affiche.</span><span class="sxs-lookup"><span data-stu-id="84af9-113">If the current status of the payment slip does not allow archiving, a message is displayed.</span></span>  

## <a name="to-archive-a-batch-of-payment-slips"></a><span data-ttu-id="84af9-114">Pour archiver un lot de bordereaux paiement</span><span class="sxs-lookup"><span data-stu-id="84af9-114">To archive a batch of payment slips</span></span>  

1.  <span data-ttu-id="84af9-115">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Archiver les bordereaux de paiement**, puis choisissez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="84af9-115">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archive Payment Slips**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="84af9-116">Sur la page **Archiver les bordereaux de paiement**, sur le raccourci **En-tête bordereau**, sélectionnez les filtres appropriés.</span><span class="sxs-lookup"><span data-stu-id="84af9-116">On the **Archive Payment Slips** page, on the **Payment Header** FastTab, select the appropriate filters.</span></span>  
3.  <span data-ttu-id="84af9-117">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="84af9-117">Choose the **OK** button.</span></span>  

<span data-ttu-id="84af9-118">Les bordereaux paiement sont archivés.</span><span class="sxs-lookup"><span data-stu-id="84af9-118">The payment slips are archived.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="84af9-119">Ce traitement par lots archive uniquement les bordereaux paiement dont la case **Archivage autorisé** est cochée sur la page **Statut règlement**.</span><span class="sxs-lookup"><span data-stu-id="84af9-119">This batch job will only archive payment slips that have the **Archiving Authorized** check box selected on the **Payment Status** page.</span></span> <span data-ttu-id="84af9-120">Pour plus d'informations, voir [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md).</span><span class="sxs-lookup"><span data-stu-id="84af9-120">For more information, see [Set Up Payment Statuses](how-to-set-up-payment-statuses.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="84af9-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="84af9-121">See Also</span></span>  
 <span data-ttu-id="84af9-122">[Gestion des paiements](payment-management.md) </span><span class="sxs-lookup"><span data-stu-id="84af9-122">[Payment Management](payment-management.md) </span></span>  
 <span data-ttu-id="84af9-123">[Paramétrer des types de règlement](how-to-set-up-payment-classes.md) </span><span class="sxs-lookup"><span data-stu-id="84af9-123">[Set Up Payment Classes](how-to-set-up-payment-classes.md) </span></span>  
 <span data-ttu-id="84af9-124">[Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md) </span><span class="sxs-lookup"><span data-stu-id="84af9-124">[Set Up Payment Statuses](how-to-set-up-payment-statuses.md) </span></span>  
 <span data-ttu-id="84af9-125">[Paramétrer des étapes règlement](how-to-set-up-payment-steps.md) </span><span class="sxs-lookup"><span data-stu-id="84af9-125">[Set Up Payment Steps](how-to-set-up-payment-steps.md) </span></span>  
 <span data-ttu-id="84af9-126">[Configurer des adresses de paiement](how-to-set-up-payment-addresses.md) </span><span class="sxs-lookup"><span data-stu-id="84af9-126">[Set Up Payment Addresses](how-to-set-up-payment-addresses.md) </span></span>  
 <span data-ttu-id="84af9-127">[Créer bordereaux paiement](how-to-create-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="84af9-127">[Create Payment Slips](how-to-create-payment-slips.md) </span></span>  
 [<span data-ttu-id="84af9-128">Valider des bordereaux paiement</span><span class="sxs-lookup"><span data-stu-id="84af9-128">Post Payment Slips</span></span>](how-to-post-payment-slips.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]