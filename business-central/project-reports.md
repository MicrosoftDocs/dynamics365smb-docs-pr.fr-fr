---
title: États et analyses de projet
description: Découvrez les états et analyses de projet disponibles dans la version standard de Business Central afin que vous puissiez suivre votre activité.
author: AndreiPanko
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 06/01/2021
ms.author: andreipa
ms.openlocfilehash: ff5294df5cdbeaf0054249f017906bfd60ee4bf7
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/09/2021
ms.locfileid: "6216358"
---
# <a name="project-reports-and-analytics-in-business-central"></a><span data-ttu-id="3415e-103">États et analyses de projet dans Business Central</span><span class="sxs-lookup"><span data-stu-id="3415e-103">Project Reports and Analytics in Business Central</span></span>

<span data-ttu-id="3415e-104">Les états de projet dans [!INCLUDE [prod_short](includes/prod_short.md)] permettent aux professionnels des projets et des affaires d’obtenir des informations et des statistiques sur les activités de projet actuelles et passées.</span><span class="sxs-lookup"><span data-stu-id="3415e-104">Project reporting in [!INCLUDE [prod_short](includes/prod_short.md)] allows project and business professionals to get insights and statistics about current and past project activities.</span></span>  

## <a name="reports"></a><span data-ttu-id="3415e-105">États</span><span class="sxs-lookup"><span data-stu-id="3415e-105">Reports</span></span>

<span data-ttu-id="3415e-106">Le tableau suivant décrit certains des principaux états dans les états de projets.</span><span class="sxs-lookup"><span data-stu-id="3415e-106">The following table describes some of the key reports in jobs reporting.</span></span>

