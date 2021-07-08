---
title: États et analyses des achats
description: Découvrez les états et analyses des achats disponibles dans la version standard de Business Central afin que vous puissiez suivre votre activité.
author: AndreiPanko
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 06/01/2021
ms.author: andreipa
ms.openlocfilehash: 5fc64db4120b80203f99742ed3ed834b23370c47
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/09/2021
ms.locfileid: "6216357"
---
# <a name="purchase-reports-and-analytics-in-business-central"></a><span data-ttu-id="10c91-103">États et analyses des achats dans Business Central</span><span class="sxs-lookup"><span data-stu-id="10c91-103">Purchase Reports and Analytics in Business Central</span></span>

<span data-ttu-id="10c91-104">Les états des achats dans [!INCLUDE [prod_short](includes/prod_short.md)] permettent aux professionnels de l’approvisionnement et des affaires d’obtenir des informations et des statistiques sur les activités d’achat actuelles et passées.</span><span class="sxs-lookup"><span data-stu-id="10c91-104">Purchase reporting in [!INCLUDE [prod_short](includes/prod_short.md)] allows procurement and business professionals to get insights and statistics about current and past purchase activities.</span></span>  

## <a name="reports"></a><span data-ttu-id="10c91-105">États</span><span class="sxs-lookup"><span data-stu-id="10c91-105">Reports</span></span>

<span data-ttu-id="10c91-106">Le tableau suivant décrit certains des principaux états dans les états des achats.</span><span class="sxs-lookup"><span data-stu-id="10c91-106">The following table describes some of the key reports in purchase reporting.</span></span>

