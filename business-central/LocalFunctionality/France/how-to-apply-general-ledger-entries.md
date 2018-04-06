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
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: bc30859b6ce5487b248925aa2de0afbc495c2518
ms.contentlocale: fr-fr
ms.lasthandoff: 03/22/2018

---
# <a name="apply-general-ledger-entries"></a><span data-ttu-id="8b9b3-103">Lettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="8b9b3-103">Apply General Ledger Entries</span></span>
<span data-ttu-id="8b9b3-104">Vous lettrez les écritures comptables pour justifier les soldes des comptes d'actif et de passif.</span><span class="sxs-lookup"><span data-stu-id="8b9b3-104">You apply general ledger entries to justify ledger balances on asset and liability accounts.</span></span> <span data-ttu-id="8b9b3-105">Par exemple, vous pouvez lettrer des transactions dans les comptes de lettre de change afin d'obtenir une image précise des lettres constituant le solde du compte.</span><span class="sxs-lookup"><span data-stu-id="8b9b3-105">For example, you can apply transactions on the bill of exchange accounts to get a clear picture of which bills make up the balance of the account.</span></span>  

## <a name="to-apply-general-ledger-entries"></a><span data-ttu-id="8b9b3-106">Pour lettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="8b9b3-106">To apply general ledger entries</span></span>  

1.  <span data-ttu-id="8b9b3-107">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Plan comptable**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="8b9b3-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8b9b3-108">Dans la fenêtre **Plan comptable**, sélectionnez le compte dont vous souhaitez lettrer les écritures, puis choisissez l'action **Écritures ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="8b9b3-108">In the **Chart of Accounts** window, select the account that you want to apply entries for, and then choose the **Apply Entries** action.</span></span>  
3.  <span data-ttu-id="8b9b3-109">Dans la fenêtre **Lettrage écritures comptables**, sélectionnez les écritures comptables à lettrer.</span><span class="sxs-lookup"><span data-stu-id="8b9b3-109">In the **Apply G/L Entries** window, select the ledger entries that you want to apply.</span></span>  
4.  <span data-ttu-id="8b9b3-110">Choisissez **Définir ID lettrage** pour remplir le champ ID lettrage avec le code de l'utilisateur actuel.</span><span class="sxs-lookup"><span data-stu-id="8b9b3-110">Choose the **Set Applies-to ID** action to populate the Applies-to ID field with the user ID of the current user.</span></span>  
5.  <span data-ttu-id="8b9b3-111">Sélectionnez l'action **Valider le lettrage**.</span><span class="sxs-lookup"><span data-stu-id="8b9b3-111">Choose the **Post Application** action.</span></span>  

<span data-ttu-id="8b9b3-112">Le lettrage est effectué en définissant les champ Lettre et Date de la lettre.</span><span class="sxs-lookup"><span data-stu-id="8b9b3-112">This effectuates the application by setting the Letter and Letter Date fields.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="8b9b3-113">Les écritures lettrées sont identifiées par la même combinaison de trois lettres et la même date.</span><span class="sxs-lookup"><span data-stu-id="8b9b3-113">Applied entries will be identified by the same three-letter combination and the same date.</span></span> <span data-ttu-id="8b9b3-114">Les écritures équilibrées reçoivent uniquement des lettres majuscules, et les écritures non équilibrées se voient affecter des lettres minuscules.</span><span class="sxs-lookup"><span data-stu-id="8b9b3-114">Balanced entries will be assigned only uppercase letters, and unbalanced entries will be assigned only lowercase letters.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8b9b3-115">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8b9b3-115">See Also</span></span>  
 [<span data-ttu-id="8b9b3-116">Délettrer des écritures comptables</span><span class="sxs-lookup"><span data-stu-id="8b9b3-116">Unapply General Ledger Entries</span></span>](how-to-unapply-general-ledger-entries.md)

