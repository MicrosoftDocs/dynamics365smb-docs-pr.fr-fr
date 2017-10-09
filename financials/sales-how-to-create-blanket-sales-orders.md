---
title: "Procédure : créer des commandes ouvertes vente | Microsoft Docs"
description: "Utilisez des commandes ouvertes quand un client a accepté d'acheter de grandes quantités à livrer en plusieurs expéditions de petite taille au cours d'une période déterminée."
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 0b91925a7ec6adb40cdf99d5bcf3398b62c28b3f
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-work-with-blanket-sales-orders"></a><span data-ttu-id="f0b1a-103">Procédure : utiliser des commandes ouvertes vente</span><span class="sxs-lookup"><span data-stu-id="f0b1a-103">How to: Work with Blanket Sales Orders</span></span>
<span data-ttu-id="f0b1a-104">Une commande ouverte vente représente le cadre d'un accord à long terme entre votre client et vous.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-104">A blanket sales order represents a framework for a long-term agreement between you and your customer.</span></span>

<span data-ttu-id="f0b1a-105">Une commande ouverte est généralement établie quand un client s'est engagé à acheter de grandes quantités à livrer en plusieurs expéditions de plus petite taille au cours d'une période déterminée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-105">A blanket order is typically made when a customer has committed to purchasing large quantities that are to be delivered in several smaller shipments over a certain period of time.</span></span> <span data-ttu-id="f0b1a-106">Souvent, les commandes ouvertes ne portent que sur un seul article avec des dates de livraison prédéterminées.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-106">Often blanket orders cover only one item with predetermined delivery dates.</span></span> <span data-ttu-id="f0b1a-107">La principale raison d'utiliser une commande ouverte plutôt qu'une commande vente est que les quantités entrées dans une commande ouverte n'affectent pas la disponibilité de l'article et peuvent donc être utilisées comme une feuille à des fins de surveillance, de précision et de planification.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-107">The main reason for using a blanket order rather than a sales order is that quantities entered on a blanket order do not affect item availability and thus can be used as a worksheet for monitoring, forecasting, and planning purposes.</span></span>

<span data-ttu-id="f0b1a-108">Sur la commande ouverte, vous pouvez configurer chaque expédition comme une ligne commande distincte qui peut ensuite être convertie en commande vente au moment de l'expédition.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-108">On the blanket order, each separate shipment can be set up as an order line, which can then be converted into a sales order at the time of shipping.</span></span>

<span data-ttu-id="f0b1a-109">Vous pouvez utiliser une commande ouverte vente, par exemple, lorsqu'un client appelle pour passer une commande de 1 000 unités d'un article et souhaite des livraisons par lot de 250 unités chaque semaine du mois suivant.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-109">An example of when a blanket sales order could be used is if a customer calls and places an order of 1000 units of an item and they want the items to be delivered in 250 units every week over the next month.</span></span>

> [!NOTE]
> <span data-ttu-id="f0b1a-110">Les commandes ouvertes achat fonctionnent de la même manière que les commandes ouvertes vente.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-110">Blanket purchase orders work in a similar way as blanket sales orders.</span></span> <span data-ttu-id="f0b1a-111">Cette documentation ne couvre pas les commandes ouvertes achat.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-111">This documentation does not cover blanket purchase orders.</span></span>

## <a name="to-create-a-blanket-sales-order"></a><span data-ttu-id="f0b1a-112">Pour créer une commande vente ouverte.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-112">To create a blanket sales order</span></span>  
1. <span data-ttu-id="f0b1a-113">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Commandes ouvertes vente**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Blanket Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f0b1a-114">Sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-114">Choose the **New** action.</span></span>  
3. <span data-ttu-id="f0b1a-115">Renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  <span data-ttu-id="f0b1a-116">Laissez vide le champ **Date commande**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-116">Leave the **Order Date** field blank.</span></span> <span data-ttu-id="f0b1a-117">Lors de la création de commandes vente séparées depuis la commande ouverte, la date commande de la commande vente est définie comme égale à la date du jour.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-117">When the separate sales orders are created from the blanket order, the order date of the sales order is set to equal the actual work date.</span></span>
5. <span data-ttu-id="f0b1a-118">Dans le raccourci **Lignes**, créez des lignes distinctes pour chaque expédition.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-118">On the **Lines** FastTab, create separate lines for each shipment.</span></span> <span data-ttu-id="f0b1a-119">Par exemple, si le client souhaite 1 000 unités réparties de façon uniforme sur quatre semaines, entrez quatre lignes distinctes de 250 unités chacune.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-119">For instance, if your customer wants 1000 units split out equally between four weeks, you would enter four separate lines of 250 units each.</span></span>   

