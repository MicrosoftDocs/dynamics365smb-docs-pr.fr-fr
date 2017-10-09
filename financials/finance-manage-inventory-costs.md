---
title: "Gestion des coûts ajustés | Microsoft Docs"
description: "La gestion des coûts, aussi appelée comptabilité analytique, se charge de l'enregistrement et de la déclaration des coûts d'exploitation de la société. Cette activité inclut la déclaration des coûts de fabrication et de stock qui constituent la valeur des articles."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 8da779426dfd06519507796c995adcedcd40ac81
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="managing-inventory-costs"></a><span data-ttu-id="c8326-104">Gestion des coûts ajustés</span><span class="sxs-lookup"><span data-stu-id="c8326-104">Managing Inventory Costs</span></span>
<span data-ttu-id="c8326-105">La gestion des coûts, aussi appelée comptabilité analytique, se charge de l'enregistrement et de la déclaration des coûts d'exploitation de la société.</span><span class="sxs-lookup"><span data-stu-id="c8326-105">Cost management, also referred to as “costing”, is concerned with recording and reporting business operating costs.</span></span> <span data-ttu-id="c8326-106">Cette activité inclut la déclaration des coûts de fabrication et de stock qui constituent la valeur des articles.</span><span class="sxs-lookup"><span data-stu-id="c8326-106">It includes the reporting of manufacturing costs and inventory costs, that is, the value of items.</span></span>   

<span data-ttu-id="c8326-107">Il est essentiel de comprendre les principes suivants : les méthodes d'évaluation des stocks au prix coûtant définissent le mode d'évaluation des articles lors de leur sortie de stock, l'ajustement des coûts met à jour le coût des biens vendus avec les coûts d'achat associés validés après la vente, les valeurs en stock doivent être validées vers les comptes généraux appropriés à des intervalles réguliers.</span><span class="sxs-lookup"><span data-stu-id="c8326-107">Central principles to understand are that costing methods define how items are valued when they leave inventory, that cost adjustment updates the cost of goods sold with related purchase costs posted after the sale, and that inventory values must be posted to dedicated G/L accounts at regular intervals.</span></span>

