---
title: "Procédure de lettrage des écritures comptables"
description: "Vous lettrez les écritures comptables pour justifier les soldes des comptes d'actif et de passif."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/14/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 5ccb9953c331e285770d72f560aad63e3f26bbfb
ms.contentlocale: fr-fr
ms.lasthandoff: 11/26/2018

---
# <a name="apply-general-ledger-entries"></a><span data-ttu-id="ffb16-103">Lettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="ffb16-103">Apply General Ledger Entries</span></span>
<span data-ttu-id="ffb16-104">Vous lettrez les écritures comptables pour justifier les soldes des comptes d'actif et de passif.</span><span class="sxs-lookup"><span data-stu-id="ffb16-104">You apply general ledger entries to justify ledger balances on asset and liability accounts.</span></span> <span data-ttu-id="ffb16-105">Par exemple, vous pouvez lettrer des transactions dans les comptes de lettre de change afin d'obtenir une image précise des lettres constituant le solde du compte.</span><span class="sxs-lookup"><span data-stu-id="ffb16-105">For example, you can apply transactions on the bill of exchange accounts to get a clear picture of which bills make up the balance of the account.</span></span>  

## <a name="to-apply-general-ledger-entries"></a><span data-ttu-id="ffb16-106">Pour lettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="ffb16-106">To apply general ledger entries</span></span>  

1.  <span data-ttu-id="ffb16-107">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Plan comptable**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="ffb16-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ffb16-108">Sur la page **Plan comptable**, sélectionnez le compte dans lequel vous souhaitez lettrer les écritures, puis choisissez l'action **Écritures ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="ffb16-108">On the **Chart of Accounts** page, select the account that you want to apply entries for, and then choose the **Apply Entries** action.</span></span>  
3.  <span data-ttu-id="ffb16-109">Sur la page **Lettrage écritures comptables**, sélectionnez les écritures comptables à lettrer.</span><span class="sxs-lookup"><span data-stu-id="ffb16-109">On the **Apply G/L Entries** page, select the ledger entries that you want to apply.</span></span>  
4.  <span data-ttu-id="ffb16-110">Choisissez **Définir ID lettrage** pour remplir le champ **ID lettrage** avec le code de l'utilisateur actuel.</span><span class="sxs-lookup"><span data-stu-id="ffb16-110">Choose the **Set Applies-to ID** action to populate the **Applies-to ID** field with the user ID of the current user.</span></span>  
5.  <span data-ttu-id="ffb16-111">Sélectionnez l'action **Valider le lettrage**.</span><span class="sxs-lookup"><span data-stu-id="ffb16-111">Choose the **Post Application** action.</span></span>  

<span data-ttu-id="ffb16-112">Le lettrage est effectué en définissant les champ **Lettre** et **Date de la lettre**.</span><span class="sxs-lookup"><span data-stu-id="ffb16-112">This effectuates the application by setting the **Letter** and **Letter Date** fields.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="ffb16-113">les écritures lettrées peuvent être identifiées par la même combinaison de trois lettres et la même date.</span><span class="sxs-lookup"><span data-stu-id="ffb16-113">Applied entries can be identified by having the same three-letter combination and the same date.</span></span>

## <a name="see-also"></a><span data-ttu-id="ffb16-114">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ffb16-114">See Also</span></span>  
[<span data-ttu-id="ffb16-115">Délettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="ffb16-115">Unapply General Ledger Entries</span></span>](how-to-unapply-general-ledger-entries.md)  
[<span data-ttu-id="ffb16-116">Lettrer les paiements fournisseur manuellement</span><span class="sxs-lookup"><span data-stu-id="ffb16-116">Apply Vendor Payments Manually</span></span>](../../payables-how-apply-purchase-transactions-manually.md)

