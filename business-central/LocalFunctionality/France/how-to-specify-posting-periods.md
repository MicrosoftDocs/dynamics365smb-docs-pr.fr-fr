---
title: "Procédure de définition des périodes de validation"
description: "En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 44b36ac39a39144a3d8f951e7533fcffdbae0bdb
ms.contentlocale: fr-fr
ms.lasthandoff: 09/28/2018

---
# <a name="specify-posting-periods"></a><span data-ttu-id="4f492-103">Définir des périodes de validation</span><span class="sxs-lookup"><span data-stu-id="4f492-103">Specify Posting Periods</span></span>
<span data-ttu-id="4f492-104">En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée.</span><span class="sxs-lookup"><span data-stu-id="4f492-104">When you specify posting periods, you limit the period in which posting is allowed.</span></span>  

## <a name="to-specify-posting-periods"></a><span data-ttu-id="4f492-105">Pour définir des périodes de validation</span><span class="sxs-lookup"><span data-stu-id="4f492-105">To specify posting periods</span></span>  

1.  <span data-ttu-id="4f492-106">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="4f492-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4f492-107">Dans la fenêtre **Paramètres comptabilité**, sous l'onglet **Général**, dans le champ **Début période validation**, spécifiez la date de début de la période de validation.</span><span class="sxs-lookup"><span data-stu-id="4f492-107">In the **General Ledger Setup** window, on the **General** tab, in the **Allow Posting From** field, specify the start date of the posting period.</span></span>  
3.  <span data-ttu-id="4f492-108">Dans le champ **Fin période validation**, spécifiez la date de fin de la période de validation.</span><span class="sxs-lookup"><span data-stu-id="4f492-108">In the **Allow Posting To** field, specify the end date of the posting period.</span></span>  

    <span data-ttu-id="4f492-109">Les dates sont validées dans les plages de validation autorisées pour garantir leur appartenance aux exercices comptables ouverts.</span><span class="sxs-lookup"><span data-stu-id="4f492-109">The dates are validated against the allowed posting ranges to make sure that they belong to open fiscal years.</span></span> <span data-ttu-id="4f492-110">Pour plus d'informations, voir Plage de validation autorisée.</span><span class="sxs-lookup"><span data-stu-id="4f492-110">For more information, see Allowed Posting Range.</span></span>  

4.  <span data-ttu-id="4f492-111">Pour vérifier quelle est la plage de validation autorisée, choisissez l'action **Extraire plage de validation autorisée**.</span><span class="sxs-lookup"><span data-stu-id="4f492-111">To verify what the allowed posting range is, choose the **Get Allowed Posting Range** action.</span></span>  

<span data-ttu-id="4f492-112">Les dates définies ici s'appliquent à l'ensemble de la société, c'est-à-dire à tous les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="4f492-112">The dates that you define here apply to the whole company, that is, to all users.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="4f492-113">Vous pouvez définir différentes périodes de comptabilisation pour divers utilisateurs et appliquer une période de validation à un utilisateur dans la fenêtre **Paramètres utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="4f492-113">You can define different posting periods for different users and apply a posting period to a user in the **User Setup** window.</span></span>

<span data-ttu-id="4f492-114">Si vous entrez des dates ici, les dates entrées sous l'onglet **Général** de la fenêtre **Paramètres comptabilité** ne s'appliquent pas à ces utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="4f492-114">If you enter dates here, the dates entered on the **General** tab in the **General Ledger Setup** window will not apply to these users.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4f492-115">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4f492-115">See Also</span></span>  
 [<span data-ttu-id="4f492-116">Périodes fiscales et exercices comptables</span><span class="sxs-lookup"><span data-stu-id="4f492-116">Fiscal Periods and Fiscal Years</span></span>](fiscal-periods-and-fiscal-years.md)

