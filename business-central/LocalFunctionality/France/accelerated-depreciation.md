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
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 894a34843d4b814a91e38a67592015f7e76cc673
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2019
ms.locfileid: "925348"
---
# <a name="accelerated-depreciation"></a><span data-ttu-id="a37c9-103">Amortissement accéléré</span><span class="sxs-lookup"><span data-stu-id="a37c9-103">Accelerated Depreciation</span></span>
<span data-ttu-id="a37c9-104">L'amortissement accéléré est calculé sur la base des différences entre la loi d'amortissement comptable et la loi d'amortissement fiscal, sur toute la durée de vie de l'immobilisation.</span><span class="sxs-lookup"><span data-stu-id="a37c9-104">Accelerated depreciation is calculated based on the differences between the accounting depreciation book and the tax depreciation book fixed asset, during the life of the fixed asset.</span></span>  

<span data-ttu-id="a37c9-105">Les immobilisations qui ont un amortissement fiscal plus élevé et un amortissement comptable plus faible sont amorties à l'aide de la méthode d'amortissement accéléré, comme l'autorisent les administrations fiscales.</span><span class="sxs-lookup"><span data-stu-id="a37c9-105">Fixed assets that have higher tax depreciation and lower accounting depreciation are depreciated using the accelerated depreciation method, as allowed by the tax authorities.</span></span>  

<span data-ttu-id="a37c9-106">Les sociétés doivent utiliser la méthode d'amortissement accéléré pour valider les montants de taxe supplémentaires si elles remplissent au moins deux des critères suivants :</span><span class="sxs-lookup"><span data-stu-id="a37c9-106">Companies must use the accelerated depreciation method to post the extra tax amounts if they meet at least two of the following criteria:</span></span>  

- <span data-ttu-id="a37c9-107">Elles ont plus de 50 salariés.</span><span class="sxs-lookup"><span data-stu-id="a37c9-107">They have more than 50 employees.</span></span>  
- <span data-ttu-id="a37c9-108">Elles ont au moins deux millions d'euros d'actifs.</span><span class="sxs-lookup"><span data-stu-id="a37c9-108">They have at least two million euros in assets.</span></span>  
- <span data-ttu-id="a37c9-109">Elles ont au moins quatre millions d'euros de chiffre d'affaires.</span><span class="sxs-lookup"><span data-stu-id="a37c9-109">They have at least four million euros in sales.</span></span>  

## <a name="depreciation-book"></a><span data-ttu-id="a37c9-110">Loi d'amortissement</span><span class="sxs-lookup"><span data-stu-id="a37c9-110">Depreciation Book</span></span>  
<span data-ttu-id="a37c9-111">La méthode d'amortissement accéléré vous permet de calculer et de valider les différences entre les montants d'amortissement fiscal et les montants d'amortissement comptable autorisés pour les immobilisations.</span><span class="sxs-lookup"><span data-stu-id="a37c9-111">The accelerated depreciation method helps you to calculate and post differences between tax depreciation amounts and accounting depreciation amounts that are allowed for fixed assets.</span></span> <span data-ttu-id="a37c9-112">Pour calculer l'amortissement accéléré pour les immobilisations, les lois d'amortissement suivantes doivent être configurées :</span><span class="sxs-lookup"><span data-stu-id="a37c9-112">To calculate accelerated depreciation for fixed assets, the following depreciation books must be set up:</span></span>  

- <span data-ttu-id="a37c9-113">la loi d'amortissement comptable (intégrée à la comptabilité) ;</span><span class="sxs-lookup"><span data-stu-id="a37c9-113">The accounting depreciation book (integrated with the general ledger).</span></span>  
- <span data-ttu-id="a37c9-114">la loi d'amortissement fiscal (non intégrée à la comptabilité).</span><span class="sxs-lookup"><span data-stu-id="a37c9-114">The tax depreciation book (not integrated with the general ledger).</span></span>  

