---
title: "Détails de conception - Équilibrage de l'approvisionnement avec la demande | Microsoft Docs"
description: "L'élément principal du système de planification implique l'équilibrage de l'approvisionnement et de la demande en proposant des actions utilisateur pour rectifier les commandes approvisionnement en cas de déséquilibre. Cela est opéré par combinaison de variante et magasin."
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
ms.openlocfilehash: 5020c048373f10e72e40f0c9b1e5a11fc45eedb5
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-balancing-supply-with-demand"></a><span data-ttu-id="2c187-104">Détails de conception : équilibrage de l'approvisionnement avec la demande</span><span class="sxs-lookup"><span data-stu-id="2c187-104">Design Details: Balancing Supply with Demand</span></span>
<span data-ttu-id="2c187-105">L'élément principal du système de planification implique l'équilibrage de l'approvisionnement et de la demande en proposant des actions utilisateur pour rectifier les commandes approvisionnement en cas de déséquilibre.</span><span class="sxs-lookup"><span data-stu-id="2c187-105">The core of the planning system involves balancing demand and supply by means of suggesting user actions to revise the supply orders in case of imbalance.</span></span> <span data-ttu-id="2c187-106">Cela est opéré par combinaison de variante et magasin.</span><span class="sxs-lookup"><span data-stu-id="2c187-106">This takes place per combination of variant and location.</span></span>  
  
<span data-ttu-id="2c187-107">Imaginez que chaque profil de stock contient une chaîne d'événements de demande (triés par date et par priorité) et une chaîne correspondante d'événements d'approvisionnement.</span><span class="sxs-lookup"><span data-stu-id="2c187-107">Imagine that each inventory profile contains a string of demand events (sorted by date and priority) and a corresponding string of supply events.</span></span> <span data-ttu-id="2c187-108">Chaque événement fait référence à son type origine et à son identification.</span><span class="sxs-lookup"><span data-stu-id="2c187-108">Each event refers back to its source type and identification.</span></span> <span data-ttu-id="2c187-109">Les règles pour équilibrer l'article sont simples.</span><span class="sxs-lookup"><span data-stu-id="2c187-109">The rules for counterbalancing the item are straightforward.</span></span> <span data-ttu-id="2c187-110">Quatre exemples de correspondance entre demande et approvisionnement peuvent apparaître à tout moment dans le processus :</span><span class="sxs-lookup"><span data-stu-id="2c187-110">Four instances of matching demand and supply can occur at any point of time in the process:</span></span>  
  