|<span data-ttu-id="10c91-107">État</span><span class="sxs-lookup"><span data-stu-id="10c91-107">Report</span></span> |<span data-ttu-id="10c91-108">ID d’objet</span><span class="sxs-lookup"><span data-stu-id="10c91-108">Object ID</span></span>|<span data-ttu-id="10c91-109">Description</span><span class="sxs-lookup"><span data-stu-id="10c91-109">Description</span></span>  |
|---------|---------|---------|
|<span data-ttu-id="10c91-110">**Statistique achat**</span><span class="sxs-lookup"><span data-stu-id="10c91-110">**Purchase statistic**</span></span>|<span data-ttu-id="10c91-111">312</span><span class="sxs-lookup"><span data-stu-id="10c91-111">312</span></span>|<span data-ttu-id="10c91-112">Affiche les statistiques achat pour chaque fournisseur.</span><span class="sxs-lookup"><span data-stu-id="10c91-112">Shows purchase statistics for each vendor.</span></span> <span data-ttu-id="10c91-113">Cela inclut des informations pour cinq périodes, à partir de la date que vous spécifiez.</span><span class="sxs-lookup"><span data-stu-id="10c91-113">This includes information for five periods, starting on the date that you specify.</span></span><br>
<span data-ttu-id="10c91-114">L’état comprend les informations concernant le total des achats, les paiements, les frais financiers et les remises, y compris les escomptes gagnés et perdus.</span><span class="sxs-lookup"><span data-stu-id="10c91-114">The report includes the total purchases, payments, finance charges, and discount information including the payment discounts taken and lost.</span></span> <span data-ttu-id="10c91-115">Les statistiques sont calculées pour les achats antérieurs à la date saisie, trois fois à un mois d’intervalle à compter de la date saisie et pour une période incluant tous les achats effectués après le troisième intervalle d’un mois.</span><span class="sxs-lookup"><span data-stu-id="10c91-115">Statistics are calculated for purchases before the date entered, at three one-month intervals from the date entered, and for a period including all purchases made after the third one-month interval.</span></span>|
|<span data-ttu-id="10c91-116">**Fournisseur – Liste des 10 meilleurs**</span><span class="sxs-lookup"><span data-stu-id="10c91-116">**Vendor – Top 10 list**</span></span>|<span data-ttu-id="10c91-117">311</span><span class="sxs-lookup"><span data-stu-id="10c91-117">311</span></span>|<span data-ttu-id="10c91-118">Affiche des informations sur les achats aux fournisseurs pour une période déterminée.</span><span class="sxs-lookup"><span data-stu-id="10c91-118">Shows information on purchases from vendors for a selected period.</span></span> <span data-ttu-id="10c91-119">Vous pouvez choisir le nombre de fournisseurs inclus dans l’état.</span><span class="sxs-lookup"><span data-stu-id="10c91-119">You can choose the number of vendors that are included in the report.</span></span><br><span data-ttu-id="10c91-120">Les fournisseurs sont triés par montant, et vous pouvez choisir s’ils doivent être triés par montant d’achat ou par solde.</span><span class="sxs-lookup"><span data-stu-id="10c91-120">The vendors are sorted in order of amount, and you can choose whether they are sorted by purchase amount or balance.</span></span> <span data-ttu-id="10c91-121">L’état vous donne un bref aperçu des fournisseurs à qui vous achetez le plus et ceux à qui vous devez le plus d’argent.</span><span class="sxs-lookup"><span data-stu-id="10c91-121">The report gives a quick overview of the vendors from which you purchase the most or to which you owe the most.</span></span>|
|<span data-ttu-id="10c91-122">**Catalogue article fournisseur** ou **Catalogue fournisseur/article**</span><span class="sxs-lookup"><span data-stu-id="10c91-122">**Vendor Item catalog** or **Item/vendor catalog**</span></span>|<span data-ttu-id="10c91-123">320 ou 720</span><span class="sxs-lookup"><span data-stu-id="10c91-123">320 or 720</span></span>|<span data-ttu-id="10c91-124">Affiche une liste des fournisseurs pour les articles sélectionnés ou des articles pour les fournisseurs sélectionnés.</span><span class="sxs-lookup"><span data-stu-id="10c91-124">Displays a list of the vendors for the selected items or items for selected vendors.</span></span> <span data-ttu-id="10c91-125">Pour chaque combinaison d’article et de fournisseur, l’état indique le coût unitaire direct, le délai de réapprovisionnement et la référence fournisseur.</span><span class="sxs-lookup"><span data-stu-id="10c91-125">For each combination of item and vendor, it shows direct unit cost, lead time calculation and the vendor's item number.</span></span><br><span data-ttu-id="10c91-126">Cet état n’est pas disponible aux États-Unis, au Canada et au Mexique.</span><span class="sxs-lookup"><span data-stu-id="10c91-126">In the US, Canada, and Mexico, this report is not available.</span></span> <span data-ttu-id="10c91-127">Utilisez plutôt l’état **Catalogue Article/Fournisseur** (10164).</span><span class="sxs-lookup"><span data-stu-id="10c91-127">Instead, use the **Item/Vendor Catalog** (10164) report.</span></span>|
|<span data-ttu-id="10c91-128">**Achats Fournisseur/Article**</span><span class="sxs-lookup"><span data-stu-id="10c91-128">**Vendor/Item Purchases**</span></span>|<span data-ttu-id="10c91-129">313</span><span class="sxs-lookup"><span data-stu-id="10c91-129">313</span></span>|<span data-ttu-id="10c91-130">Affiche la liste des écritures article de chaque fournisseur pendant la période choisie.</span><span class="sxs-lookup"><span data-stu-id="10c91-130">Shows a list of item entries for each vendor in a selected period.</span></span> <span data-ttu-id="10c91-131">L’état affiche des informations sur la quantité facturée, le montant et les remises possibles.</span><span class="sxs-lookup"><span data-stu-id="10c91-131">The report contains information on invoiced quantity, amount and possible discounts.</span></span> <span data-ttu-id="10c91-132">Il peut être utilisé, par exemple, pour analyser les achats d’articles d’une société et pour voir s’il existe une relation entre les remises et les achats d’articles.</span><span class="sxs-lookup"><span data-stu-id="10c91-132">It can be used, for example, to analyze a company's item purchases and to show whether there is a relationship between discounts and item purchases.</span></span>|
|<span data-ttu-id="10c91-133">**Liste prix et coûts stocks**</span><span class="sxs-lookup"><span data-stu-id="10c91-133">**Inventory Cost and price list**</span></span>|<span data-ttu-id="10c91-134">716</span><span class="sxs-lookup"><span data-stu-id="10c91-134">716</span></span>|<span data-ttu-id="10c91-135">Affiche la liste d’informations sur les prix des articles sélectionnés ou des points de stock : coût unitaire direct, dernier coût direct, prix unitaire, pourcentage de marge et marge.</span><span class="sxs-lookup"><span data-stu-id="10c91-135">Displays a list of price information for the selected items or stockkeeping units: direct unit cost, last direct cost, unit price, profit percentage, and profit.</span></span>|
|<span data-ttu-id="10c91-136">**Échéancier des dispo. de stock**</span><span class="sxs-lookup"><span data-stu-id="10c91-136">**Inventory Availability Plan**</span></span>|<span data-ttu-id="10c91-137">707</span><span class="sxs-lookup"><span data-stu-id="10c91-137">707</span></span>|<span data-ttu-id="10c91-138">Si vous souhaitez avoir un aperçu d’articles/de points de stock spécifiques et de leur disponibilité.</span><span class="sxs-lookup"><span data-stu-id="10c91-138">If you would like to have an overview about specific items/stockkeeping units and their availability.</span></span> <span data-ttu-id="10c91-139">Cet état affichera des valeurs cumulées telles que les besoins bruts, les réceptions planifiées et prévues, le stock, etc.</span><span class="sxs-lookup"><span data-stu-id="10c91-139">This report will show you cumulated values such as gross requirements, scheduled and planned receipts, the inventory, and so on.</span></span> |
|<span data-ttu-id="10c91-140">**Achats fournisseur stock**</span><span class="sxs-lookup"><span data-stu-id="10c91-140">**Inventory Vendor Purchases**</span></span>|<span data-ttu-id="10c91-141">714</span><span class="sxs-lookup"><span data-stu-id="10c91-141">714</span></span>|<span data-ttu-id="10c91-142">Affiche la liste des fournisseurs auxquels votre société a acheté des articles dans la période sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="10c91-142">Displays a list of the vendors that your company has purchased items from within a selected period.</span></span> <span data-ttu-id="10c91-143">Il indique la quantité facturée, le montant et la remise.</span><span class="sxs-lookup"><span data-stu-id="10c91-143">It shows invoiced quantity, amount and discount.</span></span> <span data-ttu-id="10c91-144">L’état peut être utilisé pour analyser les achats de la société.</span><span class="sxs-lookup"><span data-stu-id="10c91-144">The report can be used to analyze a company's item purchases.</span></span>|
|<span data-ttu-id="10c91-145">**Commandes achat de stock**</span><span class="sxs-lookup"><span data-stu-id="10c91-145">**Inventory Purchase Orders**</span></span>|<span data-ttu-id="10c91-146">709</span><span class="sxs-lookup"><span data-stu-id="10c91-146">709</span></span>|<span data-ttu-id="10c91-147">Affiche la liste des articles commandés chez les fournisseurs.</span><span class="sxs-lookup"><span data-stu-id="10c91-147">Displays a list of items on order from vendors.</span></span> <span data-ttu-id="10c91-148">Il indique aussi la date de réception prévue, la quantité et le montant des commandes en souffrance.</span><span class="sxs-lookup"><span data-stu-id="10c91-148">It also shows the expected receipt date and the quantity and amount on back orders.</span></span> <span data-ttu-id="10c91-149">Par exemple, utilisez l’état pour visualiser le moment où les articles doivent être réceptionnés et si un rappel de commande en souffrance doit être émis.</span><span class="sxs-lookup"><span data-stu-id="10c91-149">For example, use the report to see when items should be received, and whether a reminder of a back order should be issued</span></span>|
|<span data-ttu-id="10c91-150">**Disponibilité réservation achat**</span><span class="sxs-lookup"><span data-stu-id="10c91-150">**Purchase Reservation Availability**</span></span>|<span data-ttu-id="10c91-151">409</span><span class="sxs-lookup"><span data-stu-id="10c91-151">409</span></span>|<span data-ttu-id="10c91-152">Affiche la disponibilité des articles pour les livraisons effectuées à partir de documents achat, par exemple les retours.</span><span class="sxs-lookup"><span data-stu-id="10c91-152">Shows the availability of items for shipment on purchase documents, for example return orders.</span></span> <span data-ttu-id="10c91-153">Vous déterminez si l’état indique le statut de chaque document ou de chaque ligne achat.</span><span class="sxs-lookup"><span data-stu-id="10c91-153">You determine whether the report indicates the status of each document or of each purchase line.</span></span> <br><span data-ttu-id="10c91-154">Lorsque vous imprimez l’état, vous pouvez également mettre à jour les quantités disponibles pour livraison dans le champ **Quantité à recevoir** des lignes achat.</span><span class="sxs-lookup"><span data-stu-id="10c91-154">When you print the report, you can also update the quantity that is available for shipment in the **Qty. to Receive** field on the purchase lines.</span></span> <span data-ttu-id="10c91-155">Sur les avoirs achat et les lignes commande achat négative, le champ **Quantité à recevoir** indique la quantité à livrer.</span><span class="sxs-lookup"><span data-stu-id="10c91-155">On purchase credit memos and negative purchase order lines, the **Qty. to Receive** field contains the quantity to ship..</span></span> <span data-ttu-id="10c91-156">Vous pouvez alors utiliser cet état pour déterminer les documents à valider.</span><span class="sxs-lookup"><span data-stu-id="10c91-156">Then you can use the report to determine which documents to ship.</span></span> <span data-ttu-id="10c91-157">**Remarque** : cet état n’est pas disponible pour les fonctionnalités d’entrepôt avancées.</span><span class="sxs-lookup"><span data-stu-id="10c91-157">**Note**: This report is not available for advanced warehouse functionality.</span></span>|
<span data-ttu-id="10c91-158"><!--</span><span class="sxs-lookup"><span data-stu-id="10c91-158"><!--</span></span>|<span data-ttu-id="10c91-159">**Fournisseur - Écritures échues**</span><span class="sxs-lookup"><span data-stu-id="10c91-159">**Vendor detailed aging**</span></span>|<span data-ttu-id="10c91-160">11006</span><span class="sxs-lookup"><span data-stu-id="10c91-160">11006</span></span>| <span data-ttu-id="10c91-161">Spécifique à DACH : état qui pourrait être utilisé par le chef d’équipe de votre département d’achat ainsi que par la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="10c91-161">DACH specific: A report which could be used by the team leader of your purchased department as will the accounting.</span></span> <span data-ttu-id="10c91-162">Vous aurez ici un aperçu des factures fournisseurs impayées, y compris les dates d’échéance, les devises et les montants.</span><span class="sxs-lookup"><span data-stu-id="10c91-162">Here you will have an overview about the unpaid vendor invoices including the due dates, currencies and amounts.</span></span> <span data-ttu-id="10c91-163">La base est constituée des écritures comptables fournisseur ouvertes.</span><span class="sxs-lookup"><span data-stu-id="10c91-163">Basis is the open vendor ledger entries.</span></span>| -->




