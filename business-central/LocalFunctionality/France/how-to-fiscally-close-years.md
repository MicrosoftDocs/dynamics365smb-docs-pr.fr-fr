---
title: Procédure de clôture fiscale des exercices
description: Lorsqu'un exercice comptable est terminé, vous devez clôturer fiscalement les périodes qui le composent pour veiller à ce qu'aucune autre écriture comptable ne puisse être validée.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 44c3cb6c63cae2e528ef012650a2afad07c8c1ff
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2019
ms.locfileid: "826629"
---
# <a name="fiscally-close-years"></a><span data-ttu-id="1188d-103">Clôturer fiscalement des exercices</span><span class="sxs-lookup"><span data-stu-id="1188d-103">Fiscally Close Years</span></span>
<span data-ttu-id="1188d-104">Lorsqu'un exercice comptable est terminé, vous devez clôturer fiscalement les périodes qui le composent pour veiller à ce qu'aucune autre écriture comptable ne puisse être validée.</span><span class="sxs-lookup"><span data-stu-id="1188d-104">When a fiscal year is complete, you must fiscally close the periods that it comprises to make sure that no more general ledger entries can be posted.</span></span>  

<span data-ttu-id="1188d-105">Avant que la clôture fiscale ne soit autorisée, vous devez vérifier ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="1188d-105">Before fiscal closing is allowed the following must be done:</span></span>  

- <span data-ttu-id="1188d-106">l'exercice comptable a été préalablement clôturé ;</span><span class="sxs-lookup"><span data-stu-id="1188d-106">The fiscal year has been closed first.</span></span> <span data-ttu-id="1188d-107">Pour plus d'informations, voir [Clôture des exercices](how-to-close-years.md).</span><span class="sxs-lookup"><span data-stu-id="1188d-107">For more information, see [Close Years](how-to-close-years.md).</span></span>  
- <span data-ttu-id="1188d-108">toutes les lignes feuille non validées pour l'exercice sont validées ou supprimées avant la clôture fiscale de l'exercice ;</span><span class="sxs-lookup"><span data-stu-id="1188d-108">All journal lines that are not posted for the year are either posted or deleted before the year is fiscally closed.</span></span>
- <span data-ttu-id="1188d-109">toutes les écritures de clôture sont à jour.</span><span class="sxs-lookup"><span data-stu-id="1188d-109">All closing entries are up-to-date.</span></span>  

## <a name="to-fiscally-close-years"></a><span data-ttu-id="1188d-110">Pour clôturer fiscalement des exercices</span><span class="sxs-lookup"><span data-stu-id="1188d-110">To fiscally close years</span></span>  

1.  <span data-ttu-id="1188d-111">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Périodes comptables**, puis sélectionnez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="1188d-111">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Accounting Periods**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="1188d-112">Sous l'onglet **Naviguer**, dans le groupe **Clôture fiscale**, choisissez la case à cocher **Clôturer l'exercice fiscalement**.</span><span class="sxs-lookup"><span data-stu-id="1188d-112">On the **Navigate** tab, in the **Fiscal Closing** group, choose the **Fiscally Close Year** check box.</span></span>  

    <span data-ttu-id="1188d-113">Si plusieurs exercices comptables ne sont pas clôturés fiscalement, le plus ancien doit être clôturé.</span><span class="sxs-lookup"><span data-stu-id="1188d-113">If more than one fiscal year is not fiscally closed, the earliest one should be fiscally closed.</span></span> <span data-ttu-id="1188d-114">Un message s'affiche pour identifier l'exercice à clôturer. Il détaille également les conséquences de cette opération.</span><span class="sxs-lookup"><span data-stu-id="1188d-114">A message appears that identifies the year that should be closed and explains the consequences of closing it.</span></span>  

3.  <span data-ttu-id="1188d-115">Pour clôturer fiscalement l'exercice, cliquez sur le bouton **Oui**.</span><span class="sxs-lookup"><span data-stu-id="1188d-115">To fiscally close the year, choose the **Yes** button.</span></span>  

<span data-ttu-id="1188d-116">Lorsque l'exercice comptable est clôturé fiscalement, le champ **Clôturé fiscalement** est sélectionné pour toutes les périodes de l'exercice.</span><span class="sxs-lookup"><span data-stu-id="1188d-116">When the fiscal year is fiscally closed, the **Fiscally Closed** field for all the periods in the year is selected.</span></span> <span data-ttu-id="1188d-117">Vous ne pouvez plus rouvrir l'exercice clôturé fiscalement, ni désactiver le champ **Clôturé fiscalement**.</span><span class="sxs-lookup"><span data-stu-id="1188d-117">The fiscally closed year cannot be opened again, and you cannot clear the **Fiscally Closed** field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1188d-118">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1188d-118">See Also</span></span>  
 <span data-ttu-id="1188d-119">[Clôturer fiscalement des exercices](how-to-close-years.md) </span><span class="sxs-lookup"><span data-stu-id="1188d-119">[Close Years](how-to-close-years.md) </span></span>  
 <span data-ttu-id="1188d-120">[Vue d'ensemble des processus de fin d'exercice](year-end-processes-overview.md) </span><span class="sxs-lookup"><span data-stu-id="1188d-120">[Year End Processes Overview](year-end-processes-overview.md) </span></span>  
 <span data-ttu-id="1188d-121">[Valider l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md) </span><span class="sxs-lookup"><span data-stu-id="1188d-121">[Post the Year-End Closing Entry](how-to-post-the-year-end-closing-entry.md) </span></span>  
 [<span data-ttu-id="1188d-122">Clôture des exercices et des périodes</span><span class="sxs-lookup"><span data-stu-id="1188d-122">Closing Years and Periods</span></span>](../../year-close-years-periods.md)
