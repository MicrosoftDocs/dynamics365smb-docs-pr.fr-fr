---
title: "Détails de conception - Intégration avec le stock | Microsoft Docs"
description: "La zone d'application Warehouse Management et la zone d'application Inventory interagissent dans le stock physique et dans l'ajustement de stock ou entrepôt."
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
ms.openlocfilehash: 00a12f3f2203ed3b22cfee1af6aa8f155ca5fe4b
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-integration-with-inventory"></a><span data-ttu-id="b2cc9-103">Détails de conception : intégration avec le stock</span><span class="sxs-lookup"><span data-stu-id="b2cc9-103">Design Details: Integration with Inventory</span></span>
<span data-ttu-id="b2cc9-104">La zone d'application Warehouse Management et la zone d'application Inventory interagissent dans le stock physique et dans l'ajustement de stock ou entrepôt.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-104">The Warehouse Management application area and the Inventory application area interact with one another in physical inventory and in inventory or warehouse adjustment.</span></span>  
  
## <a name="physical-inventory"></a><span data-ttu-id="b2cc9-105">Inventaire</span><span class="sxs-lookup"><span data-stu-id="b2cc9-105">Physical Inventory</span></span>  
 <span data-ttu-id="b2cc9-106">La fenêtre **Feuille inventaire entrepôt** est utilisée avec la fenêtre **Feuille inventaire** pour tous les entrepôts avancés.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-106">The **Whse. Phys. Inventory Journal** window is used with the **Phys. Inventory Journal** window for all advanced warehouse locations.</span></span> <span data-ttu-id="b2cc9-107">Le stock au niveau de l'emplacement est calculé, et une liste imprimée est donnée au magasinier.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-107">The inventory on bin level is calculated, and a printed list is provided for the warehouse employee.</span></span> <span data-ttu-id="b2cc9-108">La liste indique les articles dans lesquels les emplacements doivent être comptabilisés.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-108">The list shows which items in which bins must be counted.</span></span>  
  
 <span data-ttu-id="b2cc9-109">Le magasinier entre la quantité comptée dans la fenêtre **Feuille inventaire entrepôt** puis valide la feuille.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-109">The warehouse employee enters the counted quantity in the **Whse. Phys. Inventory Journal** window and then posts the journal.</span></span>  
  
 <span data-ttu-id="b2cc9-110">Si la quantité comptée est supérieure à la quantité de la ligne feuille, un mouvement est validé pour cette différence à partir de l'emplacement ajustement par défaut jusqu'à l'emplacement compté.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-110">If the counted quantity is greater than the quantity on the journal line, a movement is posted for this difference from the default adjustment bin to the counted bin.</span></span> <span data-ttu-id="b2cc9-111">Cela augmente la quantité dans l'emplacement compté et diminue la quantité dans l'emplacement d'ajustement par défaut.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-111">This increases the quantity in the counted bin and decreases the quantity in the default adjustment bin.</span></span>  
  
 <span data-ttu-id="b2cc9-112">Si la quantité comptée est inférieure à la quantité de la ligne feuille, un mouvement pour cette différence est validé à partir de l'emplacement compté jusqu'à l'emplacement d'ajustement par défaut.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-112">If the quantity counted is less than the quantity on the journal line, a movement for this difference is posted from the counted bin to the default adjustment bin.</span></span> <span data-ttu-id="b2cc9-113">Cela diminue la quantité dans l'emplacement compté et augmente la quantité dans l'emplacement d'ajustement par défaut.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-113">This decreases the quantity in the counted bin and increases the quantity in the default adjustment bin.</span></span>  
  
 <span data-ttu-id="b2cc9-114">Dans les configurations d'entrepôt avancées, la valeur du champ **Quantité (calculée)** est extraite à partir des écritures comptables article et celle du champ **Qté (constatée)** est extraite à partir des écritures entrepôt, hors le contenu de l'emplacement ajustement.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-114">In advanced warehouse configurations, the value in the **Quantity (Calculated)** field is retrieved from item ledger entries and the value in the **Quantity (Phys. Inventory)** field is retrieved from warehouse entries, excluding the adjustment bin content.</span></span> <span data-ttu-id="b2cc9-115">Le champ **Quantité** spécifie la différence entre les deux premiers champs, qui doit être égale au contenu de l'emplacement ajustement.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-115">The **Quantity** field specifies the difference between the first two fields, which should be equal to the contents of the adjustment bin.</span></span>  
  
 <span data-ttu-id="b2cc9-116">Lorsque vous validez la feuille stock physique, le stock et l'emplacement d'ajustement par défaut sont mis à jour.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-116">When you post the physical inventory journal, the inventory and the default adjustment bin are updated.</span></span>  
  