## <a name="to-create-a-sales-order-from-a-blanket-sales-order"></a><span data-ttu-id="f0b1a-120">Pour créer une commande vente à partir d'une commande ouverte vente</span><span class="sxs-lookup"><span data-stu-id="f0b1a-120">To create a sales order from a blanket sales order</span></span>  

1.  <span data-ttu-id="f0b1a-121">Pour créer une commande pour l'une des lignes de l'ordre d'assemblage ouvert, effacez la quantité du champ **Qté à expédier** de toutes les lignes que vous ne voulez PAS expédier actuellement.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-121">To create an order for any of the lines in the blanket assembly order, remove the quantity in the **Qty. to Ship** field on all the lines that you DO NOT wish to ship at this time.</span></span>  
2.  <span data-ttu-id="f0b1a-122">Lorsque vous êtes prêt à créer les commandes, sélectionnez **Créer commande**, puis **Oui**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-122">When you are ready to create orders, choose the **Make Order**m action, and then choose **Yes**.</span></span> <span data-ttu-id="f0b1a-123">Un message s'affiche, vous informant que la commande ouverte a été associée à un numéro de commande.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-123">A message appears informing you that the blanket order has been assigned an order number.</span></span> <span data-ttu-id="f0b1a-124">Remarquez que la commande ouverte n'a pas été supprimée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-124">Note that the blanket order has not been deleted.</span></span>  
3.  <span data-ttu-id="f0b1a-125">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-125">Choose the **OK** button.</span></span>  
4.  <span data-ttu-id="f0b1a-126">Pour afficher les résultats des étapes précédentes, sélectionnez l'action **Ligne**, l'action **Lignes non validées**, puis l'action **Commandes**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-126">To see the results of the preceding steps, choose the **Line** action, choose the **Unposted Lines** action, and then choose the **Orders** action.</span></span>  
5.  <span data-ttu-id="f0b1a-127">Dans la fenêtre **Lignes vente**Lignes vente, sélectionnez la commande vente appropriée, sélectionnez l'action **Ligne**, sélectionnez Ligne, puis sélectionnez l'action **Afficher document**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-127">In the **Sales Lines** window, select the appropriate sales order, choose the **Line** action, and then choose the **Show Document** action.</span></span>  

<span data-ttu-id="f0b1a-128">Ce qui suit s'applique aux commandes vente après leur création à partir de commandes vente ouvertes :</span><span class="sxs-lookup"><span data-stu-id="f0b1a-128">The following applies to sales orders after they have been created from blanket sales orders:</span></span>  