|<span data-ttu-id="3415e-107">État</span><span class="sxs-lookup"><span data-stu-id="3415e-107">Report</span></span> |<span data-ttu-id="3415e-108">ID d’objet</span><span class="sxs-lookup"><span data-stu-id="3415e-108">Object ID</span></span>|<span data-ttu-id="3415e-109">Description</span><span class="sxs-lookup"><span data-stu-id="3415e-109">Description</span></span>  |
|---------|---------|---------|
|<span data-ttu-id="3415e-110">**Analyse de projet**</span><span class="sxs-lookup"><span data-stu-id="3415e-110">**Job Analysis**</span></span>|<span data-ttu-id="3415e-111">1008</span><span class="sxs-lookup"><span data-stu-id="3415e-111">1008</span></span>|<span data-ttu-id="3415e-112">Analyse votre projet à l’aide des paramètres que vous spécifiez.</span><span class="sxs-lookup"><span data-stu-id="3415e-112">Analyzes your job by using settings that you specify.</span></span> <span data-ttu-id="3415e-113">Par exemple, vous pouvez créer un état avec les prix budgétés, les prix activité et les prix facturables, et comparer ainsi les trois types de prix.</span><span class="sxs-lookup"><span data-stu-id="3415e-113">For example, you can create a report that shows you the budgeted prices, usage prices, and billable prices, and then compares the three sets of prices.</span></span><br><span data-ttu-id="3415e-114">Permet d’utiliser une combinaison des champs **Montant** disponibles pour créer une analyse personnalisée.</span><span class="sxs-lookup"><span data-stu-id="3415e-114">Use a combination of the available **Amount** fields to create your own analysis.</span></span> <span data-ttu-id="3415e-115">Pour chaque champ, sélectionnez l’un des prix, coûts ou marge suivants : Planifié, Activité, Contrat et Facturé.</span><span class="sxs-lookup"><span data-stu-id="3415e-115">For each field, select one of the following prices, costs, or profit values: Schedule, Usage, Contract, and Invoiced.</span></span> <br><span data-ttu-id="3415e-116">Permet de choisir l’affichage de la devise en Devise société (DS) ou en Devise étrangère (DE).</span><span class="sxs-lookup"><span data-stu-id="3415e-116">Select whether the currency is specified in Local Currency or Foreign Currency.</span></span> |
|<span data-ttu-id="3415e-117">**Lignes planning projet**</span><span class="sxs-lookup"><span data-stu-id="3415e-117">**Job Planning Lines**</span></span>|<span data-ttu-id="3415e-118">1006</span><span class="sxs-lookup"><span data-stu-id="3415e-118">1006</span></span>|<span data-ttu-id="3415e-119">Cet état affiche les différentes lignes planning projet et tâche projet, y compris le type de ligne, les quantités, l’unité, les coûts totaux, etc.</span><span class="sxs-lookup"><span data-stu-id="3415e-119">This report shows the different job planning and job task lines – including the line type, quantities, unit of measure, total costs, etc.</span></span>|
|<span data-ttu-id="3415e-120">**Projet Comp. réal./Budget**</span><span class="sxs-lookup"><span data-stu-id="3415e-120">**Job Actual to Budget**</span></span>|<span data-ttu-id="3415e-121">1009</span><span class="sxs-lookup"><span data-stu-id="3415e-121">1009</span></span>|<span data-ttu-id="3415e-122">Compare les montants d’activité et prévus des projets sélectionnés.</span><span class="sxs-lookup"><span data-stu-id="3415e-122">Compares scheduled and usage amounts for selected jobs.</span></span> <span data-ttu-id="3415e-123">Toutes les lignes du projet sélectionné indiquent la quantité, le coût total et le montant ligne.</span><span class="sxs-lookup"><span data-stu-id="3415e-123">All lines of the selected job show quantity, total cost, and line amount.</span></span> <br><span data-ttu-id="3415e-124">Cet état est prévu pour les projets terminés, mais vous pouvez l’utiliser à tout moment.</span><span class="sxs-lookup"><span data-stu-id="3415e-124">This report is intended for completed jobs, although you can use it at any time during a job.</span></span><br><span data-ttu-id="3415e-125">Cet état n’est pas disponible aux États-Unis, au Canada et au Mexique.</span><span class="sxs-lookup"><span data-stu-id="3415e-125">In the US, Canada, and Mexico, this report is not available.</span></span> <span data-ttu-id="3415e-126">Utilisez plutôt les états **Comparaison Coût réel projet/Coût budgété** (10210) ou **Comparaison Prix réel projet/Prix budgété** (10211).</span><span class="sxs-lookup"><span data-stu-id="3415e-126">Instead, use the **Job Actual to Budget (Cost)** (10210) or **Job Actual to Budget (Price)** (10211) reports.</span></span>|
|<span data-ttu-id="3415e-127">**Prop. de facturation projet**</span><span class="sxs-lookup"><span data-stu-id="3415e-127">**Job Suggested Billing**</span></span>|<span data-ttu-id="3415e-128">1011</span><span class="sxs-lookup"><span data-stu-id="3415e-128">1011</span></span>|<span data-ttu-id="3415e-129">Affiche la liste de tous les projets groupés par client, en indiquant le montant déjà facturé au client et le montant restant à facturer, c’est-à-dire la proposition de facturation.</span><span class="sxs-lookup"><span data-stu-id="3415e-129">Shows a list of all jobs, grouped by customer, how much the customer has already been invoiced, and how much remains to be invoiced, that is, the suggested billing.</span></span> <br><span data-ttu-id="3415e-130">Cet état n’est pas disponible aux États-Unis, au Canada et au Mexique.</span><span class="sxs-lookup"><span data-stu-id="3415e-130">In the US, Canada, and Mexico, this report is not available.</span></span> <span data-ttu-id="3415e-131">Utilisez plutôt l’état **Prop. de facturation coût projet** (10219).</span><span class="sxs-lookup"><span data-stu-id="3415e-131">Instead, use the **Job Cost Suggested Billing** (10219) report.</span></span>|
|<span data-ttu-id="3415e-132">**Projets par client**</span><span class="sxs-lookup"><span data-stu-id="3415e-132">**Jobs per Customer**</span></span>|<span data-ttu-id="3415e-133">1012</span><span class="sxs-lookup"><span data-stu-id="3415e-133">1012</span></span>|<span data-ttu-id="3415e-134">Affiche la liste de tous les projets groupés par client.</span><span class="sxs-lookup"><span data-stu-id="3415e-134">Shows a list of all jobs, grouped by customer.</span></span> <span data-ttu-id="3415e-135">Il permet de comparer le prix planifié, le pourcentage d’achèvement, le prix facturé et le pourcentage de facturation pour chaque **Client facturé**.</span><span class="sxs-lookup"><span data-stu-id="3415e-135">It allows you to compare the scheduled price, the percentage of completion, the invoiced price, and the percentage of invoiced amounts for each **Bill-to Customer**.</span></span>|
|<span data-ttu-id="3415e-136">**Articles par projet** ou **Projets par article**</span><span class="sxs-lookup"><span data-stu-id="3415e-136">**Items per Job** or **Jobs per Item**</span></span>|<span data-ttu-id="3415e-137">1013 ou 1014</span><span class="sxs-lookup"><span data-stu-id="3415e-137">1013 or 1014</span></span>|<span data-ttu-id="3415e-138">Aperçu des articles utilisés dans un projet.</span><span class="sxs-lookup"><span data-stu-id="3415e-138">An overview about the used items in a job.</span></span> <span data-ttu-id="3415e-139">En fonction de l’état que vous souhaitez utiliser pour obtenir un aperçu des articles planifiés pour un projet, vous pouvez définir un filtre supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="3415e-139">Depending on the report that you want to use to get an overview about the planned items for a project, you can set an additional filter.</span></span> <span data-ttu-id="3415e-140">L’état affiche les articles pertinents et une valeur cumulée des coûts.</span><span class="sxs-lookup"><span data-stu-id="3415e-140">The report shows the relevant items and an accumulated value about the costs.</span></span>|
|<span data-ttu-id="3415e-141">**Détail transactions projet**</span><span class="sxs-lookup"><span data-stu-id="3415e-141">**Job Transaction Detail**</span></span>|<span data-ttu-id="3415e-142">1007</span><span class="sxs-lookup"><span data-stu-id="3415e-142">1007</span></span>|<span data-ttu-id="3415e-143">Cet état vous donnera un aperçu des tâches de projets validées, telles que les ressources et les articles.</span><span class="sxs-lookup"><span data-stu-id="3415e-143">This report will give you an overview over the posted job tasks like resources and items.</span></span> <span data-ttu-id="3415e-144">Comprend des informations détaillées sur les coûts totaux et les prix totaux ainsi qu’une information concernant les remises ligne, etc.</span><span class="sxs-lookup"><span data-stu-id="3415e-144">Includes a detailed information about the total costs and total prices plus an information concerning line discounts,and so on.</span></span> <span data-ttu-id="3415e-145">L’état affiche les données des écritures comptables projet.</span><span class="sxs-lookup"><span data-stu-id="3415e-145">The report shows data from the job ledger entries.</span></span>|
|<span data-ttu-id="3415e-146">**Projet TEC en comptabilité**</span><span class="sxs-lookup"><span data-stu-id="3415e-146">**Job WIP to G/L**</span></span>|<span data-ttu-id="3415e-147">1010</span><span class="sxs-lookup"><span data-stu-id="3415e-147">1010</span></span>|<span data-ttu-id="3415e-148">Affiche la valeur des encours des projets sélectionnés comparée au montant validé en comptabilité.</span><span class="sxs-lookup"><span data-stu-id="3415e-148">Shows the value of work in process on the jobs that you select compared to the amount that has been posted in the general ledger.</span></span>|




## <a name="tasks"></a><span data-ttu-id="3415e-149">Tâches</span><span class="sxs-lookup"><span data-stu-id="3415e-149">Tasks</span></span>

<span data-ttu-id="3415e-150">Les articles suivants décrivent certaines des tâches clés pour analyser l’état de votre entreprise :</span><span class="sxs-lookup"><span data-stu-id="3415e-150">The following articles describe some of the key tasks for analyzing the state of your business:</span></span>

* [<span data-ttu-id="3415e-151">Surveiller la progression et les performances</span><span class="sxs-lookup"><span data-stu-id="3415e-151">Monitor Job Progress and Performance</span></span>](projects-how-monitor-progress-performance.md)  


## <a name="see-also"></a><span data-ttu-id="3415e-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3415e-152">See also</span></span>

[<span data-ttu-id="3415e-153">Configuration de la gestion de projet</span><span class="sxs-lookup"><span data-stu-id="3415e-153">Setting Up Project Management</span></span>](projects-setup-projects.md)  
[<span data-ttu-id="3415e-154">Gestion de projets</span><span class="sxs-lookup"><span data-stu-id="3415e-154">Project management</span></span>](projects-manage-projects.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]