---
title: Procédure d'archivage des bordereaux paiement
description: Lorsqu'un bordereau paiement a été entièrement traité, vous pouvez le séparer des bordereaux paiement actifs en l'archivant.
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
ms.openlocfilehash: 2ebcf5f7999b2a36eb4680c5adf43d855d6003fa
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/01/2020
ms.locfileid: "3181207"
---
# <a name="archive-payment-slips"></a><span data-ttu-id="a25dd-103">Archiver les bordereaux de paiement</span><span class="sxs-lookup"><span data-stu-id="a25dd-103">Archive Payment Slips</span></span>
<span data-ttu-id="a25dd-104">Lorsqu'un bordereau paiement a été entièrement traité, vous pouvez le séparer des bordereaux paiement actifs en l'archivant.</span><span class="sxs-lookup"><span data-stu-id="a25dd-104">When a payment slip has been processed, you can separate it from the active payment slips by archiving it.</span></span>  

<span data-ttu-id="a25dd-105">Vous pouvez archiver le bordereau paiement à l'aide des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a25dd-105">You can archive the payment slip by using the following methods:</span></span>  

- <span data-ttu-id="a25dd-106">Manuellement pour des bordereaux paiement individuels.</span><span class="sxs-lookup"><span data-stu-id="a25dd-106">Manually – for individual payment slips.</span></span>  
- <span data-ttu-id="a25dd-107">Automatiquement pour un lot de bordereaux paiement.</span><span class="sxs-lookup"><span data-stu-id="a25dd-107">Automatically – for a batch of payment slips.</span></span>  

## <a name="to-archive-a-payment-slip"></a><span data-ttu-id="a25dd-108">Pour archiver un bordereau paiement</span><span class="sxs-lookup"><span data-stu-id="a25dd-108">To archive a payment slip</span></span>  

1.  <span data-ttu-id="a25dd-109">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Icône Page ou état pour la recherche"), saisissez **Bordereaux paiement**, puis sélectionnez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="a25dd-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Slips**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="a25dd-110">Sélectionnez le bordereau paiement concerné, puis cliquez sur l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="a25dd-110">Select the relevant payment slip, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="a25dd-111">Sur la page **Bordereau paiement**, sélectionnez **Archiver**.</span><span class="sxs-lookup"><span data-stu-id="a25dd-111">On the **Payment Slip** page, choose the **Archive** action.</span></span>  
4.  <span data-ttu-id="a25dd-112">Cliquez sur le bouton **Oui** pour archiver le bordereau paiement.</span><span class="sxs-lookup"><span data-stu-id="a25dd-112">Choose the **Yes** button to archive the payment slip.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="a25dd-113">Si le statut actuel du bordereau paiement n'autorise pas l'archivage, un message s'affiche.</span><span class="sxs-lookup"><span data-stu-id="a25dd-113">If the current status of the payment slip does not allow archiving, a message is displayed.</span></span>  

## <a name="to-archive-a-batch-of-payment-slips"></a><span data-ttu-id="a25dd-114">Pour archiver un lot de bordereaux paiement</span><span class="sxs-lookup"><span data-stu-id="a25dd-114">To archive a batch of payment slips</span></span>  

1.  <span data-ttu-id="a25dd-115">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Icône Page ou état pour la recherche"), saisissez **Archiver les bordereaux de paiement**, puis sélectionnez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="a25dd-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Archive Payment Slips**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="a25dd-116">Sur la page **Archiver les bordereaux de paiement**, sur le raccourci **En-tête bordereau**, sélectionnez les filtres appropriés.</span><span class="sxs-lookup"><span data-stu-id="a25dd-116">On the **Archive Payment Slips** page, on the **Payment Header** FastTab, select the appropriate filters.</span></span>  
3.  <span data-ttu-id="a25dd-117">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="a25dd-117">Choose the **OK** button.</span></span>  

<span data-ttu-id="a25dd-118">Les bordereaux paiement sont archivés.</span><span class="sxs-lookup"><span data-stu-id="a25dd-118">The payment slips are archived.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a25dd-119">Ce traitement par lots archive uniquement les bordereaux paiement dont la case **Archivage autorisé** est cochée sur la page **Statut règlement**.</span><span class="sxs-lookup"><span data-stu-id="a25dd-119">This batch job will only archive payment slips that have the **Archiving Authorized** check box selected on the **Payment Status** page.</span></span> <span data-ttu-id="a25dd-120">Pour plus d'informations, voir [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md).</span><span class="sxs-lookup"><span data-stu-id="a25dd-120">For more information, see [Set Up Payment Statuses](how-to-set-up-payment-statuses.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="a25dd-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a25dd-121">See Also</span></span>  
 <span data-ttu-id="a25dd-122">[Gestion des paiements](payment-management.md) </span><span class="sxs-lookup"><span data-stu-id="a25dd-122">[Payment Management](payment-management.md) </span></span>  
 <span data-ttu-id="a25dd-123">[Paramétrer des types de règlement](how-to-set-up-payment-classes.md) </span><span class="sxs-lookup"><span data-stu-id="a25dd-123">[Set Up Payment Classes](how-to-set-up-payment-classes.md) </span></span>  
 <span data-ttu-id="a25dd-124">[Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md) </span><span class="sxs-lookup"><span data-stu-id="a25dd-124">[Set Up Payment Statuses](how-to-set-up-payment-statuses.md) </span></span>  
 <span data-ttu-id="a25dd-125">[Paramétrer des étapes règlement](how-to-set-up-payment-steps.md) </span><span class="sxs-lookup"><span data-stu-id="a25dd-125">[Set Up Payment Steps](how-to-set-up-payment-steps.md) </span></span>  
 <span data-ttu-id="a25dd-126">[Configurer des adresses de paiement](how-to-set-up-payment-addresses.md) </span><span class="sxs-lookup"><span data-stu-id="a25dd-126">[Set Up Payment Addresses](how-to-set-up-payment-addresses.md) </span></span>  
 <span data-ttu-id="a25dd-127">[Créer bordereaux paiement](how-to-create-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="a25dd-127">[Create Payment Slips](how-to-create-payment-slips.md) </span></span>  
 [<span data-ttu-id="a25dd-128">Valider des bordereaux paiement</span><span class="sxs-lookup"><span data-stu-id="a25dd-128">Post Payment Slips</span></span>](how-to-post-payment-slips.md)
