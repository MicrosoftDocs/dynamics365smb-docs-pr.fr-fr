---
title: "Procédure d'archivage des bordereaux paiement"
description: "Lorsqu'un bordereau paiement a été entièrement traité, vous pouvez le séparer des bordereaux paiement actifs en l'archivant."
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
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 7bec2b1ab6c277d5004872f7a7802645ced91f2e
ms.contentlocale: fr-fr
ms.lasthandoff: 09/28/2018

---
# <a name="archive-payment-slips"></a><span data-ttu-id="ff3e6-103">Archiver les bordereaux de paiement</span><span class="sxs-lookup"><span data-stu-id="ff3e6-103">Archive Payment Slips</span></span>
<span data-ttu-id="ff3e6-104">Lorsqu'un bordereau paiement a été entièrement traité, vous pouvez le séparer des bordereaux paiement actifs en l'archivant.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-104">When a payment slip has been processed, you can separate it from the active payment slips by archiving it.</span></span>  

<span data-ttu-id="ff3e6-105">Vous pouvez archiver le bordereau paiement à l'aide des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="ff3e6-105">You can archive the payment slip by using the following methods:</span></span>  

- <span data-ttu-id="ff3e6-106">Manuellement pour des bordereaux paiement individuels.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-106">Manually – for individual payment slips.</span></span>  
- <span data-ttu-id="ff3e6-107">Automatiquement pour un lot de bordereaux paiement.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-107">Automatically – for a batch of payment slips.</span></span>  

## <a name="to-archive-a-payment-slip"></a><span data-ttu-id="ff3e6-108">Pour archiver un bordereau paiement</span><span class="sxs-lookup"><span data-stu-id="ff3e6-108">To archive a payment slip</span></span>  

1.  <span data-ttu-id="ff3e6-109">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Bordereaux paiement**, puis sélectionnez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Slips**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="ff3e6-110">Sélectionnez le bordereau paiement concerné, puis cliquez sur l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-110">Select the relevant payment slip, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="ff3e6-111">Dans la fenêtre **Bordereau paiement**, sélectionnez **Archiver**.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-111">In the **Payment Slip** window, choose the **Archive** action.</span></span>  
4.  <span data-ttu-id="ff3e6-112">Cliquez sur le bouton **Oui** pour archiver le bordereau paiement.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-112">Choose the **Yes** button to archive the payment slip.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="ff3e6-113">Si le statut actuel du bordereau paiement n'autorise pas l'archivage, un message s'affiche.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-113">If the current status of the payment slip does not allow archiving, a message is displayed.</span></span>  

## <a name="to-archive-a-batch-of-payment-slips"></a><span data-ttu-id="ff3e6-114">Pour archiver un lot de bordereaux paiement</span><span class="sxs-lookup"><span data-stu-id="ff3e6-114">To archive a batch of payment slips</span></span>  

1.  <span data-ttu-id="ff3e6-115">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Archiver les bordereaux de paiement**, puis sélectionnez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Archive Payment Slips**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="ff3e6-116">Dans la fenêtre **Archiver les bordereaux de paiement**, sur le raccourci **En-tête bordereau**, sélectionnez les filtres appropriés.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-116">In the **Archive Payment Slips** window, on the **Payment Header** FastTab, select the appropriate filters.</span></span>  
3.  <span data-ttu-id="ff3e6-117">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-117">Choose the **OK** button.</span></span>  

<span data-ttu-id="ff3e6-118">Les bordereaux paiement sont archivés.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-118">The payment slips are archived.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="ff3e6-119">Ce traitement par lots archive uniquement les bordereaux paiement dont la case **Archivage autorisé** est cochée dans la fenêtre **Statut règlement**.</span><span class="sxs-lookup"><span data-stu-id="ff3e6-119">This batch job will only archive payment slips that have the **Archiving Authorized** check box selected in the **Payment Status** window.</span></span> <span data-ttu-id="ff3e6-120">Pour plus d'informations, voir [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md).</span><span class="sxs-lookup"><span data-stu-id="ff3e6-120">For more information, see [Set Up Payment Statuses](how-to-set-up-payment-statuses.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="ff3e6-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ff3e6-121">See Also</span></span>  
 <span data-ttu-id="ff3e6-122">[Gestion des paiements](payment-management.md) </span><span class="sxs-lookup"><span data-stu-id="ff3e6-122">[Payment Management](payment-management.md) </span></span>  
 <span data-ttu-id="ff3e6-123">[Paramétrer des types de règlement](how-to-set-up-payment-classes.md) </span><span class="sxs-lookup"><span data-stu-id="ff3e6-123">[Set Up Payment Classes](how-to-set-up-payment-classes.md) </span></span>  
 <span data-ttu-id="ff3e6-124">[Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md) </span><span class="sxs-lookup"><span data-stu-id="ff3e6-124">[Set Up Payment Statuses](how-to-set-up-payment-statuses.md) </span></span>  
 <span data-ttu-id="ff3e6-125">[Paramétrer des étapes règlement](how-to-set-up-payment-steps.md) </span><span class="sxs-lookup"><span data-stu-id="ff3e6-125">[Set Up Payment Steps](how-to-set-up-payment-steps.md) </span></span>  
 <span data-ttu-id="ff3e6-126">[Configurer des adresses de paiement](how-to-set-up-payment-addresses.md) </span><span class="sxs-lookup"><span data-stu-id="ff3e6-126">[Set Up Payment Addresses](how-to-set-up-payment-addresses.md) </span></span>  
 <span data-ttu-id="ff3e6-127">[Créer bordereaux paiement](how-to-create-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="ff3e6-127">[Create Payment Slips](how-to-create-payment-slips.md) </span></span>  
 [<span data-ttu-id="ff3e6-128">Valider des bordereaux paiement</span><span class="sxs-lookup"><span data-stu-id="ff3e6-128">Post Payment Slips</span></span>](how-to-post-payment-slips.md)