## <a name="tasks"></a><span data-ttu-id="10c91-164">Tâches</span><span class="sxs-lookup"><span data-stu-id="10c91-164">Tasks</span></span>

<span data-ttu-id="10c91-165">Les articles suivants décrivent certaines des tâches clés pour analyser l’état de votre entreprise :</span><span class="sxs-lookup"><span data-stu-id="10c91-165">The following articles describe some of the key tasks for analyzing the state of your business:</span></span>

* [<span data-ttu-id="10c91-166">Créer des rapports d’analyse</span><span class="sxs-lookup"><span data-stu-id="10c91-166">Create Analysis Reports</span></span>](bi-how-create-analysis-views-reports.md)  
* [<span data-ttu-id="10c91-167">Voir la disponibilité des articles</span><span class="sxs-lookup"><span data-stu-id="10c91-167">View the Availability of Items</span></span>](inventory-how-availability-overview.md)  


## <a name="see-also"></a><span data-ttu-id="10c91-168">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="10c91-168">See also</span></span>

[<span data-ttu-id="10c91-169">Définition des achats</span><span class="sxs-lookup"><span data-stu-id="10c91-169">Setting Up Purchase</span></span>](purchasing-setup-purchasing.md)  
[<span data-ttu-id="10c91-170">Achats</span><span class="sxs-lookup"><span data-stu-id="10c91-170">Purchasing</span></span>](purchasing-manage-purchasing.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]