1. <span data-ttu-id="2c187-111">Aucune demande ou offre n'existe pour l'article => la planification est terminée (ou ne doit pas démarrer).</span><span class="sxs-lookup"><span data-stu-id="2c187-111">No demand or supply exists for the item => the planning has finished (or should not start).</span></span>  
2. <span data-ttu-id="2c187-112">La demande existe mais il n'y a pas d'offre => une offre doit être proposée.</span><span class="sxs-lookup"><span data-stu-id="2c187-112">Demand exists but there is no supply => supply should be suggested.</span></span>  
3. <span data-ttu-id="2c187-113">L'offre existe mais il n'y a pas de demande correspondante => l'offre doit être annulée.</span><span class="sxs-lookup"><span data-stu-id="2c187-113">Supply exists but there is no demand for it => supply should be canceled.</span></span>  
4. <span data-ttu-id="2c187-114">L'offre et la demande existent => les questions doivent être posées et résolues pour que le système puisse garantir que la demande sera satisfaite et que l'offre est suffisante.</span><span class="sxs-lookup"><span data-stu-id="2c187-114">Both demand and supply exist => questions should be asked and answered before the system can ensure that demand will be met and supply is sufficient.</span></span>  
  
     <span data-ttu-id="2c187-115">Si le délai de l'approvisionnement n'est pas approprié, l'approvisionnement peut être replanifié par exemple comme suit :</span><span class="sxs-lookup"><span data-stu-id="2c187-115">If the timing of the supply is not suitable, perhaps the supply can be rescheduled as follows:</span></span>  
  
    1.  <span data-ttu-id="2c187-116">Si l'approvisionnement est placé avant la demande, l'approvisionnement peut éventuellement être replanifié en sortie pour que le stock soit le plus bas possible.</span><span class="sxs-lookup"><span data-stu-id="2c187-116">If the supply is placed earlier than the demand, perhaps the supply can be rescheduled out so that inventory is as low as possible.</span></span>  
    2.  <span data-ttu-id="2c187-117">Si l'approvisionnement est placé après la demande, l'approvisionnement peut éventuellement être replanifié en entrée.</span><span class="sxs-lookup"><span data-stu-id="2c187-117">If the supply is placed later than the demand, perhaps the supply can be rescheduled in.</span></span> <span data-ttu-id="2c187-118">Sinon, le système suggère un nouvel approvisionnement.</span><span class="sxs-lookup"><span data-stu-id="2c187-118">Otherwise, the system will suggest new supply.</span></span>  
    3.  <span data-ttu-id="2c187-119">Si l'approvisionnement satisfait la demande à la date, le système de planification peut continuer à chercher si la quantité de l'approvisionnement peut couvrir la demande.</span><span class="sxs-lookup"><span data-stu-id="2c187-119">If the supply meets the demand on the date, the planning system can proceed to investigate whether the quantity of the supply can cover the demand.</span></span>  
  
     <span data-ttu-id="2c187-120">Une fois que le délai est en place, la quantité appropriée à approvisionner peut être calculée comme suit :</span><span class="sxs-lookup"><span data-stu-id="2c187-120">Once the timing is in place, the adequate quantity to be supplied can be calculated as follows:</span></span>  
  
    1.  <span data-ttu-id="2c187-121">Si la quantité d'approvisionnement est inférieure à la demande, il est possible que la quantité d'approvisionnement puisse être augmentée (ou pas, si limitée par une stratégie de quantité maximum).</span><span class="sxs-lookup"><span data-stu-id="2c187-121">If the supply quantity is less than the demand, it is possible that the supply quantity could be increased (or not, if limited by a maximum quantity policy).</span></span>  
    2.  <span data-ttu-id="2c187-122">Si la quantité d'approvisionnement est supérieure à la demande, il est possible que la quantité d'approvisionnement puisse être diminuée (ou pas, si limitée par une stratégie de quantité minimum).</span><span class="sxs-lookup"><span data-stu-id="2c187-122">If the supply quantity is greater than the demand, it is possible that the supply quantity can be decreased (or not, if limited by a minimum quantity policy).</span></span>  
  
     <span data-ttu-id="2c187-123">A ce stade, l'une de ces deux situations existe :</span><span class="sxs-lookup"><span data-stu-id="2c187-123">At this point, either of these two situations exists:</span></span>  
  
    1.  <span data-ttu-id="2c187-124">La demande actuelle peut être couverte, dans ce cas, elle peut être clôturée et la planification des demandes suivantes peut commencer.</span><span class="sxs-lookup"><span data-stu-id="2c187-124">The current demand can be covered, in which case it can be closed and planning for the next demand can start.</span></span>  
    2.  <span data-ttu-id="2c187-125">L'approvisionnement a atteint son maximum, en laissant une partie de la quantité de demande non couverte.</span><span class="sxs-lookup"><span data-stu-id="2c187-125">The supply has reached its maximum, leaving some of the demand quantity uncovered.</span></span> <span data-ttu-id="2c187-126">Dans ce cas, le système de planification peut clôturer l'approvisionnement actif et passer au suivant.</span><span class="sxs-lookup"><span data-stu-id="2c187-126">In this case, the planning system can close the current supply and proceed to the next one.</span></span>  
  
 <span data-ttu-id="2c187-127">La procédure recommence à la demande suivante et à l'approvisionnement actif ou vice versa.</span><span class="sxs-lookup"><span data-stu-id="2c187-127">The procedure starts all over with the next demand and the current supply or vice versa.</span></span> <span data-ttu-id="2c187-128">L'approvisionnement actif peut peut-être couvrir cette demande suivante également, ou la demande actuelle n'a pas encore été entièrement couverte.</span><span class="sxs-lookup"><span data-stu-id="2c187-128">The current supply might be able to cover this next demand as well, or the current demand has not yet been fully covered.</span></span>  
  