<span data-ttu-id="a37c9-115">Vous devez configurer la loi d'amortissement fiscal en tant que loi dérogatoire à l'aide d'un paramètre d'amortissement accéléré.</span><span class="sxs-lookup"><span data-stu-id="a37c9-115">You must set up the tax book as a derogatory book by using an accelerated depreciation setup parameter.</span></span> <span data-ttu-id="a37c9-116">Si ce paramètre est défini, les différences entre la loi d'amortissement fiscal et la loi d'amortissement comptable sont calculées et validées en tant que montants d'amortissement accéléré.</span><span class="sxs-lookup"><span data-stu-id="a37c9-116">If this parameter is set, differences between the tax book and the accounting book are calculated and posted as accelerated depreciation amounts.</span></span> <span data-ttu-id="a37c9-117">Pour en savoir plus, voir [Paramétrer l'amortissement accéléré](how-to-set-up-accelerated-depreciation.md).</span><span class="sxs-lookup"><span data-stu-id="a37c9-117">For more information, see [Set Up Accelerated Depreciation](how-to-set-up-accelerated-depreciation.md).</span></span>  

### <a name="example"></a><span data-ttu-id="a37c9-118">Exemple :</span><span class="sxs-lookup"><span data-stu-id="a37c9-118">Example</span></span>  
 <span data-ttu-id="a37c9-119">Si vous avez une immobilisation d'une valeur de 1 000 euros qui est amortie dans la loi d'amortissement comptable sur cinq ans, et amortie dans la loi d'amortissement fiscal sur trois ans, l'amortissement comptable pour la première année est de 200 euros (1 000/5) et l'amortissement fiscal pour la première année est de 333,33 euros (1 000/3).</span><span class="sxs-lookup"><span data-stu-id="a37c9-119">If you have a fixed asset valued at 1,000 euros that is depreciated in the accounting depreciation book over five years, and depreciated in the tax depreciation book over three years, then the accounting depreciation for the first year is 200 euros (1,000/5) and the tax depreciation for the first year is 333.33 euros (1,000/3).</span></span> <span data-ttu-id="a37c9-120">Le montant d'amortissement accéléré est la différence entre ces deux montants : 133,33 euros (333,33 - 200).</span><span class="sxs-lookup"><span data-stu-id="a37c9-120">The accelerated depreciation amount is the difference between these two amounts: 133.33 euros (333.33 - 200).</span></span>  

## <a name="accelerated-depreciation-accounts"></a><span data-ttu-id="a37c9-121">Montants d'amortissement accéléré</span><span class="sxs-lookup"><span data-stu-id="a37c9-121">Accelerated Depreciation Accounts</span></span>  
<span data-ttu-id="a37c9-122">L'amortissement accéléré utilise le type de comptabilisation immobilisation dérogatoire.</span><span class="sxs-lookup"><span data-stu-id="a37c9-122">Accelerated depreciation uses the derogatory fixed asset posting type.</span></span> <span data-ttu-id="a37c9-123">Les statistiques et les états utilisent ce type de comptabilisation pour déclarer le calcul de l'amortissement accéléré.</span><span class="sxs-lookup"><span data-stu-id="a37c9-123">Statistics and reports use this posting type to report the accelerated depreciation calculation.</span></span> <span data-ttu-id="a37c9-124">Pour en savoir plus, voir [Configurer l'amortissement d'immobilisation](../../fa-how-setup-depreciation.md).</span><span class="sxs-lookup"><span data-stu-id="a37c9-124">For more information, see [Set Up Fixed Asset Depreciation](../../fa-how-setup-depreciation.md).</span></span>  

<span data-ttu-id="a37c9-125">Deux comptes doivent être configurés pour les montants dérogatoires :</span><span class="sxs-lookup"><span data-stu-id="a37c9-125">There are two accounts to set up for derogatory amounts:</span></span>  

