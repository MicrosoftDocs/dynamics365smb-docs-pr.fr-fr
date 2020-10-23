---
title: Procédure de paramétrage de l'amortissement accéléré
description: Pour utiliser la fonction de calcul de l'amortissement accéléré, vous devez configurer les lois d'amortissement pour les immobilisations.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 41fd82c4632713fc3b0092d76c7d1667f0c203af
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/01/2020
ms.locfileid: "3920120"
---
# <a name="set-up-accelerated-depreciation"></a><span data-ttu-id="1dda5-103">Paramétrer l'amortissement accéléré</span><span class="sxs-lookup"><span data-stu-id="1dda5-103">Set Up Accelerated Depreciation</span></span>
<span data-ttu-id="1dda5-104">Pour utiliser la fonction de calcul de l'amortissement accéléré, vous devez configurer les lois d'amortissement suivantes pour les immobilisations :</span><span class="sxs-lookup"><span data-stu-id="1dda5-104">To use the accelerated depreciation calculation, you must set up the following depreciation books for fixed assets:</span></span>  

- <span data-ttu-id="1dda5-105">la loi d'amortissement comptable (intégrée à la comptabilité) ;</span><span class="sxs-lookup"><span data-stu-id="1dda5-105">The accounting depreciation book (integrated with the general ledger).</span></span>  
- <span data-ttu-id="1dda5-106">la loi d'amortissement fiscal (non intégrée à la comptabilité).</span><span class="sxs-lookup"><span data-stu-id="1dda5-106">The tax depreciation book (not integrated with the general ledger).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="1dda5-107">Lorsque vous validez une acquisition, un amortissement ou une cession pour la loi d'amortissement comptable, la transaction est automatiquement dupliquée et validée dans la loi d'amortissement fiscal lorsque la feuille immobilisation est validée.</span><span class="sxs-lookup"><span data-stu-id="1dda5-107">When you post an acquisition, depreciation, or disposal for the accounting depreciation book, the transaction is duplicated and posted in the tax depreciation book when the fixed asset journal is posted.</span></span>  

## <a name="to-set-up-the-accounting-depreciation-book"></a><span data-ttu-id="1dda5-108">Pour configurer la loi d'amortissement comptable</span><span class="sxs-lookup"><span data-stu-id="1dda5-108">To set up the accounting depreciation book</span></span>  

1.  <span data-ttu-id="1dda5-109">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Lois d'amortissement**, puis choisissez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="1dda5-109">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Depreciation Books**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="1dda5-110">Sur la page **Liste de la loi d'amortissement**, sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="1dda5-110">On the **Depreciation Book List** page, choose ¨the **New** action.</span></span>  
3.  <span data-ttu-id="1dda5-111">Sous le raccourci **Général**, renseignez les champs obligatoires comme indiqué dans le tableau ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="1dda5-111">On the **General** FastTab, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="1dda5-112">Champ</span><span class="sxs-lookup"><span data-stu-id="1dda5-112">Field</span></span>|<span data-ttu-id="1dda5-113">Désignation</span><span class="sxs-lookup"><span data-stu-id="1dda5-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="1dda5-114">**Code**</span><span class="sxs-lookup"><span data-stu-id="1dda5-114">**Code**</span></span>|<span data-ttu-id="1dda5-115">Code d'identification unique de la loi d'amortissement comptable.</span><span class="sxs-lookup"><span data-stu-id="1dda5-115">The unique identification code for the accounting depreciation book.</span></span> <span data-ttu-id="1dda5-116">Vous pouvez entrer 10 caractères alphanumériques maximum.</span><span class="sxs-lookup"><span data-stu-id="1dda5-116">You can enter a maximum of 10 alphanumeric characters.</span></span>|  
    |<span data-ttu-id="1dda5-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1dda5-117">**Description**</span></span>|<span data-ttu-id="1dda5-118">Description des lois d'amortissement.</span><span class="sxs-lookup"><span data-stu-id="1dda5-118">The depreciation book description.</span></span>|  

    > [!IMPORTANT]  
    >  <span data-ttu-id="1dda5-119">Laissez le champ **Calcul dérogatoire** vide.</span><span class="sxs-lookup"><span data-stu-id="1dda5-119">Leave the **Derogatory Calculation** field blank.</span></span>  

4.  <span data-ttu-id="1dda5-120">Dans le raccourci **Intégration**, sélectionnez la case à cocher **Dérogatoire** pour intégrer l'amortissement accéléré dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="1dda5-120">On the **Integration** FastTab, select the **Derogatory** check box to integrate accelerated depreciation with the general ledger.</span></span>  

    <span data-ttu-id="1dda5-121">Pour en savoir plus, voir [Configurer l'amortissement d'immobilisation](../../fa-how-setup-depreciation.md).</span><span class="sxs-lookup"><span data-stu-id="1dda5-121">For more information, see [Set Up Fixed Asset Depreciation](../../fa-how-setup-depreciation.md).</span></span>  

