---
title: "Définition des centres de coûts et des coûts associés pour le plan comptable | Microsoft Docs"
description: "Vous pouvez transférer automatiquement les écritures de dépenses et de revenus à partir de la comptabilité générale vers la comptabilité analytique, que ce soit pour la validation comptable ou avec un traitement par lots. Lors du transfert, le système transfère uniquement les écritures déjà liées à un centre de coûts ou aux coûts associés. Pour préparer un transfert pertinent, assurez-vous que les centres de coûts et les coûts associés sont définis correctement."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 0a3b89e2d2a59aa3434e747976437f24860be408
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="defining-cost-centers-and-cost-objects-for-chart-of-accounts"></a><span data-ttu-id="97fa2-105">Définition des centres de coûts et des coûts associés pour le plan comptable</span><span class="sxs-lookup"><span data-stu-id="97fa2-105">Defining Cost Centers and Cost Objects for Chart of Accounts</span></span>
<span data-ttu-id="97fa2-106">Vous pouvez transférer automatiquement les écritures de dépenses et de revenus à partir de la comptabilité générale vers la comptabilité analytique, que ce soit pour la validation comptable ou avec un traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="97fa2-106">You can automatically transfer the expense and income entries from the general ledger to cost accounting either for each general ledger posting or with a batch job.</span></span> <span data-ttu-id="97fa2-107">Lors du transfert, [!INCLUDE[d365fin](includes/d365fin_md.md)] transfère uniquement les écritures déjà liées à un centre de coûts ou aux coûts associés.</span><span class="sxs-lookup"><span data-stu-id="97fa2-107">When you do the transfer, [!INCLUDE[d365fin](includes/d365fin_md.md)] only transfers the entries that are already linked to a cost center or a cost object.</span></span> <span data-ttu-id="97fa2-108">Pour préparer un transfert pertinent, assurez-vous que les centres de coûts et les coûts associés sont définis correctement.</span><span class="sxs-lookup"><span data-stu-id="97fa2-108">To establish a meaningful transfer, you must ensure that the cost centers and cost objects are correctly defined.</span></span>  

## <a name="defining-default-dimension-values-for-general-ledger-accounts"></a><span data-ttu-id="97fa2-109">Définition des sections analytiques par défaut pour des comptes généraux</span><span class="sxs-lookup"><span data-stu-id="97fa2-109">Defining Default Dimension Values for General Ledger Accounts</span></span>  
<span data-ttu-id="97fa2-110">Pour chaque compte général, vous pouvez définir des sections analytiques par défaut dans la table **Affectation analytique**.</span><span class="sxs-lookup"><span data-stu-id="97fa2-110">For each general ledger account, you can define default dimension values in the **Default Dimension** table.</span></span> <span data-ttu-id="97fa2-111">L'exemple suivant décrit la configuration requise pour avoir un centre de coût DÉPARTEMENT sans jamais avoir de coûts associés PROJET lors de la validation d'un compte général.</span><span class="sxs-lookup"><span data-stu-id="97fa2-111">The following example shows how to define that there should always be a DEPARTMENT cost center, but never be a PROJECT cost object when posting to a general ledger account.</span></span>  

|<span data-ttu-id="97fa2-112">**Code axe analytique**</span><span class="sxs-lookup"><span data-stu-id="97fa2-112">**Dimension Code**</span></span>|<span data-ttu-id="97fa2-113">**Contrôle validation**</span><span class="sxs-lookup"><span data-stu-id="97fa2-113">**Value Posting**</span></span>|  
|------------------------------------------|-----------------------------------------|  
|<span data-ttu-id="97fa2-114">Département</span><span class="sxs-lookup"><span data-stu-id="97fa2-114">Department</span></span>|<span data-ttu-id="97fa2-115">Code obligatoire</span><span class="sxs-lookup"><span data-stu-id="97fa2-115">Code Mandatory</span></span>|  
|<span data-ttu-id="97fa2-116">Dossier</span><span class="sxs-lookup"><span data-stu-id="97fa2-116">Project</span></span>|<span data-ttu-id="97fa2-117">Pas de code</span><span class="sxs-lookup"><span data-stu-id="97fa2-117">No Code</span></span>|  

