---
title: "Déplacement d'articles | Microsoft Docs"
description: "Lorsque les articles sont en stock, il peut être nécessaire de les déplacer entre plusieurs emplacements pour prendre en charge les activités entrepôt quotidiennes permettant de conserver le flux d'articles dans l'entrepôt. Certains mouvements se produisent en relation directe avec les opérations internes ; par exemple, lorsqu'un ordre de fabrication impose que des composants soient livrés ou que des produits finis soient rangés. D'autres mouvements se produisent dans le cadre d'une simple optimisation de l'espace des entrepôts ou en tant que mouvements ad-hoc depuis ou vers des opérations."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: f52353ec74b10983b0acfd04169d6b146c70eb84
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="moving-items"></a><span data-ttu-id="c4155-105">Déplacement d'articles</span><span class="sxs-lookup"><span data-stu-id="c4155-105">Moving Items</span></span>
<span data-ttu-id="c4155-106">L'activité entrepôt consistant à déplacer les articles dans l'entrepôt s'exécute différemment selon la configuration des fonctionnalités du module Gestion d'entrepôt.</span><span class="sxs-lookup"><span data-stu-id="c4155-106">The warehouse activity of moving items within the warehouse is performed in different ways depending on how warehouse management features are configured.</span></span> <span data-ttu-id="c4155-107">Le niveau de complexité du paramétrage varie : aucune fonctionnalité entrepôt, configurations de stockage de base pour le traitement par commande dans une ou plusieurs activités uniquement, configurations avancées dans lesquelles toutes les activités entrepôt doivent être exécutées dans un flux suggéré.</span><span class="sxs-lookup"><span data-stu-id="c4155-107">The complexity can rank from no warehouse features, through basic warehouse configurations for order-by order handling in one or more activities only, to advanced configurations where all warehouse activities must be performed in a directed workflow.</span></span> <span data-ttu-id="c4155-108">Pour plus d'informations, voir [Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="c4155-108">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

<span data-ttu-id="c4155-109">Dans un entrepôt, il peut être nécessaire de les déplacer entre plusieurs emplacements pour prendre en charge les activités entrepôt quotidiennes permettant de conserver le flux d'articles dans l'entrepôt.</span><span class="sxs-lookup"><span data-stu-id="c4155-109">While in one warehouse location, items may need to be moved between bins to support the daily warehouse activities involved in keeping items flowing through the warehouse.</span></span> <span data-ttu-id="c4155-110">Certains mouvements se produisent en relation directe avec les opérations internes ; par exemple, lorsqu'un ordre de fabrication impose que des composants soient livrés ou que des produits finis soient rangés.</span><span class="sxs-lookup"><span data-stu-id="c4155-110">Some movements happen in direct relation to internal operations, such as a production order that needs components delivered or end items put away.</span></span> <span data-ttu-id="c4155-111">D'autres mouvements se produisent dans le cadre d'une simple optimisation de l'espace des entrepôts ou en tant que mouvements ad-hoc depuis ou vers des opérations.</span><span class="sxs-lookup"><span data-stu-id="c4155-111">Other movements happen as mere warehouse space optimization or as ad-hoc movements to and from operations.</span></span>

<span data-ttu-id="c4155-112">Si le déplacement a lieu vers d'autres magasins, il a une incidence sur les écritures comptables article et doit donc être effectué dans le cadre d'un ordre de transfert.</span><span class="sxs-lookup"><span data-stu-id="c4155-112">Moving items to other locations affects the item ledger entries and must therefore be done by transfer order.</span></span> <span data-ttu-id="c4155-113">Pour plus d'informations, voir [Procédure : Transfert de stock entre des magasins](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="c4155-113">For more information, see [How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>  

<span data-ttu-id="c4155-114">Des tâches de mouvement ont lieu régulièrement afin de réapprovisionner les emplacements prélèvement et atelier et modifier les informations relatives au contenu des emplacements.</span><span class="sxs-lookup"><span data-stu-id="c4155-114">Additional movement tasks are to periodically replenish picking bins or shop floor bins and to modify bin content information.</span></span>  

 <span data-ttu-id="c4155-115">Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.</span><span class="sxs-lookup"><span data-stu-id="c4155-115">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="c4155-116">**Pour**</span><span class="sxs-lookup"><span data-stu-id="c4155-116">**To**</span></span>|<span data-ttu-id="c4155-117">**Voir**</span><span class="sxs-lookup"><span data-stu-id="c4155-117">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="c4155-118">Déplacer des articles d'un emplacement à l'autre dans des configurations entrepôt de base à tout moment et sans documents origine.</span><span class="sxs-lookup"><span data-stu-id="c4155-118">Move items between bins in basic warehouse configurations at any time and without source documents.</span></span>|[<span data-ttu-id="c4155-119">Procédure : déplacer des articles dans les configurations de stockage de base</span><span class="sxs-lookup"><span data-stu-id="c4155-119">How to: Move Items in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)|
