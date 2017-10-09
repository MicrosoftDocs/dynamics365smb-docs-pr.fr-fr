---
title: "Détails de conception - Lot pour lot | Microsoft Docs"
description: "Découvrez comment utiliser la méthode lot pour lot pour déterminer la quantité de commande en fonction de la demande."
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
ms.openlocfilehash: 2e0d1d18685f3395c31071ca9a2495c0091c564d
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-lot-for-lot"></a><span data-ttu-id="532b7-103">Détails de conception : lot pour lot</span><span class="sxs-lookup"><span data-stu-id="532b7-103">Design Details: Lot-for-Lot</span></span>
<span data-ttu-id="532b7-104">La méthode lot pour lot est la plus souple, parce que le système réagit uniquement à la demande réelle, de plus il agit sur une demande anticipée à partir de commandes de prévision et de commandes ouvertes, puis détermine la quantité commande en fonction de la demande.</span><span class="sxs-lookup"><span data-stu-id="532b7-104">The lot-for-lot policy is the most flexible because the system only reacts on actual demand, plus it acts on anticipated demand from forecast and blanket orders and then settles the order quantity based on the demand.</span></span> <span data-ttu-id="532b7-105">La méthode lot pour lot visé cible les articles A et B pour lesquels le stock peut être accepté mais doit être évité.</span><span class="sxs-lookup"><span data-stu-id="532b7-105">The lot-for-lot policy is aimed at A- and B-items where inventory can be accepted but should be avoided.</span></span>  
  
<span data-ttu-id="532b7-106">Par certains côtés, la méthode lot pour lot ressemble à la méthode de commande, mais elle a une approche générique des articles ; elle peut accepter des quantités en stock, et elle groupe une demande et un approvisionnement correspondants dans des intervalles de planification définis par l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="532b7-106">In some ways, the lot-for-lot policy looks like the Order policy, but it has a generic approach to items; it can accept quantities in inventory, and it bundles demand and corresponding supply in time buckets defined by the user.</span></span>  
  
<span data-ttu-id="532b7-107">L'intervalle de planification est défini dans le champ **Intervalle de planification**.</span><span class="sxs-lookup"><span data-stu-id="532b7-107">The time bucket is defined in the **Time Bucket** field.</span></span> <span data-ttu-id="532b7-108">Le système travaille avec un intervalle de planification minimum d'un jour, car il s'agit de la plus petite unité de temps des événements de demande et d'approvisionnement dans le système (même si, dans la pratique, l'unité de temps des ordres de fabrication et des besoins de composants peuvent être des secondes).</span><span class="sxs-lookup"><span data-stu-id="532b7-108">The system works with a minimum time bucket of one day, since this is the smallest time unit of measure on demand and supply events in the system (although, in practice, the time unit of measure on production orders and component needs can be seconds).</span></span>  
  
<span data-ttu-id="532b7-109">L'intervalle de planification fixe également des limites lorsque un ordre de fabrication existant doit être replanifié pour répondre à une demande donnée.</span><span class="sxs-lookup"><span data-stu-id="532b7-109">The time bucket also sets limits on when an existing supply order should be rescheduled to meet a given demand.</span></span> <span data-ttu-id="532b7-110">Si l'approvisionnement se trouve dans l'intervalle de planification, il est replanifié en entrée ou en sortie pour répondre à la demande.</span><span class="sxs-lookup"><span data-stu-id="532b7-110">If the supply lies within the time bucket, it will be rescheduled in or out to meet the demand.</span></span> <span data-ttu-id="532b7-111">Sinon, s'il a lieu précédemment, il provoque une accumulation de stock inutile et doit être annulé.</span><span class="sxs-lookup"><span data-stu-id="532b7-111">Otherwise, if it lies earlier, it will cause unnecessary build-up of inventory and should be canceled.</span></span> <span data-ttu-id="532b7-112">S'il se trouve plus tard, une commande approvisionnement est créée à la place.</span><span class="sxs-lookup"><span data-stu-id="532b7-112">If it lies later, a new supply order will be created instead.</span></span>  
  
<span data-ttu-id="532b7-113">Avec cette méthode, il est également possible de définir un stock de sécurité pour compenser les fluctuations possibles de l'approvisionnement, ou répondre à une demande soudaine.</span><span class="sxs-lookup"><span data-stu-id="532b7-113">With this policy, it is also possible to define a safety stock in order to compensate for possible fluctuations in supply, or to meet sudden demand.</span></span>  
  
<span data-ttu-id="532b7-114">Étant donné que la quantité de commande approvisionnement est basée sur la demande réelle, il peut sembler raisonnable d'utiliser les modificateurs de commande : arrondir la quantité commandée pour répondre à un multiple spécifié de la commande (ou unité d'achat), augmenter la commande à une quantité de commande minimale spécifiée, ou réduire la quantité à la quantité maximale spécifiée (et ainsi créer deux ou plusieurs approvisionnements pour répondre à la quantité nécessaire totale).</span><span class="sxs-lookup"><span data-stu-id="532b7-114">Because the supply order quantity is based on the actual demand it can make sense to use the order modifiers: round the order quantity up to meet a specified order multiple (or purchase unit of measure), increase the order to a specified minimum order quantity, or decrease the quantity to the specified maximum quantity (and thus create two or more supplies to reach the total needed quantity).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="532b7-115">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="532b7-115">See Also</span></span>  
<span data-ttu-id="532b7-116">[Détails de conception : méthodes de réapprovisionnement](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="532b7-116">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="532b7-117">[Détails de conception : paramètres de planification](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="532b7-117">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="532b7-118">[Détails de conception : gestion des méthodes de réapprovisionnement](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="532b7-118">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="532b7-119">Détails de conception : planification de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="532b7-119">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)