## <a name="rules-concerning-actions-for-supply-events"></a><span data-ttu-id="2c187-129">Règles en ce qui concerne les actions pour les événements d'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="2c187-129">Rules Concerning Actions for Supply Events</span></span>  
<span data-ttu-id="2c187-130">Lorsque le système de planification effectue un calcul hiérarchisé dans lequel l'approvisionnement doit répondre à la demande, la demande est considérée comme sûr, c'est-à-dire qu'elle se trouve en dehors du contrôle du système de planification.</span><span class="sxs-lookup"><span data-stu-id="2c187-130">When the planning system performs a top-down calculation in which supply must fulfill demand, the demand is taken as a given, that is, it lies outside the control of the planning system.</span></span> <span data-ttu-id="2c187-131">Cependant, le côté approvisionnement peut être géré.</span><span class="sxs-lookup"><span data-stu-id="2c187-131">However, the supply side can be managed.</span></span> <span data-ttu-id="2c187-132">Par conséquent, le système de planification suggère de créer de nouvelles commandes approvisionnement, reprogrammant celles existantes et/ou modifiant la quantité de commande.</span><span class="sxs-lookup"><span data-stu-id="2c187-132">Therefore, the planning system will suggest creating new supply orders, rescheduling existing ones, and/or changing the order quantity.</span></span> <span data-ttu-id="2c187-133">Si une commande approvisionnement existante devient superflue, le système de planification suggère à l'utilisateur de l'annuler.</span><span class="sxs-lookup"><span data-stu-id="2c187-133">If an existing supply order becoming superfluous, the planning system will suggest that the user cancels it.</span></span>  
  
<span data-ttu-id="2c187-134">Si l'utilisateur souhaite exclure une commande approvisionnement existante des propositions planning, il peut déclarer qu'il n'y a pas de flexibilité de planification (flexibilité de planification = Aucune).</span><span class="sxs-lookup"><span data-stu-id="2c187-134">If the user wants to exclude an existing supply order from the planning suggestions, he can state that it has no planning flexibility (Planning Flexibility = None).</span></span> <span data-ttu-id="2c187-135">Ensuite, l'approvisionnement excédentaire à partir de cette commande est utilisé pour répondre à la demande, mais aucune action n'est suggérée.</span><span class="sxs-lookup"><span data-stu-id="2c187-135">Then, excess supply from that order will be used to cover demand, but no action will be suggested.</span></span>  
  
<span data-ttu-id="2c187-136">En général, tous les approvisionnements ont une flexibilité de planification qui est limitée par les conditions de chacune des mesures suggérées.</span><span class="sxs-lookup"><span data-stu-id="2c187-136">In general, all supply has a planning flexibility that is limited by the conditions of each of the suggested actions.</span></span>  
  