## <a name="defining-dimension-values-for-overhead-costs-and-direct-costs"></a><span data-ttu-id="97fa2-118">Définition des sections analytiques pour les frais généraux et les coûts directs</span><span class="sxs-lookup"><span data-stu-id="97fa2-118">Defining Dimension Values for Overhead Costs and Direct Costs</span></span>  
 <span data-ttu-id="97fa2-119">Vous pouvez transférer des frais généraux à un centre de coûts, et des coûts directs aux coûts associés.</span><span class="sxs-lookup"><span data-stu-id="97fa2-119">You can transfer overhead costs to a cost center and direct costs to a cost object.</span></span> <span data-ttu-id="97fa2-120">Le tableau suivant décrit comment optimiser la combinaison des valeurs de paramétrage des axes analytiques.</span><span class="sxs-lookup"><span data-stu-id="97fa2-120">The following table shows the optimal combination of the dimension setup values.</span></span>  

|<span data-ttu-id="97fa2-121">Transférer vers</span><span class="sxs-lookup"><span data-stu-id="97fa2-121">Transfer To</span></span>|<span data-ttu-id="97fa2-122">Validation du centre de coûts</span><span class="sxs-lookup"><span data-stu-id="97fa2-122">Cost Center Posting</span></span>|<span data-ttu-id="97fa2-123">Validation des coûts associés</span><span class="sxs-lookup"><span data-stu-id="97fa2-123">Cost Object Posting</span></span>|  
|-----------------|-------------------------|-------------------------|  
|<span data-ttu-id="97fa2-124">Centre de coûts</span><span class="sxs-lookup"><span data-stu-id="97fa2-124">Cost Center</span></span>|<span data-ttu-id="97fa2-125">Code obligatoire</span><span class="sxs-lookup"><span data-stu-id="97fa2-125">Code Mandatory</span></span>|<span data-ttu-id="97fa2-126">Pas de code</span><span class="sxs-lookup"><span data-stu-id="97fa2-126">No Code</span></span>|  
|<span data-ttu-id="97fa2-127">Coûts associés</span><span class="sxs-lookup"><span data-stu-id="97fa2-127">Cost Object</span></span>|<span data-ttu-id="97fa2-128">Pas de code</span><span class="sxs-lookup"><span data-stu-id="97fa2-128">No Code</span></span>|<span data-ttu-id="97fa2-129">Code obligatoire</span><span class="sxs-lookup"><span data-stu-id="97fa2-129">Code Mandatory</span></span>|  

> [!NOTE]  
>  <span data-ttu-id="97fa2-130">Pour vous assurer que le centre de coûts et les coûts associés prédéfinis et configurés en comptabilité générale sont reportés automatiquement dans la comptabilité analytique, cochez la case **Vérifier validations compta** dans la fenêtre Paramètres comptabilité analytique.</span><span class="sxs-lookup"><span data-stu-id="97fa2-130">To make sure that the predefined cost center and cost object that you set up in the general ledger are automatically carried over to cost accounting, select the **Check G/L Postings** check box in the Cost Accounting Setup window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="97fa2-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="97fa2-131">See Also</span></span>  
[<span data-ttu-id="97fa2-132">Comptabilité pour les coûts</span><span class="sxs-lookup"><span data-stu-id="97fa2-132">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="97fa2-133">[Procédure : configuration des centres de coûts](finance-how-to-set-up-cost-centers.md) </span><span class="sxs-lookup"><span data-stu-id="97fa2-133">[How to: Set Up Cost Centers](finance-how-to-set-up-cost-centers.md) </span></span>  
[<span data-ttu-id="97fa2-134">Procédure : configurer les coûts associés</span><span class="sxs-lookup"><span data-stu-id="97fa2-134">How to: Set Up Cost Objects</span></span>](finance-how-to-set-up-cost-objects.md)  
<span data-ttu-id="97fa2-135">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="97fa2-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