### <a name="warehouse-adjustments-to-the-item-ledger"></a><span data-ttu-id="b2cc9-117">Ajustements d'entrepôt dans l'écriture article</span><span class="sxs-lookup"><span data-stu-id="b2cc9-117">Warehouse Adjustments to the Item Ledger</span></span>  
 <span data-ttu-id="b2cc9-118">Vous utilisez la fenêtre **Feuille article** et la fonction **Calculer ajustement entrepôt** pour ajuster le stock dans l'écriture article conformément à ajustement qui a été apporté sur la quantité d'un article dans un emplacement entrepôt.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-118">You use the **Item Journal** window and the **Calculate Whse. Adjustment** function to adjust inventory on the item ledger in accordance with an adjustment that has been made to the item quantity in a warehouse bin.</span></span> <span data-ttu-id="b2cc9-119">Pour créer un lien entre stock et l'entrepôt, vous devez définir un emplacement d'ajustement par défaut par magasin.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-119">To create a link between the inventory and the warehouse, you must define a default adjustment bin per location.</span></span>  
  
 <span data-ttu-id="b2cc9-120">L'emplacement ajustement par défaut enregistre les articles dans l'entrepôt lorsque vous validez une entrée de stock.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-120">The default adjustment bin registers items in the warehouse when you post an increase for the inventory.</span></span> <span data-ttu-id="b2cc9-121">Toutefois, si vous validez une sortie, la quantité sur l'emplacement par défaut est également diminuée.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-121">However, if you post a decrease, the quantity on the default bin is also decreased.</span></span> <span data-ttu-id="b2cc9-122">Dans les deux cas, les écritures comptables article et les écritures entrepôt sont créées.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-122">In both cases, item ledger entries and warehouse entries are created.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="b2cc9-123">L'emplacement ajustement n'est pas inclus dans le calcul de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-123">The adjustment bin is not included in the availability calculation.</span></span>  
  
 <span data-ttu-id="b2cc9-124">Si vous souhaitez ajuster le contenu de l'emplacement, vous pouvez utiliser la feuille article entrepôt, à partir de laquelle vous pouvez saisir le numéro d'article, le code zone, le code emplacement et la quantité que vous voulez ajuster.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-124">If you want to adjust the bin content, you can use the warehouse item journal, from which you can enter the item number, zone code, bin code, and quantity that you want to adjust.</span></span>  
  
 <span data-ttu-id="b2cc9-125">Si vous saisissez une quantité positive et validez la ligne, le stock enregistré dans les entrées de l'emplacement, et la quantité de l'emplacement ajustement par défaut diminue en conséquence.</span><span class="sxs-lookup"><span data-stu-id="b2cc9-125">If you enter a positive quantity and post the line, then the inventory stored in the bin increases, and the quantity of the default adjustment bin decreases correspondingly.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="b2cc9-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b2cc9-126">See Also</span></span>  
 <span data-ttu-id="b2cc9-127">[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md) </span><span class="sxs-lookup"><span data-stu-id="b2cc9-127">[Design Details: Warehouse Management](design-details-warehouse-management.md) </span></span>  
 [<span data-ttu-id="b2cc9-128">Détails de conception : disponibilité dans l'entrepôt</span><span class="sxs-lookup"><span data-stu-id="b2cc9-128">Design Details: Availability in the Warehouse</span></span>](design-details-availability-in-the-warehouse.md)