-   <span data-ttu-id="2c187-137">**Replanifier en dehors** : La date à partir d'une commande approvisionnement existante peut être planifiée en dehors pour satisfaire la date d'échéance de demande à moins que :</span><span class="sxs-lookup"><span data-stu-id="2c187-137">**Reschedule Out**: The date of an existing supply order can be scheduled out to meet the demand due date unless:</span></span>  
  
    -   <span data-ttu-id="2c187-138">Il représente le stock (toujours au jour zéro).</span><span class="sxs-lookup"><span data-stu-id="2c187-138">It represents inventory (always on day zero).</span></span>  
    -   <span data-ttu-id="2c187-139">Elle a un ordre pour ordre lié à une autre demande.</span><span class="sxs-lookup"><span data-stu-id="2c187-139">It has an order-to-order linked to another demand.</span></span>  
    -   <span data-ttu-id="2c187-140">Il se trouve hors de la fenêtre de replanification définie avant l'intervalle de planification.</span><span class="sxs-lookup"><span data-stu-id="2c187-140">It lies outside the reschedule window defined by the time bucket.</span></span>  
    -   <span data-ttu-id="2c187-141">Il existe un approvisionnement plus proche qui peut être utilisé.</span><span class="sxs-lookup"><span data-stu-id="2c187-141">There is a closer supply that could be used.</span></span>  
    -   <span data-ttu-id="2c187-142">Par ailleurs, l'utilisateur peut choisir de ne pas replanifier pour les raisons suivantes :</span><span class="sxs-lookup"><span data-stu-id="2c187-142">On the other hand, the user may decide not to reschedule because:</span></span>  
    -   <span data-ttu-id="2c187-143">La commande approvisionnement a déjà été liée à une autre demande à une date précédente.</span><span class="sxs-lookup"><span data-stu-id="2c187-143">The supply order has already been tied to another demand on a previous date.</span></span>  
    -   <span data-ttu-id="2c187-144">La replanification nécessaire est si minime que l'utilisateur la trouve négligeable.</span><span class="sxs-lookup"><span data-stu-id="2c187-144">The needed rescheduling is so minimal that the user finds it negligible.</span></span>  
  
-   <span data-ttu-id="2c187-145">**Replanifier dans** : La date à partir d'une commande approvisionnement existante peut être replanifiée dans, sauf dans les conditions suivantes :</span><span class="sxs-lookup"><span data-stu-id="2c187-145">**Reschedule In**: The date of an existing supply order can be scheduled in, except in the following conditions:</span></span>  
  
    -   <span data-ttu-id="2c187-146">Elle est directement liée à une autre demande.</span><span class="sxs-lookup"><span data-stu-id="2c187-146">It is linked directly to some other demand.</span></span>  
    -   <span data-ttu-id="2c187-147">Il se trouve hors de la fenêtre de replanification définie avant l'intervalle de planification.</span><span class="sxs-lookup"><span data-stu-id="2c187-147">It lies outside the reschedule window defined by the time bucket.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="2c187-148">Lors de la planification d'un article utilisant un point de commande, la commande approvisionnement peut toujours être planifiée si nécessaire.</span><span class="sxs-lookup"><span data-stu-id="2c187-148">When planning an item using a reorder point, the supply order can always be scheduled in if necessary.</span></span> <span data-ttu-id="2c187-149">Ceci est courant dans les commandes approvisionnement planifiées déclenchées par un point de commande.</span><span class="sxs-lookup"><span data-stu-id="2c187-149">This is common in forward-scheduled supply orders triggered by a reorder point.</span></span>  
  
-   <span data-ttu-id="2c187-150">**Augmenter la quantité** : il est possible d'augmenter la quantité d'une commande approvisionnement existante pour répondre à la demande sauf si la commande approvisionnement est directement liée à une demande par un lien ordre pour ordre.</span><span class="sxs-lookup"><span data-stu-id="2c187-150">**Increase Quantity**: The quantity of an existing supply order can be increased to meet the demand unless the supply order is linked directly to a demand by an order-to-order link.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="2c187-151">Bien qu'il soit possible d'augmenter la commande approvisionnement, elle peut être limité en raison d'une quantité maximum commande définie par l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2c187-151">Even though it is possible to increase the supply order, it may be limited due to a defined maximum order quantity.</span></span>  
  