- <span data-ttu-id="f0b1a-129">Une fois la commande ouverte convertie en commande vente, celle-ci contient toutes les lignes de la commande ouverte.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-129">After the blanket order is converted into a sales order, the sales order contains all the lines from the blanket order.</span></span> <span data-ttu-id="f0b1a-130">Les lignes où la quantité figurant dans le champ **Qté à expédier** a été supprimée s'affichent mais avec les champs **Quantité** vides.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-130">The lines where the quantity in the **Qty. to Ship** field was deleted appear, but with blank **Quantity** fields.</span></span> <span data-ttu-id="f0b1a-131">Vous pouvez décider de laisser, de modifier ou de supprimer les lignes.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-131">You may choose to leave, edit, or delete the lines.</span></span>  
- <span data-ttu-id="f0b1a-132">N'oubliez pas que la quantité de la ligne commande vente ne peut pas dépasser celle de la ligne commande ouverte associée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-132">It is important to remember that the sales order line quantity must not exceed the quantity of the associated blanket order line.</span></span> <span data-ttu-id="f0b1a-133">Sinon, la validation de la commande vente est impossible.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-133">Otherwise, posting of the sales order will not be possible.</span></span>  
- <span data-ttu-id="f0b1a-134">Lorsque la commande vente est validée comme expédiée et/ou facturée, les champs **Qté expédiée** et **Quantité facturée** sont mis à jour sur la commande ouverte concernée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-134">When the sales order is posted as shipped and/or invoiced, the **Quantity Shipped** and **Quantity Invoiced** fields are updated on the related blanket order.</span></span>  
- <span data-ttu-id="f0b1a-135">Le numéro de commande ouverte et un numéro de ligne sont enregistrés comme propriétés des lignes vente en cas de création à partir d'une commande ouverte.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-135">The blanket order number and line number are recorded as properties of the sales lines when created from a blanket order.</span></span>  
- <span data-ttu-id="f0b1a-136">Si les commandes vente ne sont pas créées directement depuis la commande ouverte mais ont trait à celle\-ci, il est possible de créer un lien entre une commande vente et une commande ouverte en entrant le numéro de commande ouverte associé dans le champ **N° commande ouverte**</span><span class="sxs-lookup"><span data-stu-id="f0b1a-136">When sales orders are not created directly from the blanket order but still relate to it, a link between a sales order and a blanket order can be established by entering the associated blanket order number in the **Blanket Order No.**</span></span> <span data-ttu-id="f0b1a-137">sur la ligne de commande vente.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-137">field on the sales order line.</span></span>  
- <span data-ttu-id="f0b1a-138">Une fois la commande vente créée pour la quantité totale d'une ligne commande ouverte, aucune autre commande vente ne peut être créée pour la même ligne.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-138">After the sales order has been created for the total quantity of a blanket order line, no other sales order can be created for the same line.</span></span> <span data-ttu-id="f0b1a-139">Les utilisateurs ne peuvent plus entrer de quantité dans le champ **Qté à expédier**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-139">Users are prevented from entering a quantity in the **Qty. to Ship** field.</span></span> <span data-ttu-id="f0b1a-140">Toutefois, si des quantités supplémentaires doivent être ajoutées à une commande ouverte, il est possible d'augmenter la valeur du champ **Quantité** et de créer des commandes supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-140">If, however, additional quantities need to be added to a blanket order, the value in the **Quantity** field can be increased and additional orders can then be created.</span></span>  
- <span data-ttu-id="f0b1a-141">La commande ouverte vente facturée reste dans le système jusqu'à ce qu'elle soit supprimée, soit en supprimant les commandes ouvertes individuelles, soit en exécutant le traitement par lots **Suppr. cdes vente ouv. fact.**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-141">The invoiced blanket sales order remains in the system until it is deleted, either by deleting individual blanket orders or by running the **Delete Invoiced Blanket Sales Orders** batch job.</span></span>  
- <span data-ttu-id="f0b1a-142">Si un client est également enregistré comme contact dans le module Marketing et si vous avez spécifié un code modèle interaction pour les commandes vente ouvertes dans la fenêtre **Paramètres Marketing**, lorsque vous sélectionnez **Imprimer** pour imprimer la commande vente ouverte, une interaction est enregistrée automatiquement dans la table Écriture journal interaction.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-142">If a customer is also recorded as a contact in the Marketing application area, and if you have specified an interaction template code for blanket sales order in the **Marketing Setup** window, an interaction is recorded in the Interaction Log Entry table when you select **Print** to print the blanket sales order.</span></span>

## <a name="to-view-the-status-of-a-blanket-purchase-order"></a><span data-ttu-id="f0b1a-143">Pour visualiser le statut d'une commande ouverte achat</span><span class="sxs-lookup"><span data-stu-id="f0b1a-143">To view the status of a blanket purchase order</span></span>  
<span data-ttu-id="f0b1a-144">Vous pouvez visualiser le statut d'une commande ouverte vente dans la fenêtre **Statistiques Commande ouverte achat**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-144">You can see the status of a blanket sales order in the **Purchase Blanket Order Statistics** window.</span></span> <span data-ttu-id="f0b1a-145">Ceci peut s'avérer utile lorsque vous commencez à facturer une commande créée à partir de la commande ouverte achat.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-145">This may be relevant when you start to invoice the order that is created from the blanket purchase order.</span></span>  

