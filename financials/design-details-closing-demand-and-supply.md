---
title: "Détails de conception - Clôture de la demande et de l'approvisionnement | Microsoft Docs"
description: "Cette rubrique suggère des tâches à effectuer une fois les procédures d'équilibrage d'approvisionnement exécutées."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, planning, example, closing, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 0796865fa5b04630cc3ac68a63cc8113664a2d24
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-closing-demand-and-supply"></a><span data-ttu-id="c09cb-103">Détails de conception : clôture de la demande et de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="c09cb-103">Design Details: Closing Demand and Supply</span></span>
<span data-ttu-id="c09cb-104">Lorsque les procédures d'équilibre d'approvisionnement ont été réalisées, il existe trois situations de fin possibles :</span><span class="sxs-lookup"><span data-stu-id="c09cb-104">When the supply balancing procedures have been performed, there are three possible end situations:</span></span>  
  
* <span data-ttu-id="c09cb-105">La quantité et la date requises des événements de demande ont été respectées et leur planification peut être clôturée.</span><span class="sxs-lookup"><span data-stu-id="c09cb-105">The required quantity and date of the demand events have been met and the planning for them can be closed.</span></span> <span data-ttu-id="c09cb-106">L'événement d'approvisionnement est encore ouvert et peut couvrir la demande suivante, donc la procédure de contrepartie peut recommencer avec l'événement d'approvisionnement actif et la demande suivante.</span><span class="sxs-lookup"><span data-stu-id="c09cb-106">The supply event is still open and may be able to cover the next demand, so the balancing procedure can start over with the current supply event and the next demand.</span></span>  
* <span data-ttu-id="c09cb-107">La commande approvisionnement ne peut pas être modifiée pour couvrir l'ensemble de la demande.</span><span class="sxs-lookup"><span data-stu-id="c09cb-107">The supply order cannot be modified to cover all of the demand.</span></span> <span data-ttu-id="c09cb-108">L'événement demande est encore ouvert, avec une certaine quantité non couverte qui peut être couverte par l'événement suivant d'approvisionnement.</span><span class="sxs-lookup"><span data-stu-id="c09cb-108">The demand event is still open, with some uncovered quantity that may be covered by the next supply event.</span></span> <span data-ttu-id="c09cb-109">Ainsi, l'événement d'approvisionnement actuel est fermé, donc l'acte d'équilibrage peut recommencer avec la demande actuelle et l'événement d'approvisionnement suivant.</span><span class="sxs-lookup"><span data-stu-id="c09cb-109">Thus the current supply event is closed, so the balancing act can start over with the current demand and the next supply event.</span></span>  
* <span data-ttu-id="c09cb-110">L'ensemble de la demande a été couvert ; il n'existe aucune demande suivante (ou il n'y a pas de demande du tout).</span><span class="sxs-lookup"><span data-stu-id="c09cb-110">All of the demand has been covered; there is no subsequent demand (or there has been no demand at all).</span></span> <span data-ttu-id="c09cb-111">S'il y a un approvisionnement excédentaire, il peut être diminué (ou annulé), puis être clôturé.</span><span class="sxs-lookup"><span data-stu-id="c09cb-111">If there is any surplus supply, it may be decreased (or canceled) and then closed.</span></span> <span data-ttu-id="c09cb-112">Il est possible que des événements d'approvisionnement supplémentaires existent plus loin dans la chaîne, et ils doivent également être annulés.</span><span class="sxs-lookup"><span data-stu-id="c09cb-112">It is possible that additional supply events exist further along in the chain, and they should also be canceled.</span></span>  
  
<span data-ttu-id="c09cb-113">Enfin, le système de planification crée un lien de chaînage entre l'approvisionnement et la demande.</span><span class="sxs-lookup"><span data-stu-id="c09cb-113">Last, the planning system will create an order tracking link between the supply and the demand.</span></span>  
  
## <a name="creating-the-planning-line-suggested-action"></a><span data-ttu-id="c09cb-114">Création de la ligne planning (action suggérée)</span><span class="sxs-lookup"><span data-stu-id="c09cb-114">Creating the Planning Line (Suggested Action)</span></span>  
<span data-ttu-id="c09cb-115">Si une action quelconque (Nouveau, Changer qté, Replanifier, Replanifier et changer qté ou Annuler) est suggérée pour modifier la commande approvisionnement, le système de planification crée une ligne planning dans la feuille planning.</span><span class="sxs-lookup"><span data-stu-id="c09cb-115">If any action – New, Change Quantity, Reschedule, Reschedule and Change Quantity, or Cancel – is suggested to revise the supply order, the planning system creates a planning line in the planning worksheet.</span></span> <span data-ttu-id="c09cb-116">En raison du chaînage, la ligne planification est créée non seulement lorsque l'événement d'approvisionnement est clôturé, mais également si l'événement de demande est clôturé, même si l'événement d'approvisionnement est encore ouvert et qu'il peut être soumis à des modifications supplémentaires lorsque l'événement de demande suivant est traité.</span><span class="sxs-lookup"><span data-stu-id="c09cb-116">Due to order tracking, the planning line is created not only when the supply event is closed, but also if the demand event is closed, even though the supply event is still open and may be subject to additional changes when the next demand event is processed.</span></span> <span data-ttu-id="c09cb-117">Cela signifie qu'après sa création, la ligne de planification peut être modifiée à nouveau.</span><span class="sxs-lookup"><span data-stu-id="c09cb-117">This means that when first created, the planning line may be changed again.</span></span>  
  
<span data-ttu-id="c09cb-118">Pour réduire l'accès aux bases de données lors du traitement des ordres de fabrication, la ligne de planification peut être maintenue dans trois niveaux, tout en visant à effectuer le niveau de maintenance le moins exigeant :</span><span class="sxs-lookup"><span data-stu-id="c09cb-118">To minimize database access when handling production orders, the planning line can be maintained in three levels, while aiming to perform the least demanding maintenance level:</span></span>  
  
* <span data-ttu-id="c09cb-119">Créer uniquement la ligne planning avec la date d'échéance et la quantité actuelles mais sans gamme et composants.</span><span class="sxs-lookup"><span data-stu-id="c09cb-119">Create only the planning line with the current due date and quantity but without the routing and components.</span></span>  
* <span data-ttu-id="c09cb-120">Inclure la gamme : la gamme planifiée est présentée avec le calcul des dates et heures de début et de fin.</span><span class="sxs-lookup"><span data-stu-id="c09cb-120">Include routing: the planned routing is laid out including calculation of starting and ending dates and times.</span></span> <span data-ttu-id="c09cb-121">Ceci est exigeant en termes d'accès aux bases de données.</span><span class="sxs-lookup"><span data-stu-id="c09cb-121">This is demanding in terms of database accesses.</span></span> <span data-ttu-id="c09cb-122">Pour déterminer les dates de fin et d'échéance, il peut être nécessaire de calculer ceci même si l'événement d'approvisionnement n'a pas été clôturé (dans le cas d'une planification en aval).</span><span class="sxs-lookup"><span data-stu-id="c09cb-122">To determine the ending and due dates, it may be necessary to calculate this even if the supply event has not been closed (in the case of forward scheduling).</span></span>  
* <span data-ttu-id="c09cb-123">Inclure l'éclatement de la nomenclature : ceci peut attendre juste avant que l'événement approvisionnement soit clôturé.</span><span class="sxs-lookup"><span data-stu-id="c09cb-123">Include BOM explosion: this can wait until just before the supply event is closed.</span></span>  
  
<span data-ttu-id="c09cb-124">Cela conclut les descriptions de la manière dont la demande et l'approvisionnement sont chargés, priorisés et équilibrés par le système de planification.</span><span class="sxs-lookup"><span data-stu-id="c09cb-124">This concludes the descriptions of how demand and supply is loaded, prioritized, and balanced by the planning system.</span></span> <span data-ttu-id="c09cb-125">En association avec cette activité de planification des approvisionnements, le système doit veiller à ce que le niveau de stock requis de chaque article soit maintenu en fonction de ses méthodes de réapprovisionnement.</span><span class="sxs-lookup"><span data-stu-id="c09cb-125">In integration with this supply planning activity, the system must ensure that the required inventory level of each planned item is maintained according to its reordering policies.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="c09cb-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c09cb-126">See Also</span></span>  
<span data-ttu-id="c09cb-127">[Détails de conception : équilibrage de la demande et de l'approvisionnement](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="c09cb-127">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="c09cb-128">[Détails de conception : concepts centraux du système de planification](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="c09cb-128">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="c09cb-129">Détails de conception : planification de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="c09cb-129">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)