-   <span data-ttu-id="2c187-152">**Diminuer la quantité** : une commande approvisionnement existante avec un excédent par rapport à la demande existante peut être diminuée pour répondre à la demande.</span><span class="sxs-lookup"><span data-stu-id="2c187-152">**Decrease Quantity**: An existing supply order with a surplus compared to an existing demand can be decreased to meet the demand.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="2c187-153">Bien que la quantité puisse être diminuée, il peut y avoir encore des excédents par rapport à la demande en raison d'une quantité minimum commande définie ou d'une valeur Commandé par.</span><span class="sxs-lookup"><span data-stu-id="2c187-153">Even though the quantity could be decreased, there may still be some surplus compared to the demand due to a defined minimum order quantity or order multiple.</span></span>  
  
-   <span data-ttu-id="2c187-154">**Annuler** : comme un incident spécial de l'action de diminuer la quantité, la commande approvisionnement peut être annulée si elle a été diminuée à zéro.</span><span class="sxs-lookup"><span data-stu-id="2c187-154">**Cancel**: As a special incident of the decrease quantity action, the supply order could be canceled if it has been decreased to zero.</span></span>  
-   <span data-ttu-id="2c187-155">**Nouveau** : si aucune commande approvisionnement n'existe déjà, ou si une existante ne peut pas être modifiée pour satisfaire la quantité nécessaire à la date d'échéance demandée, une nouvelle commande approvisionnement est suggérée.</span><span class="sxs-lookup"><span data-stu-id="2c187-155">**New**: If no supply order already exists, or an existing one cannot be changed to meet the necessary quantity on the demanded due date, a new supply order is suggested.</span></span>  
  
## <a name="determining-the-supply-quantity"></a><span data-ttu-id="2c187-156">Déterminer la quantité d'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="2c187-156">Determining the Supply Quantity</span></span>  
<span data-ttu-id="2c187-157">Les paramètres de planification définis par l'utilisateur contrôlent la quantité suggérée de chaque commande approvisionnement.</span><span class="sxs-lookup"><span data-stu-id="2c187-157">Planning parameters defined by the user control the suggested quantity of each supply order.</span></span>  
  
<span data-ttu-id="2c187-158">Lorsque le système de planification calcule la quantité d'une nouvelle commande approvisionnement ou la modification de quantité d'une commande existante, la quantité proposée n'est pas forcément identique à ce qui est vraiment demandé.</span><span class="sxs-lookup"><span data-stu-id="2c187-158">When the planning system calculates the quantity of a new supply order or the quantity change on an existing one, the suggested quantity may be different from what is actually demanded.</span></span>  
  
<span data-ttu-id="2c187-159">Si un stock maximum ou une quantité de commande fixe sont sélectionnés, la quantité proposée peut être augmentée pour répondre à cette quantité fixe ou au stock maximum.</span><span class="sxs-lookup"><span data-stu-id="2c187-159">If a maximum inventory or fixed order quantity are selected, the suggested quantity may be increased to meet that fixed quantity or the maximum inventory.</span></span> <span data-ttu-id="2c187-160">Si une méthode de réapprovisionnement utilise un point de commande, la quantité peut être augmentée au moins pour répondre au point de commande.</span><span class="sxs-lookup"><span data-stu-id="2c187-160">If a reordering policy uses a reorder point, the quantity may be increased at least to meet the reorder point.</span></span>  
  
 <span data-ttu-id="2c187-161">La quantité proposée peut être modifiée dans cette séquence :</span><span class="sxs-lookup"><span data-stu-id="2c187-161">The suggested quantity may be modified in this sequence:</span></span>  
  