1.  <span data-ttu-id="f0b1a-146">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Commandes ouvertes vente**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-146">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Blanket Purchase Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f0b1a-147">Sélectionnez une commande ouverte achat, puis sélectionnez l'action **Statistiques**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-147">Select a blanket purchase order, and then choose the **Statistics** action.</span></span>  
3.  <span data-ttu-id="f0b1a-148">Dans la fenêtre **Statistiques Commande ouverte achat**, sur le raccourci **Général**, vous pouvez visualiser des informations récapitulatives concernant l'intégralité de la commande. Elles se basent sur la quantité totale des **champs Quantité** sur les lignes commande ouverte achat.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-148">In the **Purchase Blanket Order Statistics** window, on the **General** FastTab, you can see summary information about the entire order based on the total quantity in the various **Quantity fields** on the blanket purchase order lines.</span></span>  

    - <span data-ttu-id="f0b1a-149">Sur le raccourci **Facturation**, vous pouvez visualiser des informations récapitulatives concernant l'intégralité de la quantité dans les champs **Qté à facturer** des lignes commande ouverte achat.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-149">On the **Invoicing** FastTab, you can see summary information based on the total quantity in the **Qty. to Invoice** fields on the purchase blanket order lines.</span></span>  
    - <span data-ttu-id="f0b1a-150">Sur le raccourci **Expédition**, vous pouvez visualiser des informations récapitulatives concernant l'intégralité de la quantité dans les champs **Qté à recevoir** des lignes commande ouverte achat.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-150">On the **Shipping** FastTab, you can see summary information based on the total quantity in the **Qty. to Receive** fields on the purchase blanket order lines.</span></span>  
    - <span data-ttu-id="f0b1a-151">Sur le raccourci **Acompte**, vous pouvez visualiser des informations récapitulatives concernant les éventuels acomptes.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-151">On the **Prepayment** FastTab, you can see summary information about any prepaid amounts.</span></span>  
    - <span data-ttu-id="f0b1a-152">Sur le raccourci **Fournisseur**, vous pouvez visualiser certaines informations de base concernant le fournisseur.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-152">On the **Vendor** FastTab, you can see certain basic information about the vendor.</span></span>    

## <a name="to-view-unposted-and-posted-blanket-sales-order-lines"></a><span data-ttu-id="f0b1a-153">Pour afficher des lignes de commande vente ouverte non validées et validées</span><span class="sxs-lookup"><span data-stu-id="f0b1a-153">To view unposted and posted blanket sales order lines</span></span>   
<span data-ttu-id="f0b1a-154">Le lien entre la commande ouverte vente et la commande vente d'origine, et n'importe quel autre document vente, est conservé après validation en tant que liste des lignes facture validées et non validées de commande vente.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-154">The link between the blanket sales order and the originating sales order, and any other sales document, is retained after posting as a list of posted and unposted sales order invoice lines.</span></span>  

