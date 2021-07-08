---
title: États et analyses de production
description: Découvrez les états et analyses de production disponibles dans la version standard de Business Central afin que vous puissiez suivre votre activité.
author: AndreiPanko
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 06/01/2021
ms.author: andreipa
ms.openlocfilehash: 0cacf41f0a055267af5b0ce5a8b68b34d86a1cb5
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/09/2021
ms.locfileid: "6216354"
---
# <a name="production-reports-and-analytics-in-business-central"></a><span data-ttu-id="7b703-103">États et analyses de production dans Business Central</span><span class="sxs-lookup"><span data-stu-id="7b703-103">Production Reports and Analytics in Business Central</span></span>

<span data-ttu-id="7b703-104">Les états de production dans [!INCLUDE [prod_short](includes/prod_short.md)] permettent aux professionnels de la production et des affaires d’obtenir des informations et des statistiques sur les activités de production actuelles et passées.</span><span class="sxs-lookup"><span data-stu-id="7b703-104">Production reporting in [!INCLUDE [prod_short](includes/prod_short.md)] allows production and business professionals to get insights and statistics about current and past production activities.</span></span>  

## <a name="reports"></a><span data-ttu-id="7b703-105">États</span><span class="sxs-lookup"><span data-stu-id="7b703-105">Reports</span></span>

<span data-ttu-id="7b703-106">Le tableau suivant décrit certains des principaux états dans les états de production.</span><span class="sxs-lookup"><span data-stu-id="7b703-106">The following table describes some of the key reports in production reporting.</span></span>