|<span data-ttu-id="c4155-120">Utiliser la feuille mouvement entrepôt pour déplacer des articles dans des configurations d'entrepôt avancées, pour les documents origine et ad hoc.</span><span class="sxs-lookup"><span data-stu-id="c4155-120">Use the warehouse movement worksheet to move items in advanced warehouse configurations, both for source documents and ad hoc.</span></span>|[<span data-ttu-id="c4155-121">Procédure : déplacer des articles dans les configurations de stockage avancées</span><span class="sxs-lookup"><span data-stu-id="c4155-121">How to: Move Items in Advanced Warehouse Configurations</span></span>](warehouse-how-to-move-items-in-advanced-warehousing.md)|  
|<span data-ttu-id="c4155-122">Ajouter des articles de composant à des opérations internes dans des configurations entrepôt de base en fonction des demandes issues des documents origine de ces opérations.</span><span class="sxs-lookup"><span data-stu-id="c4155-122">Bring component items to internal operations in basic warehouse configurations as requested by source documents for those operations.</span></span>|[<span data-ttu-id="c4155-123">Procédure : déplacer les composants vers une zone opérations dans les configurations de stockage de base</span><span class="sxs-lookup"><span data-stu-id="c4155-123">How to: Move Components to an Operation Area in Basic Warehouse Configurations</span></span>](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)|
|<span data-ttu-id="c4155-124">Planifier les emplacements à remplir ou vider pour maintenir un flux efficace (par exemple, vidage d'une zone de stockage en vrac avant une réception importante).</span><span class="sxs-lookup"><span data-stu-id="c4155-124">Plan which bins to fill or empty to maintain an efficient flow, such as emptying a bulk storage area before a large receipt.</span></span>|[<span data-ttu-id="c4155-125">Comment planifier des mouvements entrepôt dans la feuille</span><span class="sxs-lookup"><span data-stu-id="c4155-125">How to: Plan Warehouse Movements in Worksheets</span></span>](warehouse-how-to-plan-warehouse-movements-in-worksheets.md)|
|<span data-ttu-id="c4155-126">Mettre à jour la fréquence de réapprovisionnement des emplacements (emplacements prélèvement, etc.) suite aux fluctuations de la demande.</span><span class="sxs-lookup"><span data-stu-id="c4155-126">Update the frequency at which bins, such as picking bins, must be replenished as a result of demand fluctuations.</span></span>|[<span data-ttu-id="c4155-127">Procédure : calculer réappro. emplacement</span><span class="sxs-lookup"><span data-stu-id="c4155-127">How to: Calculate Bin Replenishment</span></span>](warehouse-how-to-calculate-bin-replenishment.md)|
|<span data-ttu-id="c4155-128">Restructurez votre entrepôt avec de nouveaux codes et caractéristiques emplacement et déplacez-les potentiellement autour.</span><span class="sxs-lookup"><span data-stu-id="c4155-128">Restructure your warehouse with new bin codes and new bin characteristics and potentially move them around.</span></span>|[<span data-ttu-id="c4155-129">Comment restructurer les entrepôts</span><span class="sxs-lookup"><span data-stu-id="c4155-129">How to: Restructure Warehouses</span></span>](warehouse-how-to-restructure-warehouses.md)|  

## <a name="see-also"></a><span data-ttu-id="c4155-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c4155-130">See Also</span></span>  
[<span data-ttu-id="c4155-131">Gestion d'entrepôt</span><span class="sxs-lookup"><span data-stu-id="c4155-131">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="c4155-132">STOCKS ET EN-COURS</span><span class="sxs-lookup"><span data-stu-id="c4155-132">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="c4155-133">[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="c4155-133">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="c4155-134">[Gestion des assemblages](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="c4155-134">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="c4155-135">Détails de conception : gestion d'entrepôt</span><span class="sxs-lookup"><span data-stu-id="c4155-135">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="c4155-136">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c4155-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