5.  <span data-ttu-id="1dda5-122">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="1dda5-122">Choose the **OK** button.</span></span>  

## <a name="to-set-up-the-tax-depreciation-book"></a><span data-ttu-id="1dda5-123">Pour configurer la loi d'amortissement fiscal</span><span class="sxs-lookup"><span data-stu-id="1dda5-123">To set up the tax depreciation book</span></span>  

1.  <span data-ttu-id="1dda5-124">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Lois d'amortissement**, puis choisissez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="1dda5-124">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Depreciation Books**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="1dda5-125">Sur la page **Liste de la loi d'amortissement**, sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="1dda5-125">On the **Depreciation Book List** page, choose the **New** action.</span></span>  
3.  <span data-ttu-id="1dda5-126">Sous le raccourci **Général**, renseignez les champs obligatoires comme indiqué dans le tableau ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="1dda5-126">On the **General** FastTab, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="1dda5-127">Champ</span><span class="sxs-lookup"><span data-stu-id="1dda5-127">Field</span></span>|<span data-ttu-id="1dda5-128">Désignation</span><span class="sxs-lookup"><span data-stu-id="1dda5-128">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="1dda5-129">**Code**</span><span class="sxs-lookup"><span data-stu-id="1dda5-129">**Code**</span></span>|<span data-ttu-id="1dda5-130">Code d'identification unique de la loi d'amortissement fiscal.</span><span class="sxs-lookup"><span data-stu-id="1dda5-130">The unique identification code for the tax depreciation book.</span></span> <span data-ttu-id="1dda5-131">Vous pouvez entrer 10 caractères alphanumériques maximum.</span><span class="sxs-lookup"><span data-stu-id="1dda5-131">You can enter a maximum of 10 alphanumeric characters.</span></span>|  
    |<span data-ttu-id="1dda5-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="1dda5-132">**Description**</span></span>|<span data-ttu-id="1dda5-133">Description des lois d'amortissement fiscal.</span><span class="sxs-lookup"><span data-stu-id="1dda5-133">The tax depreciation book description.</span></span>|  

4.  <span data-ttu-id="1dda5-134">Dans le champ **Calcul dérogatoire**, sélectionnez une loi d'amortissement comptable pour indiquer qu'il s'agit d'une loi d'amortissement fiscal pour le calcul de l'amortissement dérogatoire.</span><span class="sxs-lookup"><span data-stu-id="1dda5-134">In the **Derogatory Calculation** field, select the accounting depreciation book code to indicate that this is a tax depreciation book to calculate derogatory depreciation.</span></span>  

    <span data-ttu-id="1dda5-135">Pour en savoir plus, voir [Configurer l'amortissement d'immobilisation](../../fa-how-setup-depreciation.md).</span><span class="sxs-lookup"><span data-stu-id="1dda5-135">For more information, see [Set Up Fixed Asset Depreciation](../../fa-how-setup-depreciation.md).</span></span>  

5.  <span data-ttu-id="1dda5-136">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="1dda5-136">Choose the **OK** button.</span></span>  

<span data-ttu-id="1dda5-137">Le champ **Utilisé avec la loi dérogatoire** dans la loi d'amortissement comptable est mis à jour avec le code de la loi d'amortissement fiscal.</span><span class="sxs-lookup"><span data-stu-id="1dda5-137">The **Used with Derogatory Book** field in the accounting depreciation book is updated with the tax depreciation book code.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1dda5-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1dda5-138">See Also</span></span>  
 <span data-ttu-id="1dda5-139">[Amortissement accéléré](accelerated-depreciation.md) </span><span class="sxs-lookup"><span data-stu-id="1dda5-139">[Accelerated Depreciation](accelerated-depreciation.md) </span></span>  
 <span data-ttu-id="1dda5-140">[Calculer l'amortissement accéléré](how-to-calculate-accelerated-depreciation.md) </span><span class="sxs-lookup"><span data-stu-id="1dda5-140">[Calculate Accelerated Depreciation](how-to-calculate-accelerated-depreciation.md) </span></span>  
[<span data-ttu-id="1dda5-141">Configurer un amortissement immobilisation</span><span class="sxs-lookup"><span data-stu-id="1dda5-141">Set Up Fixed Asset Depreciation</span></span>](../../fa-how-setup-depreciation.md)
