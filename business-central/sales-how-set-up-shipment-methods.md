---
title: Procédure de configuration des méthodes d'expédition | Microsoft Docs
description: Vous pouvez définir un code pour chacune de vos méthodes d'expédition offertes, par exemple, saisir les informations qui les concernent.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoterms
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: be65cd62cec984cd2571b6e88998dc169741f376
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/01/2019
ms.locfileid: "2312075"
---
# <a name="set-up-shipment-methods"></a><span data-ttu-id="6cc7a-103">Configurer des conditions de livraison</span><span class="sxs-lookup"><span data-stu-id="6cc7a-103">Set Up Shipment Methods</span></span>
<span data-ttu-id="6cc7a-104">Les conditions de livraison, également appelées incoterms, dépendent souvent des articles, des clients et des fournisseurs.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-104">Shipment methods, also called incoterms, often depend on the items, the customers, and the vendors.</span></span> <span data-ttu-id="6cc7a-105">Par exemple, si le client habite sur une île, il peut choisir d'être toujours livré par voie aérienne ou maritime.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-105">For example, if the customer lives on an island, they can choose to have items always shipped by air or always by sea.</span></span> <span data-ttu-id="6cc7a-106">Certains clients peuvent exiger une livraison le lendemain.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-106">Some customers may require next day delivery.</span></span> <span data-ttu-id="6cc7a-107">Certains voudront peut-être récupérer la commande.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-107">Some may want to pick up the order.</span></span> <span data-ttu-id="6cc7a-108">Vous pouvez spécifier le type de livraison souhaité sur les fiches client et les fiches fournisseur.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-108">On the customer and vendor cards, you can specify what sort of delivery is desired.</span></span>

<span data-ttu-id="6cc7a-109">Vous définissez la désignation et le code de chaque condition de livraison sur la page **Conditions de livraison**.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-109">You set up the description and code for each shipment method on the **Shipment Methods** page.</span></span> <span data-ttu-id="6cc7a-110">Par exemple, vous définissez le code F.O.B., et saisissez Franco bord dans le champ **Désignation**.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-110">For example, you can set up the code FOB, and enter Free on Board in the **Description** field.</span></span> <span data-ttu-id="6cc7a-111">Vous pouvez ensuite saisir ce code dans les champs **Code de méthode de livraison** ailleurs dans le système, par exemple sur une fiche client.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-111">You can then enter the code in **Shipment Method Code** fields elsewhere in the system, such as on a customer card.</span></span> <span data-ttu-id="6cc7a-112">Ensuite, lorsque vous créez des commandes, des factures, des avoirs, etc., le système copie la désignation représentée par le code.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-112">Then when you create new orders, invoices, credit memos, and so on, the system will enter the description represented by the code.</span></span> <span data-ttu-id="6cc7a-113">Au besoin, vous pouvez le modifier sur le document.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-113">You can change it on the document as needed.</span></span>

## <a name="to-set-up-a-shipment-code"></a><span data-ttu-id="6cc7a-114">Pour configurer un code de livraison</span><span class="sxs-lookup"><span data-stu-id="6cc7a-114">To set up a shipment code</span></span>
1. <span data-ttu-id="6cc7a-115">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Modes de livraison**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Shipment Methods**, and then choose the related link.</span></span>
2. <span data-ttu-id="6cc7a-116">Sur la page **Conditions de livraison**, sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-116">On the **Shipment Methods** page, choose the **New** action.</span></span>
3. <span data-ttu-id="6cc7a-117">Sur la nouvelle ligne, indiquez un code et une description pour les conditions de livraison.</span><span class="sxs-lookup"><span data-stu-id="6cc7a-117">On the new line, specify a code and description for the shipment method.</span></span>

## <a name="see-also"></a><span data-ttu-id="6cc7a-118">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6cc7a-118">See Also</span></span>
[<span data-ttu-id="6cc7a-119">Incoterms</span><span class="sxs-lookup"><span data-stu-id="6cc7a-119">Incoterms</span></span>](https://iccwbo.org/resources-for-business/incoterms-rules)  
[<span data-ttu-id="6cc7a-120">Configurer des transporteurs</span><span class="sxs-lookup"><span data-stu-id="6cc7a-120">Set Up Shipping Agents</span></span>](sales-how-to-set-up-shipping-agents.md)  
<span data-ttu-id="6cc7a-121">[Suivre des colis](sales-how-track-packages.md)  </span><span class="sxs-lookup"><span data-stu-id="6cc7a-121">[Track Packages](sales-how-track-packages.md)  </span></span>  
[<span data-ttu-id="6cc7a-122">Gestion d’entrepôt</span><span class="sxs-lookup"><span data-stu-id="6cc7a-122">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="6cc7a-123">Stock</span><span class="sxs-lookup"><span data-stu-id="6cc7a-123">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="6cc7a-124">[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="6cc7a-124">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="6cc7a-125">[Gestion des assemblages](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="6cc7a-125">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="6cc7a-126">Détails de conception : gestion d'entrepôt</span><span class="sxs-lookup"><span data-stu-id="6cc7a-126">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="6cc7a-127">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6cc7a-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  