<span data-ttu-id="c8326-108">Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.</span><span class="sxs-lookup"><span data-stu-id="c8326-108">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="c8326-109">**Pour**</span><span class="sxs-lookup"><span data-stu-id="c8326-109">**To**</span></span>|<span data-ttu-id="c8326-110">**Voir**</span><span class="sxs-lookup"><span data-stu-id="c8326-110">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="c8326-111">Lire différentes informations conceptuelles pour comprendre les principes et définitions qui gouvernent la fonctionnalité Comptabilité des coûts de stock [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="c8326-111">Read various conceptual information to understand the principles and definitions that govern the inventory costing accounting functionality in [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)].</span></span>|[<span data-ttu-id="c8326-112">À propos de l'évaluation des coûts de stock</span><span class="sxs-lookup"><span data-stu-id="c8326-112">About Inventory Costing</span></span>](finance-learn-about-costing.md)|  
|<span data-ttu-id="c8326-113">Configurer les périodes inventaire, les méthodes d'évaluation des stocks au prix coûtant et les modes d'arrondi.</span><span class="sxs-lookup"><span data-stu-id="c8326-113">Set up inventory periods, costing methods, and rounding methods.</span></span>|[<span data-ttu-id="c8326-114">Configuration de l'évaluation du stock</span><span class="sxs-lookup"><span data-stu-id="c8326-114">Setting Up Inventory Valuation and Costing</span></span>](finance-set-up-inventory-valuation-and-costing.md)|
|<span data-ttu-id="c8326-115">Réévaluer ou amortir la valeur d'un ou de plusieurs articles dans le stock en validant leur valeur calculée courante.</span><span class="sxs-lookup"><span data-stu-id="c8326-115">Appreciate or depreciate the value of one or more items in inventory by posting their current, calculated value.</span></span>|[<span data-ttu-id="c8326-116">Procédure : réévaluer le stock</span><span class="sxs-lookup"><span data-stu-id="c8326-116">How to: Revalue Inventory</span></span>](inventory-how-revalue-inventory.md)|
|<span data-ttu-id="c8326-117">Ajuster les coûts d'article, automatiquement ou manuellement, pour transférer les modifications de coût des écritures entrantes à leurs écritures sortantes associées.</span><span class="sxs-lookup"><span data-stu-id="c8326-117">Adjust item costs, either automatically or manually, to forward cost changes from inbound entries to their related outbound entries.</span></span>|[<span data-ttu-id="c8326-118">Procédure : ajustement des coûts article</span><span class="sxs-lookup"><span data-stu-id="c8326-118">How to: Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|
|<span data-ttu-id="c8326-119">Utiliser les fonctions d'évaluation des coûts spéciales pour les transactions article quotidiennes dans les opérations liées aux articles.</span><span class="sxs-lookup"><span data-stu-id="c8326-119">Use special costing functions for every-day item transactions in the item operations.</span></span>|[<span data-ttu-id="c8326-120">Gestion des coûts ajustés et des coûts de fabrication</span><span class="sxs-lookup"><span data-stu-id="c8326-120">Handling Inventory and Manufacturing Costs</span></span>](finance-handle-inventory-and-manufacturing-costs.md)|  
|<span data-ttu-id="c8326-121">Actualisez périodiquement les coûts standard des composants, dans les nomenclatures d'assemblage ou de production, et remonter les nouveaux coûts dans l'article parent.</span><span class="sxs-lookup"><span data-stu-id="c8326-121">Periodically update the standard costs of components, in assembly or production BOMs, and roll the new costs up to the parent item.</span></span>|[<span data-ttu-id="c8326-122">Procédure : mise à jour des coûts standard</span><span class="sxs-lookup"><span data-stu-id="c8326-122">How to: Update Standard Costs</span></span>](finance-how-to-update-standard-costs.md)|
|<span data-ttu-id="c8326-123">Effectuer un contrôle de clôture d'exercice et des tâches de création de rapports, tels que le calcul de la valeur du stock et la validation des coûts dans la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="c8326-123">Perform period-end control and reporting tasks, such calculate the value of inventory and post costs to the general ledger.</span></span>|[<span data-ttu-id="c8326-124">Génération des coûts et rapprochement en comptabilité</span><span class="sxs-lookup"><span data-stu-id="c8326-124">Reporting Costs and Reconciling with the General Ledger</span></span>](finance-report-costs-and-reconcile-with-the-general-ledger.md)|  
|<span data-ttu-id="c8326-125">En savoir plus sur les mécanismes dans le système d'évaluation.</span><span class="sxs-lookup"><span data-stu-id="c8326-125">Learn about all mechanisms in the costing system.</span></span>|[<span data-ttu-id="c8326-126">Détails de conception : évaluation stock</span><span class="sxs-lookup"><span data-stu-id="c8326-126">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|  

## <a name="see-also"></a><span data-ttu-id="c8326-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c8326-127">See Also</span></span>  
 [<span data-ttu-id="c8326-128">Finances</span><span class="sxs-lookup"><span data-stu-id="c8326-128">Finance</span></span>](finance.md)  
 <span data-ttu-id="c8326-129">[STOCKS ET EN-COURS](inventory-manage-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="c8326-129">[Inventory](inventory-manage-inventory.md) </span></span>  
 <span data-ttu-id="c8326-130">[Ventes](sales-manage-sales.md) </span><span class="sxs-lookup"><span data-stu-id="c8326-130">[Sales](sales-manage-sales.md) </span></span>  
 [<span data-ttu-id="c8326-131">Achats</span><span class="sxs-lookup"><span data-stu-id="c8326-131">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="c8326-132">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c8326-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