1. <span data-ttu-id="f0b1a-155">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Commandes ouvertes vente**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-155">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon enter **Blanket Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="f0b1a-156">Ouvrez la commande vente ouverte que vous souhaitez afficher.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-156">Open the blanket sales order you want to view.</span></span>
3. <span data-ttu-id="f0b1a-157">Pour visualiser les écritures non validées, sélectionnez la ligne en question, sélectionnez l'action **Ligne**, puis l'action **Lignes non validées**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-157">To view unposted entries, select the line in question, choose the **Line** action, and then choose the **Unposted Lines** action.</span></span> <span data-ttu-id="f0b1a-158">Choisissez l'une des options suivantes.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-158">Choose one of the following options.</span></span>  

    <table>
    <tr>
    <th><span data-ttu-id="f0b1a-159">Option</span><span class="sxs-lookup"><span data-stu-id="f0b1a-159">Option</span></span></th>
    <th><span data-ttu-id="f0b1a-160">Désignation</span><span class="sxs-lookup"><span data-stu-id="f0b1a-160">Description</span></span></th>
    </tr>
    <tr>
    <td><span data-ttu-id="f0b1a-161">**Commandes**</span><span class="sxs-lookup"><span data-stu-id="f0b1a-161">**Orders**</span></span></td>
    <td><span data-ttu-id="f0b1a-162">Spécifie les commandes ouvertes associées à la ligne sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-162">Specifies open orders associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="f0b1a-163">**Factures**</span><span class="sxs-lookup"><span data-stu-id="f0b1a-163">**Invoices**</span></span></td>
    <td><span data-ttu-id="f0b1a-164">Spécifie les factures ouvertes associées à la ligne sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-164">Specifies open invoices that have been associated with the selected line.</span></span> <span data-ttu-id="f0b1a-165">Ouvrez les factures associées manuellement à une commande ouverte en entrant le numéro de commande ouverte dans la ligne facture vente.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-165">Open invoices are manually associated with a blanket order by entering the blanket order number on the sales invoice line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="f0b1a-166">**Retours**</span><span class="sxs-lookup"><span data-stu-id="f0b1a-166">**Return Orders**</span></span></td>
    <td><span data-ttu-id="f0b1a-167">Spécifie les commandes retour ouvertes associées à la ligne sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-167">Specifies open return orders that have been associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="f0b1a-168">**Avoirs**</span><span class="sxs-lookup"><span data-stu-id="f0b1a-168">**Credit Memos**</span></span></td>
    <td><span data-ttu-id="f0b1a-169">Spécifie les avoirs ouverts associés à la ligne sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-169">Specifies open credit memos that have been associated with the selected line.</span></span></td>
    </tr>
    </table><span data-ttu-id="f0b1a-170">
4. Pour visualiser les écritures validées, sélectionnez la ligne en question, choisissez l'action **Ligne**, puis l'action **Lignes validées**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-170">
4. To view posted entries, select the line in question, choose the **Line** action, and then choose the **Posted Lines** action.</span></span> <span data-ttu-id="f0b1a-171">Choisissez l'une des options suivantes.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-171">Choose one of the following options.</span></span>  

    <table>
    <tr>
    <th><span data-ttu-id="f0b1a-172">Option</span><span class="sxs-lookup"><span data-stu-id="f0b1a-172">Option</span></span></th>
    <th><span data-ttu-id="f0b1a-173">Désignation</span><span class="sxs-lookup"><span data-stu-id="f0b1a-173">Description</span></span></th>
    </tr>
    <tr>
    <td><span data-ttu-id="f0b1a-174">**Livraisons**</span><span class="sxs-lookup"><span data-stu-id="f0b1a-174">**Shipments**</span></span></td>
    <td><span data-ttu-id="f0b1a-175">Livraisons validées associées à la ligne sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-175">Posted shipments associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="f0b1a-176">**Factures**</span><span class="sxs-lookup"><span data-stu-id="f0b1a-176">**Invoices**</span></span></td>
    <td><span data-ttu-id="f0b1a-177">Factures validées associées à la ligne sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-177">Posted invoices associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="f0b1a-178">**Réceptions retour**</span><span class="sxs-lookup"><span data-stu-id="f0b1a-178">**Return Receipts**</span></span></td>
    <td><span data-ttu-id="f0b1a-179">Réceptions retour validées associés à la ligne sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-179">Posted return receipts that have been associated with the selected line.</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="f0b1a-180">**Avoirs**</span><span class="sxs-lookup"><span data-stu-id="f0b1a-180">**Credit Memos**</span></span></td>
    <td><span data-ttu-id="f0b1a-181">Avoirs validés associés à la ligne sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-181">Posted credit memos that have been associated with the selected line.</span></span></td>
    </tr>
    </table><span data-ttu-id="f0b1a-182">
5. Dans la fenêtre **Lignes vente**, sélectionnez l'action **Afficher document** pour afficher l'écriture.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-182">
5. In the **Sales Lines** window, choose the **Show Document** action to view the entry.</span></span>

## <a name="see-also"></a><span data-ttu-id="f0b1a-183">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f0b1a-183">See Also</span></span>
[<span data-ttu-id="f0b1a-184">Ventes</span><span class="sxs-lookup"><span data-stu-id="f0b1a-184">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="f0b1a-185">Définition des ventes</span><span class="sxs-lookup"><span data-stu-id="f0b1a-185">Setting Up Sales</span></span>](sales-setup-sales.md)  
<span data-ttu-id="f0b1a-186">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f0b1a-186">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