|<span data-ttu-id="7b703-107">État</span><span class="sxs-lookup"><span data-stu-id="7b703-107">Report</span></span> |<span data-ttu-id="7b703-108">ID d’objet</span><span class="sxs-lookup"><span data-stu-id="7b703-108">Object ID</span></span>|<span data-ttu-id="7b703-109">Description</span><span class="sxs-lookup"><span data-stu-id="7b703-109">Description</span></span>  |
|---------|---------|---------|
|<span data-ttu-id="7b703-110">**Nomenclature multi-niveau**</span><span class="sxs-lookup"><span data-stu-id="7b703-110">**Quantity Explosion of BOM**</span></span>|<span data-ttu-id="7b703-111">99000753</span><span class="sxs-lookup"><span data-stu-id="7b703-111">99000753</span></span>|<span data-ttu-id="7b703-112">Affiche la liste des nomenclatures multi-niveaux pour l’article ou les articles que vous définissez dans les filtres.</span><span class="sxs-lookup"><span data-stu-id="7b703-112">Shows an indented BOM listing for the item or items that you specify in the filters.</span></span> <span data-ttu-id="7b703-113">La nomenclature de production est entièrement éclatée pour tous les niveaux.</span><span class="sxs-lookup"><span data-stu-id="7b703-113">The production BOM is completely exploded for all levels.</span></span>|
|<span data-ttu-id="7b703-114">**Article – Capable de fabriquer (Temps)**</span><span class="sxs-lookup"><span data-stu-id="7b703-114">**Item – Able to Make (Time)**</span></span>|<span data-ttu-id="7b703-115">5871</span><span class="sxs-lookup"><span data-stu-id="7b703-115">5871</span></span>|<span data-ttu-id="7b703-116">Indique comment cinq chiffres de disponibilité principaux différents évoluent dans le temps pour un article de nomenclature.</span><span class="sxs-lookup"><span data-stu-id="7b703-116">Shows how five different key availability figures change over time for a BOM item.</span></span> <span data-ttu-id="7b703-117">Ces chiffres sont modifiés en fonction des événements d’offre et de demande prévus et de l’approvisionnement qui est basé sur les composants disponibles qui peuvent être assemblés ou produits.</span><span class="sxs-lookup"><span data-stu-id="7b703-117">These figures change according to expected supply and demand events and to supply that is based on available components that can be assembled or produced.</span></span><br><span data-ttu-id="7b703-118">Vous pouvez utiliser l’état pour vérifier si vous pouvez traiter une commande vente d’un article à une date spécifique, en consultant sa disponibilité actuelle ainsi que les quantités potentielles que ses composants peuvent fournir si un ordre d’assemblage a été lancé.</span><span class="sxs-lookup"><span data-stu-id="7b703-118">You can use the report to see whether you can fulfill a sales order for an item on a specified date by looking at its current availability in combination with the potential quantities that its components can supply if an assembly order has been started.</span></span> <span data-ttu-id="7b703-119">L’état indique la date et le nombre d’unités d’un élément d’assemblage et de production que vous pouvez fabriquer, en fonction de la disponibilité des composants et de la disponibilité actuelle de l’article.</span><span class="sxs-lookup"><span data-stu-id="7b703-119">The report shows you when and how many units of an assembly and production item you can make based on component availability and the item's current availability.</span></span> <span data-ttu-id="7b703-120">Cela est affiché en tant que quantité totale.</span><span class="sxs-lookup"><span data-stu-id="7b703-120">This is shown as the total quantity.</span></span><br><span data-ttu-id="7b703-121">Les informations sont affichées dans un graphique dans lequel chaque chiffre de disponibilité est une ligne qui progresse dans la chronologie et se déplace vers le haut ou vers le bas en fonction des modifications des quantités.</span><span class="sxs-lookup"><span data-stu-id="7b703-121">The information is shown in a graph where each availability figure is a line that progresses along the timeline and moves up and down as quantities change.</span></span> <span data-ttu-id="7b703-122">Les chiffres de quantité proviennent du même moteur qui fournit des informations dans la fenêtre **Disponibilité article par niveau de nomenclature**.</span><span class="sxs-lookup"><span data-stu-id="7b703-122">The quantity figures come from the same engine that provides information to the **Item Availability by BOM Level** window.</span></span> |
|<span data-ttu-id="7b703-123">**Distribution coût total nomenclature**</span><span class="sxs-lookup"><span data-stu-id="7b703-123">**BOM Cost Share Distribution**</span></span>|<span data-ttu-id="7b703-124">5872</span><span class="sxs-lookup"><span data-stu-id="7b703-124">5872</span></span>|<span data-ttu-id="7b703-125">Indique graphiquement la manière dont le coût d’un article assemblé ou produit est distribué dans sa nomenclature.</span><span class="sxs-lookup"><span data-stu-id="7b703-125">Shows graphically how an assembled or produced item’s cost is distributed through its BOM.</span></span><br><span data-ttu-id="7b703-126">Ces informations peuvent être utiles pour décider, par exemple, de changer de fournisseurs de composants, de remplacer une utilisation interne de capacité par un travail externalisé, ou inversement, ou lors de l’examen et de la modification de la nomenclature d’un article.</span><span class="sxs-lookup"><span data-stu-id="7b703-126">Such information can be useful in deciding, for example, whether to change component suppliers, replace internal capacity usage with outsourced labor or vice versa or when reviewing and modifying an item’s bill of material.</span></span><br><span data-ttu-id="7b703-127">Le premier graphique de l’état affiche le coût unitaire total des composants et des ressources de travail de l’article parent, réparti en cinq parts de coût différentes au maximum et représenté graphiquement par des couleurs différentes.</span><span class="sxs-lookup"><span data-stu-id="7b703-127">The first chart in the report shows the total unit cost of the parent item’s components and labor resources broken down in up to five different cost shares, and represented graphically with different colors.</span></span><br><span data-ttu-id="7b703-128">Le graphique en secteurs avec la légende *Par matière/travail* affiche la répartition proportionnelle entre les coûts de matériel et de travail de l’article parent, ainsi que ses propres frais généraux de fabrication.</span><span class="sxs-lookup"><span data-stu-id="7b703-128">The pie chart with the caption *By Material/Labor* shows the proportional distribution between the parent item’s material and labor costs, as well as its own manufacturing overhead.</span></span> <span data-ttu-id="7b703-129">La part du coût matière inclut les coûts matière de l’article.</span><span class="sxs-lookup"><span data-stu-id="7b703-129">The material cost share includes the item's material costs.</span></span> <span data-ttu-id="7b703-130">La part du coût de travail inclut la capacité, les frais généraux opératoires et les coûts de sous-traitance.</span><span class="sxs-lookup"><span data-stu-id="7b703-130">The labor cost share includes capacity, capacity overhead and subcontracted costs.</span></span> <span data-ttu-id="7b703-131">Les parts de coûts sont affichées différemment en fonction des choix indiqués dans le champ **Afficher uniquement**.</span><span class="sxs-lookup"><span data-stu-id="7b703-131">The cost shares are displayed differently depending on your choices in the **Show only** field.</span></span><br><span data-ttu-id="7b703-132">Le graphique en secteurs avec la légende *Par direct/indirect* affiche la répartition proportionnelle entre les coûts directs et indirects de la nomenclature.</span><span class="sxs-lookup"><span data-stu-id="7b703-132">The pie chart with the caption *By Direct/Indirect* shows the proportional distribution between the parent item's direct and indirect costs.</span></span> <span data-ttu-id="7b703-133">La part des coûts directs inclut les coûts matière, de capacité et les coûts de sous-traitance de l’article.</span><span class="sxs-lookup"><span data-stu-id="7b703-133">The direct cost share includes the item's material, capacity, and subcontracted costs.</span></span> <span data-ttu-id="7b703-134">La part des coûts indirects inclut les frais généraux opératoires et les frais généraux de fabrication.</span><span class="sxs-lookup"><span data-stu-id="7b703-134">The indirect cost share includes capacity overhead and manufacturing overhead.</span></span><br><span data-ttu-id="7b703-135">Le tableau en bas de l’état est inclus lorsque vous activez la case à cocher **Inclure détails**.</span><span class="sxs-lookup"><span data-stu-id="7b703-135">The table at the bottom of the report is included when you select the **Include Details** check box.</span></span> <span data-ttu-id="7b703-136">Il affiche les valeurs sélectionnées dans la fenêtre Coûts totaux nomenclature par mono-niveau ou multi-niveau, en fonction du choix que vous avez effectué dans le champ **Afficher coût total comme**.</span><span class="sxs-lookup"><span data-stu-id="7b703-136">It shows selected values from the BOM Cost Shares window by single level or rolled up, depending on your choices in the **Show Cost Shares as** field.</span></span>|
|<span data-ttu-id="7b703-137">**Coût détaillé**</span><span class="sxs-lookup"><span data-stu-id="7b703-137">**Detailed Calculation**</span></span>|<span data-ttu-id="7b703-138">99000756</span><span class="sxs-lookup"><span data-stu-id="7b703-138">99000756</span></span>|<span data-ttu-id="7b703-139">Affiche la liste des coûts par article en tenant compte du rebut.</span><span class="sxs-lookup"><span data-stu-id="7b703-139">Shows a cost list per item taking into account the scrap.</span></span>|
|<span data-ttu-id="7b703-140">**Cas d’emploi (multi-niveau)**</span><span class="sxs-lookup"><span data-stu-id="7b703-140">**Where-Used (Top Level)**</span></span>|<span data-ttu-id="7b703-141">99000757</span><span class="sxs-lookup"><span data-stu-id="7b703-141">99000757</span></span>|<span data-ttu-id="7b703-142">Affiche où et en quelle quantité sont utilisés les articles dans la structure produit.</span><span class="sxs-lookup"><span data-stu-id="7b703-142">Shows where and in what quantities the items are used in the product structure.</span></span><br><span data-ttu-id="7b703-143">L’état indique uniquement l’article comme cas d’emploi lorsque l’article de base est utilisé comme article de niveau supérieur.</span><span class="sxs-lookup"><span data-stu-id="7b703-143">The report shows only the item as where-used, when the base item is used as the top-level item.</span></span> <span data-ttu-id="7b703-144">Par exemple, si l’article A est utilisé pour fabriquer l’article B, et que l’article B est utilisé pour fabriquer l’article C, l’état affiche l’article B si vous exécutez cet état pour l’article A. Si vous exécutez l’article B, l’article C est affiché comme cas d’emploi.</span><span class="sxs-lookup"><span data-stu-id="7b703-144">For example, if item "A" is used to produce item "B", and item "B" is used to produce item "C", the report will show item B if you run this report for item A. If you run this report for item B, then item C will be shown as where-used.</span></span><br><span data-ttu-id="7b703-145">Vous pouvez également ouvrir la page **Ligne cas d’emploi** directement à partir de l’article.</span><span class="sxs-lookup"><span data-stu-id="7b703-145">You can also open the **Where-Used Line** page directly from the item.</span></span>|
|<span data-ttu-id="7b703-146">**Liste de comparaison des nomenclatures article**</span><span class="sxs-lookup"><span data-stu-id="7b703-146">**Item BOM Compare list**</span></span>|<span data-ttu-id="7b703-147">99000758</span><span class="sxs-lookup"><span data-stu-id="7b703-147">99000758</span></span>|<span data-ttu-id="7b703-148">Cet état vous donne la possibilité de comparer des produits finis similaires concernant les coûts.</span><span class="sxs-lookup"><span data-stu-id="7b703-148">This report gives you the possibility to compare similar final products concerning the costs.</span></span> <span data-ttu-id="7b703-149">Vous verrez une liste de tous les composants et leurs coûts, ainsi que les quantités nécessaires.</span><span class="sxs-lookup"><span data-stu-id="7b703-149">You will see a listing with all components and their costs as well the needed quantities.</span></span> <span data-ttu-id="7b703-150">La date de calcul est normalement fixée à la date de travail.</span><span class="sxs-lookup"><span data-stu-id="7b703-150">The calculation date is normally set to the work date.</span></span> |
|<span data-ttu-id="7b703-151">**Statistiques O.F.**</span><span class="sxs-lookup"><span data-stu-id="7b703-151">**Production Order Statistics**</span></span>|<span data-ttu-id="7b703-152">99000791</span><span class="sxs-lookup"><span data-stu-id="7b703-152">99000791</span></span>|<span data-ttu-id="7b703-153">Spécifie les différents coûts qui se sont cumulés de l’ordre de fabrication sélectionné.</span><span class="sxs-lookup"><span data-stu-id="7b703-153">Specifies the various costs that have accumulated for the selected production order.</span></span><br><span data-ttu-id="7b703-154">Le contenu de l’état est presque identique à la page **Statistiques O.F.**.</span><span class="sxs-lookup"><span data-stu-id="7b703-154">The content of the report are very similar to the **Production Order Statistics** page.</span></span><br><span data-ttu-id="7b703-155">Pour les ordres de fabrication utilisant la méthode de fabrication *Fabrication à la commande*, la fenêtre n’affiche que le coût matière et capacité des articles au niveau de nomenclature le plus élevé.</span><span class="sxs-lookup"><span data-stu-id="7b703-155">For production orders that use the *Make-to-Order* manufacturing policy, the window only shows material and capacity cost of items at the highest BOM level.</span></span>|
|<span data-ttu-id="7b703-156">**Liste des tâches par capacité**</span><span class="sxs-lookup"><span data-stu-id="7b703-156">**Capacity Task list**</span></span>|<span data-ttu-id="7b703-157">99000780</span><span class="sxs-lookup"><span data-stu-id="7b703-157">99000780</span></span>|<span data-ttu-id="7b703-158">Indique les ordres de fabrication en attente de traitement dans les centres ou les postes de charge.</span><span class="sxs-lookup"><span data-stu-id="7b703-158">Shows the production orders that are waiting to be processed at the work centers and machine centers.</span></span> <span data-ttu-id="7b703-159">Les documents imprimés indiquent la capacité du centre ou du poste de charge).</span><span class="sxs-lookup"><span data-stu-id="7b703-159">Printouts are made for the capacity of the work center or machine center).</span></span> <span data-ttu-id="7b703-160">L’état comprend les données telles que l’heure début et fin, la date O.F. et la quantité d’entrée.</span><span class="sxs-lookup"><span data-stu-id="7b703-160">The report includes information such as starting and ending time, date per production order and input quantity.</span></span>|
|<span data-ttu-id="7b703-161">**Charge centre de charge** ou **Charge poste de charge**</span><span class="sxs-lookup"><span data-stu-id="7b703-161">**Work Center Load** or **Machine Center Load**</span></span>|<span data-ttu-id="7b703-162">99000783 ou 99000784</span><span class="sxs-lookup"><span data-stu-id="7b703-162">99000783 or 99000784</span></span>|<span data-ttu-id="7b703-163">Les deux états affichent la liste de la charge d’un centre de charge ou d’un poste de charge.</span><span class="sxs-lookup"><span data-stu-id="7b703-163">Both reports show a list for the load on a work or machine center.</span></span> <span data-ttu-id="7b703-164">La charge d’un centre de charge/poste de charge représente la somme du nombre d’heures nécessaires pour exécuter toutes les commandes réelles et planifiées dans un centre de charge, sur une période précise.</span><span class="sxs-lookup"><span data-stu-id="7b703-164">The load on a work/machine center is the sum of the required number of times that all the planned and actual orders are run on the work center in a specified period.</span></span>|
|<span data-ttu-id="7b703-165">**Liste des ruptures O.F.**</span><span class="sxs-lookup"><span data-stu-id="7b703-165">**Prod. Order Shortage list**</span></span>|<span data-ttu-id="7b703-166">99000788</span><span class="sxs-lookup"><span data-stu-id="7b703-166">99000788</span></span>|<span data-ttu-id="7b703-167">Cet état peut être utilisé pour voir tous les composants qui ne sont pas disponibles en raison d’un stock manquant.</span><span class="sxs-lookup"><span data-stu-id="7b703-167">This report can be used to see all components that are not available because of missing stock.</span></span> <span data-ttu-id="7b703-168">Ainsi, cet aperçu peut être utilisé pour voir si le calendrier d’un ordre de fabrication planifié ou lancé et si le temps planifié peuvent être respectés.</span><span class="sxs-lookup"><span data-stu-id="7b703-168">So, this overview can be used to see in time, if the timeline for a planned or released production order if the planned time can be kept.</span></span>|


