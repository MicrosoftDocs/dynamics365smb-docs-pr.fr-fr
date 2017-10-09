---
title: "Procédure de configuration des centres de coûts | Microsoft Docs"
description: "Les centres de coûts sont les départements responsables des coûts et des revenus. Le plan des centres de coûts est semblable aux informations sur l'axe analytique pour la comptabilité."
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
ms.openlocfilehash: 433526fbd2a13f32e64be94cc1936151445c19f5
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-cost-centers"></a><span data-ttu-id="ec4d8-104">Procédure : configuration des centres de coûts</span><span class="sxs-lookup"><span data-stu-id="ec4d8-104">How to: Set Up Cost Centers</span></span>
<span data-ttu-id="ec4d8-105">Les centres de coûts sont les départements responsables des coûts et des revenus.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-105">Cost centers are departments that are responsible for costs and income.</span></span> <span data-ttu-id="ec4d8-106">Le plan des centres de coûts est semblable aux informations sur l'axe analytique pour la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-106">The chart of cost centers is similar to the dimension information for the general ledger.</span></span> <span data-ttu-id="ec4d8-107">Vous pouvez configurer le plan des centres de coûts comme suit :</span><span class="sxs-lookup"><span data-stu-id="ec4d8-107">You can set up the chart of cost centers in the following ways:</span></span>  

-   <span data-ttu-id="ec4d8-108">Transférez des sections analytiques de la comptabilité vers le plan des centres de coûts.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-108">Transfer dimension values in the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="ec4d8-109">Vous pouvez effectuer tous les ajustements nécessaires après le transfert.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-109">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="ec4d8-110">Créez un nouveau plan du centre de coûts, qui est indépendant de la comptabilité ou ajoutez un nouveau centre de coûts à un plan existant du centre de coûts.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-110">Create a new chart of cost center that is independent of the general ledger or add a new cost center to an existing chart of cost center.</span></span> <span data-ttu-id="ec4d8-111">Vous devez créer chaque centre de coûts individuellement.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-111">You must create each cost center individually.</span></span>  

## <a name="to-transfer-dimension-values-in-the-general-ledger-to-the-chart-of-cost-centers"></a><span data-ttu-id="ec4d8-112">Pour transférer des sections analytiques de la comptabilité vers le plan des centres de coûts.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-112">To transfer dimension values in the general ledger to the chart of cost centers</span></span>  
1.  <span data-ttu-id="ec4d8-113">Définissez un axe analytique pour être celui de la dimension des centres de coûts dans la fenêtre **Mettre à jour les axes analytiques de comptabilité analytique**.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-113">Set up a dimension to be the cost center dimension in the **Update Cost Acctg. Dimensions** window.</span></span> <span data-ttu-id="ec4d8-114">Seules les valeurs de cet axe analytique sont transférées.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-114">Only the values from this dimension are transferred.</span></span>  
2.  <span data-ttu-id="ec4d8-115">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Plan comptable des centres de coûts**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Centers**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="ec4d8-116">Sous l'onglet **Actions**, dans le groupe **Fonctions**, choisissez **Extraire les centres de coûts de l'axe analytique** pour transférer des sections du plan des centres de coûts.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost Centers from Dimension** to transfer dimension values to the chart of cost centers.</span></span> <span data-ttu-id="ec4d8-117">La fonction transfère les sections analytiques que vous avez définis dans l'étape 1.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-117">The function transfers the dimension values that you defined in step 1.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="ec4d8-118">Vous pouvez configurer le champ **Aligner axe centre de coûts** pour définir la synchronisation unidirectionnelle des sections analytiques à partir de la comptabilité vers le plan des centres de coûts.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-118">You can set up the **Align Cost Center Dimension**  field to define a one-way synchronization of dimension values from the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="ec4d8-119">Vous ne pouvez pas définir une synchronisation du plan des centres de coûts avec les sections analytiques issues de la comptabilité.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-119">You cannot define a synchronization of the chart of cost centers to dimension values from the general ledger.</span></span>  

<span data-ttu-id="ec4d8-120">Le plan des centres de coûts comprend désormais toutes les sections analytiques spécifiées provenant de la comptabilité. Il inclut les titres et les sous-totaux.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-120">The chart of cost centers now contains all specified dimension values from the general ledger and includes titles and subtotals.</span></span>  

