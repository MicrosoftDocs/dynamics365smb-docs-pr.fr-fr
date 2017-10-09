---
title: "Procédure : Établissement d'un devis de vente Assembler pour commande | Microsoft Docs"
description: "Vous pouvez utiliser la gestion nomenclature d'assemblage pour personnaliser un élément d'assemblage sur la demande d'un client au cours du processus de vente."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7602b067e4b3fc99815a581c851138d7cc3ff41e
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-quote-an-assemble-to-order-sale"></a><span data-ttu-id="1cb71-103">Procédure : Établissement d'un devis de vente Assembler pour commande</span><span class="sxs-lookup"><span data-stu-id="1cb71-103">How to: Quote an Assemble-to-Order Sale</span></span>
<span data-ttu-id="1cb71-104">Vous pouvez utiliser la gestion nomenclature d'assemblage pour personnaliser un élément d'assemblage sur la demande d'un client au cours du processus de vente.</span><span class="sxs-lookup"><span data-stu-id="1cb71-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="1cb71-105">Pour plus d'informations sur le paramétrage des éléments d'assemblage, voir [Procédure : Vente d'articles à assembler pour commande](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="1cb71-105">For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

<span data-ttu-id="1cb71-106">Lorsque vous vendez tout autre type d'article, vous pouvez également créer un devis pour un élément d'assemblage personnalisé avant de le convertir en commande vente.</span><span class="sxs-lookup"><span data-stu-id="1cb71-106">As when you sell any other type of item, you can also create a sales quote for a customized assembly item before converting it to a sales order.</span></span> <span data-ttu-id="1cb71-107">Ce processus implique plusieurs étapes supplémentaires lorsque vous le comparez à la création d'un devis normal et il recourt à une variation d'un ordre d'assemblage associé, qui est un devis d'assemblage.</span><span class="sxs-lookup"><span data-stu-id="1cb71-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span></span>

> [!NOTE]  
>  <span data-ttu-id="1cb71-108">Comme tous les types de devis, les quantités sur les devis d'assemblage ne sont pas utilisées en termes de disponibilité, planification ou réservations.</span><span class="sxs-lookup"><span data-stu-id="1cb71-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span></span>  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a><span data-ttu-id="1cb71-109">Créer un devis pour un article à assembler pour commande</span><span class="sxs-lookup"><span data-stu-id="1cb71-109">To create a sales quote for an assemble-to-order item</span></span>  
1.  <span data-ttu-id="1cb71-110">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Devis**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="1cb71-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Quote**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="1cb71-111">Créez une ligne devis avec une ligne pour un élément d'assemblage.</span><span class="sxs-lookup"><span data-stu-id="1cb71-111">Create a sales quote line with one line for an assembly item.</span></span> <span data-ttu-id="1cb71-112">Pour plus d'informations, voir [Procédure : créer des offres](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="1cb71-112">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span></span>  
3.  <span data-ttu-id="1cb71-113">Dans le champ **Quantité à assembler pour commande**, entrez la quantité entière.</span><span class="sxs-lookup"><span data-stu-id="1cb71-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="1cb71-114">Vous ne devez pas établir un devis pour une quantité partielle.</span><span class="sxs-lookup"><span data-stu-id="1cb71-114">You should not quote a partial quantity.</span></span> <span data-ttu-id="1cb71-115">Par conséquent, vous devez entrer la même quantité que vous avez saisie dans le champ **Quantité** de la ligne devis.</span><span class="sxs-lookup"><span data-stu-id="1cb71-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span></span>  

4.  <span data-ttu-id="1cb71-116">Sur le raccourci **Lignes**, sélectionnez **Ligne**, puis **Assembler pour commande** et **Lignes d'assemblage pour commande**.</span><span class="sxs-lookup"><span data-stu-id="1cb71-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span></span> <span data-ttu-id="1cb71-117">Sinon, choisissez le champ **Quantité à assembler pour commande** sur la ligne.</span><span class="sxs-lookup"><span data-stu-id="1cb71-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span></span>  
5.  <span data-ttu-id="1cb71-118">Dans la fenêtre **Lignes d'assemblage pour commande**, vérifiez ou modifiez les lignes d'assemblage pour commande en fonction du devis demandé par le client.</span><span class="sxs-lookup"><span data-stu-id="1cb71-118">In the **Assemble-to-Order Lines** window, review or modify the assembly order lines according to the quote that the customer is requesting.</span></span> <span data-ttu-id="1cb71-119">Des informations supplémentaires sont disponibles en choisissant **Afficher document** pour ouvrir la commande devis ouverte complète.</span><span class="sxs-lookup"><span data-stu-id="1cb71-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span></span> <span data-ttu-id="1cb71-120">Vous ne pouvez pas modifier le contenu de la plupart des champs, et vous ne pouvez pas valider.</span><span class="sxs-lookup"><span data-stu-id="1cb71-120">You cannot change the contents of most fields, and you cannot post.</span></span>  
6.  <span data-ttu-id="1cb71-121">Lorsque vous avez ajusté les lignes d'ordre d'assemblage en fonction du devis, fermez la fenêtre **Lignes d'assemblage pour commande** pour revenir à la fenêtre **Devis**.</span><span class="sxs-lookup"><span data-stu-id="1cb71-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** window to return to the **Sales Quote** window.</span></span>  
7.  <span data-ttu-id="1cb71-122">Si le client accepte le devis, créez une commande vente pour l'élément d'assemblage qui a fait l'objet du devis.</span><span class="sxs-lookup"><span data-stu-id="1cb71-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span></span> <span data-ttu-id="1cb71-123">Pour plus d'informations, voir [Procédure : créer des offres](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="1cb71-123">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span></span> <span data-ttu-id="1cb71-124">Le devis d'assemblage associé et toutes les personnalisations sont liées à cette nouvelle commande vente à préparer pour l'assemblage de l'article ou des articles à vendre.</span><span class="sxs-lookup"><span data-stu-id="1cb71-124">The linked assembly quote and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1cb71-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1cb71-125">See Also</span></span>  
[<span data-ttu-id="1cb71-126">Gestion des assemblages</span><span class="sxs-lookup"><span data-stu-id="1cb71-126">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="1cb71-127">Procédure : utiliser les nomenclatures</span><span class="sxs-lookup"><span data-stu-id="1cb71-127">How to: Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="1cb71-128">STOCKS ET EN-COURS</span><span class="sxs-lookup"><span data-stu-id="1cb71-128">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="1cb71-129">Détails de conception : gestion d'entrepôt</span><span class="sxs-lookup"><span data-stu-id="1cb71-129">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="1cb71-130">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1cb71-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
