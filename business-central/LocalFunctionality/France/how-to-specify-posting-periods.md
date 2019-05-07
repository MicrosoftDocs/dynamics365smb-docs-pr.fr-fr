---
title: Procédure de définition des périodes de validation
description: En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 97255eed953fb81e2a15829449015d390f9df10a
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2019
ms.locfileid: "913747"
---
# <a name="specify-posting-periods"></a><span data-ttu-id="cc424-103">Définir des périodes de validation</span><span class="sxs-lookup"><span data-stu-id="cc424-103">Specify Posting Periods</span></span>
<span data-ttu-id="cc424-104">En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée.</span><span class="sxs-lookup"><span data-stu-id="cc424-104">When you specify posting periods, you limit the period in which posting is allowed.</span></span>  

## <a name="to-specify-posting-periods"></a><span data-ttu-id="cc424-105">Pour définir des périodes de validation</span><span class="sxs-lookup"><span data-stu-id="cc424-105">To specify posting periods</span></span>  

1.  <span data-ttu-id="cc424-106">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="cc424-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cc424-107">Sur la page **Paramètres comptabilité**, sous l'onglet **Général**, dans le champ **Début période validation**, spécifiez la date de début de la période de validation.</span><span class="sxs-lookup"><span data-stu-id="cc424-107">On the **General Ledger Setup** page, on the **General** tab, in the **Allow Posting From** field, specify the start date of the posting period.</span></span>  
3.  <span data-ttu-id="cc424-108">Dans le champ **Fin période validation**, spécifiez la date de fin de la période de validation.</span><span class="sxs-lookup"><span data-stu-id="cc424-108">In the **Allow Posting To** field, specify the end date of the posting period.</span></span>  

    <span data-ttu-id="cc424-109">Les dates sont validées dans les plages de validation autorisées pour garantir leur appartenance aux exercices comptables ouverts.</span><span class="sxs-lookup"><span data-stu-id="cc424-109">The dates are validated against the allowed posting ranges to make sure that they belong to open fiscal years.</span></span> <span data-ttu-id="cc424-110">Pour plus d'informations, voir Plage de validation autorisée.</span><span class="sxs-lookup"><span data-stu-id="cc424-110">For more information, see Allowed Posting Range.</span></span>  

4.  <span data-ttu-id="cc424-111">Pour vérifier quelle est la plage de validation autorisée, choisissez l'action **Extraire plage de validation autorisée**.</span><span class="sxs-lookup"><span data-stu-id="cc424-111">To verify what the allowed posting range is, choose the **Get Allowed Posting Range** action.</span></span>  

<span data-ttu-id="cc424-112">Les dates définies ici s'appliquent à l'ensemble de la société, c'est-à-dire à tous les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="cc424-112">The dates that you define here apply to the whole company, that is, to all users.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="cc424-113">Vous pouvez définir différentes périodes de comptabilisation pour divers utilisateurs et appliquer une période de validation à un utilisateur sur la page **Paramètres utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="cc424-113">You can define different posting periods for different users and apply a posting period to a user on the **User Setup** page.</span></span>

<span data-ttu-id="cc424-114">Si vous entrez des dates ici, les dates entrées sous l'onglet **Général** sur la page **Paramètres comptabilité** ne s'appliquent pas à ces utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="cc424-114">If you enter dates here, the dates entered on the **General** tab on the **General Ledger Setup** page will not apply to these users.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cc424-115">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cc424-115">See Also</span></span>  
 [<span data-ttu-id="cc424-116">Périodes fiscales et exercices comptables</span><span class="sxs-lookup"><span data-stu-id="cc424-116">Fiscal Periods and Fiscal Years</span></span>](fiscal-periods-and-fiscal-years.md)
