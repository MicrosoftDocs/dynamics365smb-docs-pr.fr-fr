---
title: Procédure de lettrage des écritures comptables
description: Vous lettrez les écritures comptables pour justifier les soldes des comptes d'actif et de passif.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 5c644201f884efad83333bb4fc29879386191c0e
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301352"
---
# <a name="apply-general-ledger-entries"></a><span data-ttu-id="59766-103">Lettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="59766-103">Apply General Ledger Entries</span></span>
<span data-ttu-id="59766-104">Vous lettrez les écritures comptables pour justifier les soldes des comptes d'actif et de passif.</span><span class="sxs-lookup"><span data-stu-id="59766-104">You apply general ledger entries to justify ledger balances on asset and liability accounts.</span></span> <span data-ttu-id="59766-105">Par exemple, vous pouvez lettrer des transactions dans les comptes de lettre de change afin d'obtenir une image précise des lettres constituant le solde du compte.</span><span class="sxs-lookup"><span data-stu-id="59766-105">For example, you can apply transactions on the bill of exchange accounts to get a clear picture of which bills make up the balance of the account.</span></span>  

## <a name="to-apply-general-ledger-entries"></a><span data-ttu-id="59766-106">Pour lettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="59766-106">To apply general ledger entries</span></span>  

1.  <span data-ttu-id="59766-107">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Plan comptable**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="59766-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="59766-108">Sur la page **Plan comptable**, sélectionnez le compte dans lequel vous souhaitez lettrer les écritures, puis choisissez l'action **Écritures ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="59766-108">On the **Chart of Accounts** page, select the account that you want to apply entries for, and then choose the **Apply Entries** action.</span></span>  
3.  <span data-ttu-id="59766-109">Sur la page **Lettrage écritures comptables**, sélectionnez les écritures comptables à lettrer.</span><span class="sxs-lookup"><span data-stu-id="59766-109">On the **Apply G/L Entries** page, select the ledger entries that you want to apply.</span></span>  
4.  <span data-ttu-id="59766-110">Choisissez **Définir ID lettrage** pour remplir le champ **ID lettrage** avec le code de l'utilisateur actuel.</span><span class="sxs-lookup"><span data-stu-id="59766-110">Choose the **Set Applies-to ID** action to populate the **Applies-to ID** field with the user ID of the current user.</span></span>  
5.  <span data-ttu-id="59766-111">Sélectionnez l'action **Valider le lettrage**.</span><span class="sxs-lookup"><span data-stu-id="59766-111">Choose the **Post Application** action.</span></span>  

<span data-ttu-id="59766-112">Le lettrage est effectué en définissant les champ **Lettre** et **Date de la lettre**.</span><span class="sxs-lookup"><span data-stu-id="59766-112">This effectuates the application by setting the **Letter** and **Letter Date** fields.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="59766-113">les écritures lettrées peuvent être identifiées par la même combinaison de trois lettres et la même date.</span><span class="sxs-lookup"><span data-stu-id="59766-113">Applied entries can be identified by having the same three-letter combination and the same date.</span></span>

## <a name="see-also"></a><span data-ttu-id="59766-114">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59766-114">See Also</span></span>  
[<span data-ttu-id="59766-115">Délettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="59766-115">Unapply General Ledger Entries</span></span>](how-to-unapply-general-ledger-entries.md)  
[<span data-ttu-id="59766-116">Lettrer les paiements fournisseur manuellement</span><span class="sxs-lookup"><span data-stu-id="59766-116">Apply Vendor Payments Manually</span></span>](../../payables-how-apply-purchase-transactions-manually.md)