## <a name="tasks"></a><span data-ttu-id="7b703-169">Tâches</span><span class="sxs-lookup"><span data-stu-id="7b703-169">Tasks</span></span>

<span data-ttu-id="7b703-170">Les articles suivants décrivent certaines des tâches clés pour analyser l’état de votre entreprise :</span><span class="sxs-lookup"><span data-stu-id="7b703-170">The following articles describe some of the key tasks for analyzing the state of your business:</span></span>

* [<span data-ttu-id="7b703-171">Afficher la charge des centres de charge et des postes de charge</span><span class="sxs-lookup"><span data-stu-id="7b703-171">View Load on Work and Machine Centers</span></span>](production-how-to-view-the-load-on-work-centers.md)  
* [<span data-ttu-id="7b703-172">Voir la disponibilité des articles</span><span class="sxs-lookup"><span data-stu-id="7b703-172">View the Availability of Items</span></span>](inventory-how-availability-overview.md)

## <a name="see-also"></a><span data-ttu-id="7b703-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7b703-173">See also</span></span>

[<span data-ttu-id="7b703-174">Paramétrage de la production</span><span class="sxs-lookup"><span data-stu-id="7b703-174">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
[<span data-ttu-id="7b703-175">Production</span><span class="sxs-lookup"><span data-stu-id="7b703-175">Manufacturing</span></span>](production-manage-manufacturing.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]