1. <span data-ttu-id="2c187-162">Diminuer à la quantité maximum commande (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="2c187-162">Down to the maximum order quantity (if any).</span></span>  
2. <span data-ttu-id="2c187-163">Jusqu'à la quantité de commande minimale.</span><span class="sxs-lookup"><span data-stu-id="2c187-163">Up to the minimum order quantity.</span></span>  
3. <span data-ttu-id="2c187-164">Jusqu'à répondre à la commande multiple la plus proche.</span><span class="sxs-lookup"><span data-stu-id="2c187-164">Up to meet the nearest order multiple.</span></span> <span data-ttu-id="2c187-165">(Si des paramètres sont erronés, cela peut enfreindre la quantité de commande maximale).</span><span class="sxs-lookup"><span data-stu-id="2c187-165">(In case of erroneous settings, this may violate the maximum order quantity.)</span></span>  
  
## <a name="order-tracking-links-during-planning"></a><span data-ttu-id="2c187-166">Liens de chaînage lors de la planification</span><span class="sxs-lookup"><span data-stu-id="2c187-166">Order Tracking Links during Planning</span></span>  
<span data-ttu-id="2c187-167">En ce qui concerne le chaînage lors de la planification, il est important de mentionner que le système de planification réarrange les liens de chaînage créés de façon dynamique pour les combinaisons de article/variante/magasin.</span><span class="sxs-lookup"><span data-stu-id="2c187-167">Concerning order tracking during planning, it is important to mention that the planning system rearranges the dynamically created order tracking links for the item/variant/location combinations.</span></span>  
  
<span data-ttu-id="2c187-168">Deux raisons expliquent cela :</span><span class="sxs-lookup"><span data-stu-id="2c187-168">There are two reasons for this:</span></span>  
  
-   <span data-ttu-id="2c187-169">Le système de planification doit pouvoir justifier ses propositions ; que toute demande a été couverte, et qu'aucune commande approvisionnement n'est superflue.</span><span class="sxs-lookup"><span data-stu-id="2c187-169">The planning system must be able to justify its suggestions; that all demand has been covered, and that no supply orders are superfluous.</span></span>  
-   <span data-ttu-id="2c187-170">Les liens de chaînage créés de façon dynamique doivent être rééquilibrés régulièrement.</span><span class="sxs-lookup"><span data-stu-id="2c187-170">Dynamically created order tracking links need to be rebalanced regularly.</span></span>  
  
<span data-ttu-id="2c187-171">Avec le temps, les liens de chaînage dynamiques deviennent déséquilibrés puisque le réseau de chaînage entier n'est pas réorganisé tant qu'un événement de demande ou d'approvisionnement n'est pas réellement clôturé.</span><span class="sxs-lookup"><span data-stu-id="2c187-171">Over time, dynamic order tracking links become out of balance since the entire order tracking network is not rearranged until a demand or supply event is actually closed.</span></span>  
  
<span data-ttu-id="2c187-172">Avant d'équilibrer un approvisionnement par demande, le programme supprime les liens de chaînage existants.</span><span class="sxs-lookup"><span data-stu-id="2c187-172">Before balancing supply by demand, the program deletes all existing order tracking links.</span></span> <span data-ttu-id="2c187-173">Puis au cours de la procédure de contrepartie, lorsqu'un événement de demande ou d'approvisionnement est clôturé, il crée de nouveaux liens de suivi de commande entre la demande et l'approvisionnement.</span><span class="sxs-lookup"><span data-stu-id="2c187-173">Then during the balancing procedure, when a demand or supply event is closed, it establishes new order tracking links between the demand and supply.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="2c187-174">Même si l'article n'est pas configuré pour le chaînage dynamique, le système planifié crée des liens de chaînage équilibrés comme expliqué ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="2c187-174">Even if the item is not set up for dynamic order tracking, the planned system will create balanced order tracking links as explained above.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="2c187-175">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2c187-175">See Also</span></span>  
<span data-ttu-id="2c187-176">[Détails de conception : équilibrage de la demande et de l'approvisionnement](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="2c187-176">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="2c187-177">[Détails de conception : concepts centraux du système de planification](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="2c187-177">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="2c187-178">Détails de conception : planification de l'approvisionnement</span><span class="sxs-lookup"><span data-stu-id="2c187-178">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)