- <span data-ttu-id="a37c9-126">Montants d'amortissement accéléré positifs (augmentation de l'amortissement accéléré) :</span><span class="sxs-lookup"><span data-stu-id="a37c9-126">Positive accelerated depreciation amounts (increase of accelerated depreciation):</span></span>  

    - <span data-ttu-id="a37c9-127">Compte dérogatoire</span><span class="sxs-lookup"><span data-stu-id="a37c9-127">Derogatory account</span></span>  
    - <span data-ttu-id="a37c9-128">Compte frais dérogatoire</span><span class="sxs-lookup"><span data-stu-id="a37c9-128">Derogatory expense account</span></span>  
    - <span data-ttu-id="a37c9-129">Montants d'amortissement accéléré négatifs (réduction de l'amortissement accéléré) :</span><span class="sxs-lookup"><span data-stu-id="a37c9-129">Negative accelerated depreciation amounts (decrease of accelerated depreciation):</span></span>  
    - <span data-ttu-id="a37c9-130">Compte dérogatoire sur cession</span><span class="sxs-lookup"><span data-stu-id="a37c9-130">Derogatory Acc. on Disposal</span></span>  
    - <span data-ttu-id="a37c9-131">Compte de contrepartie dérogatoire sur cession</span><span class="sxs-lookup"><span data-stu-id="a37c9-131">Derog. Bal. Acc. on Disposal</span></span>  

<span data-ttu-id="a37c9-132">Si vous validez une acquisition, un amortissement ou une cession pour la loi d'amortissement comptable, la transaction est automatiquement dupliquée et validée dans la loi d'amortissement fiscal lorsque la feuille est validée.</span><span class="sxs-lookup"><span data-stu-id="a37c9-132">If you post an acquisition, depreciation, or disposal for the accounting depreciation book, the transaction is automatically duplicated and posted in the tax depreciation book when the journal is posted.</span></span>  

<span data-ttu-id="a37c9-133">Après avoir configuré la loi d'amortissement fiscal et la loi d'amortissement comptable, l'amortissement accéléré est calculé automatiquement pour les immobilisations à l'aide du traitement par lots Calculer amortissement dans la loi d'amortissement comptable.</span><span class="sxs-lookup"><span data-stu-id="a37c9-133">After you set up the tax depreciation book and the accounting depreciation book, the accelerated depreciation is calculated automatically for fixed assets using the calculate depreciation batch job in the accounting depreciation book.</span></span> <span data-ttu-id="a37c9-134">Pour en savoir plus, voir [Calculer l'amortissement accéléré](how-to-calculate-accelerated-depreciation.md).</span><span class="sxs-lookup"><span data-stu-id="a37c9-134">For more information, see [Calculate Accelerated Depreciation](how-to-calculate-accelerated-depreciation.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="a37c9-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a37c9-135">See Also</span></span>  
 <span data-ttu-id="a37c9-136">[Paramétrer l'amortissement accéléré](how-to-set-up-accelerated-depreciation.md) </span><span class="sxs-lookup"><span data-stu-id="a37c9-136">[Set Up Accelerated Depreciation](how-to-set-up-accelerated-depreciation.md) </span></span>  
 <span data-ttu-id="a37c9-137">[Calculer l'amortissement accéléré](how-to-calculate-accelerated-depreciation.md) </span><span class="sxs-lookup"><span data-stu-id="a37c9-137">[Calculate Accelerated Depreciation](how-to-calculate-accelerated-depreciation.md) </span></span>  
 <span data-ttu-id="a37c9-138">[Configurer un amortissement immobilisation](../../fa-how-setup-depreciation.md) </span><span class="sxs-lookup"><span data-stu-id="a37c9-138">[Set Up Fixed Asset Depreciation](../../fa-how-setup-depreciation.md) </span></span>  
[<span data-ttu-id="a37c9-139">COMPTES D'IMMOBILISATIONS</span><span class="sxs-lookup"><span data-stu-id="a37c9-139">Fixed Assets</span></span>](../../fa-manage.md)  
 [<span data-ttu-id="a37c9-140">Fonctionnalité locale, France</span><span class="sxs-lookup"><span data-stu-id="a37c9-140">France Local Functionality</span></span>](france-local-functionality.md)