## <a name="to-create-new-cost-centers-in-the-chart-of-cost-centers-window"></a><span data-ttu-id="ec4d8-121">Pour créer de nouveaux centres de coût dans la fenêtre Plan comptable des centres de coûts</span><span class="sxs-lookup"><span data-stu-id="ec4d8-121">To create new cost centers in the Chart of Cost Centers window</span></span>  
<span data-ttu-id="ec4d8-122">Vous pouvez configurer et gérer les centres de coût, soit dans la fenêtre **Fiche centre de coût**, soit dans la fenêtre **Plan comptable des centres de coûts**.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-122">You can set up and maintain cost centers in either the **Cost Center Card** card or in the **Chart of Cost Centers** window.</span></span> <span data-ttu-id="ec4d8-123">Dans cette procédure, vous configurez de nouveaux centres de coût dans la fenêtre **Plan comptable des centres de coûts**.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-123">In this procedure, you set up cost centers in the **Chart of Cost Centers** window.</span></span>  

1. <span data-ttu-id="ec4d8-124">Ouvrez la fenêtre **Plan comptable des centres de coûts** en mode édition.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-124">Open the **Chart of Cost Centers** window in edit mode.</span></span>  
2. <span data-ttu-id="ec4d8-125">Dans le champ **Code**, entrez le code centre de coûts.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-125">In the **Code** field, enter the cost center code.</span></span> <span data-ttu-id="ec4d8-126">Tous les centres de coûts doivent avoir un code.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-126">All cost centers must have a code.</span></span>  
3. <span data-ttu-id="ec4d8-127">Dans le champ **Nom**, saisissez le nom du centre de coûts.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-127">In the **Name** field, enter the cost center name.</span></span>  
4. <span data-ttu-id="ec4d8-128">Sélectionnez la flèche déroulante dans le champ **Type ligne** pour spécifier l'objectif du centre de coûts.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost center.</span></span>  

    - <span data-ttu-id="ec4d8-129">Pour les centres de coûts de type **Total**, vous devez renseigner le champ **Totalisation**.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span></span> <span data-ttu-id="ec4d8-130">Utilisez l'opérateur **or**, qui est une ligne verticale (**&#124;**) pour définir les plages des centres de coûts.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span></span>  
    - <span data-ttu-id="ec4d8-131">Pour les centres de coûts de type de ligne **Fin total**, ce champ est renseigné automatiquement lorsque vous utilisez la fonction d'indentation.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-131">For cost centers of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span></span>  
5.  <span data-ttu-id="ec4d8-132">Renseignez les champs **Ordre de tri** et **Sous-type coût**.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span></span>  
6.  <span data-ttu-id="ec4d8-133">Choisissez la ligne vide suivante pour créer un centre de coûts, puis répétez les étapes 2 à 5.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-133">Choose the next empty line to create a new cost center, and then repeat steps 2 through 5.</span></span>  
7.  <span data-ttu-id="ec4d8-134">Après avoir défini tous les centres de coûts, choisissez l'action **Indenter les centres de coûts**.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-134">After you have set up all the cost centers, choose the **Indent Cost Centers** action.</span></span> <span data-ttu-id="ec4d8-135">Cliquez sur le bouton **Oui**.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-135">Choose the **Yes** button.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="ec4d8-136">Si vous avez saisi des définitions dans les champs **Totalisation** pour les centres de coûts **Fin total** avant d'exécuter la fonction d'indentation, vous devez les saisir à nouveau.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-136">If you have entered definitions in the **Totaling** fields for **End-Total** cost centers before you run the indent function, then you must enter them again.</span></span> <span data-ttu-id="ec4d8-137">La fonction remplace les valeurs dans tous les champs **Fin total**.</span><span class="sxs-lookup"><span data-stu-id="ec4d8-137">The function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ec4d8-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec4d8-138">See Also</span></span>  
[<span data-ttu-id="ec4d8-139">Comptabilité pour les coûts</span><span class="sxs-lookup"><span data-stu-id="ec4d8-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="ec4d8-140">[Paramétrage du contrôle de gestion](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="ec4d8-140">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="ec4d8-141">[Terminologie en comptabilité analytique](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="ec4d8-141">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="ec4d8-142">À propos de la comptabilité analytique</span><span class="sxs-lookup"><span data-stu-id="ec4d8-142">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="ec4d8-143">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ec4d8-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
