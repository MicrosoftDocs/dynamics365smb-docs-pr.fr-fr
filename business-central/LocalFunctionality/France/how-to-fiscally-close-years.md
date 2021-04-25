---
title: Procédure de clôture fiscale des exercices
description: Lorsqu'un exercice comptable est terminé, vous devez clôturer fiscalement les périodes qui le composent pour veiller à ce qu'aucune autre écriture comptable ne puisse être validée.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 4b775f39f62f0fac7247a5fa44ca2d92a1155ba9
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5784649"
---
# <a name="fiscally-close-years"></a><span data-ttu-id="fad9f-103">Clôturer fiscalement des exercices</span><span class="sxs-lookup"><span data-stu-id="fad9f-103">Fiscally Close Years</span></span>
<span data-ttu-id="fad9f-104">Lorsqu'un exercice comptable est terminé, vous devez clôturer fiscalement les périodes qui le composent pour veiller à ce qu'aucune autre écriture comptable ne puisse être validée.</span><span class="sxs-lookup"><span data-stu-id="fad9f-104">When a fiscal year is complete, you must fiscally close the periods that it comprises to make sure that no more general ledger entries can be posted.</span></span>  

<span data-ttu-id="fad9f-105">Avant que la clôture fiscale ne soit autorisée, vous devez vérifier ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="fad9f-105">Before fiscal closing is allowed the following must be done:</span></span>  

- <span data-ttu-id="fad9f-106">l'exercice comptable a été préalablement clôturé ;</span><span class="sxs-lookup"><span data-stu-id="fad9f-106">The fiscal year has been closed first.</span></span> <span data-ttu-id="fad9f-107">Pour plus d'informations, voir [Clôture des exercices](how-to-close-years.md).</span><span class="sxs-lookup"><span data-stu-id="fad9f-107">For more information, see [Close Years](how-to-close-years.md).</span></span>  
- <span data-ttu-id="fad9f-108">toutes les lignes feuille non validées pour l'exercice sont validées ou supprimées avant la clôture fiscale de l'exercice ;</span><span class="sxs-lookup"><span data-stu-id="fad9f-108">All journal lines that are not posted for the year are either posted or deleted before the year is fiscally closed.</span></span>
- <span data-ttu-id="fad9f-109">toutes les écritures de clôture sont à jour.</span><span class="sxs-lookup"><span data-stu-id="fad9f-109">All closing entries are up-to-date.</span></span>  

## <a name="to-fiscally-close-years"></a><span data-ttu-id="fad9f-110">Pour clôturer fiscalement des exercices</span><span class="sxs-lookup"><span data-stu-id="fad9f-110">To fiscally close years</span></span>  

1.  <span data-ttu-id="fad9f-111">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Périodes comptables**, puis choisissez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="fad9f-111">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Accounting Periods**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="fad9f-112">Sélectionnez la case à cocher **Clôturer l'exercice fiscalement**.</span><span class="sxs-lookup"><span data-stu-id="fad9f-112">Choose the **Fiscally Close Year** check box.</span></span>  

    <span data-ttu-id="fad9f-113">Si plusieurs exercices comptables ne sont pas clôturés fiscalement, le plus ancien doit être clôturé.</span><span class="sxs-lookup"><span data-stu-id="fad9f-113">If more than one fiscal year is not fiscally closed, the earliest one should be fiscally closed.</span></span> <span data-ttu-id="fad9f-114">Un message s'affiche pour identifier l'exercice à clôturer. Il détaille également les conséquences de cette opération.</span><span class="sxs-lookup"><span data-stu-id="fad9f-114">A message appears that identifies the year that should be closed and explains the consequences of closing it.</span></span>  

3.  <span data-ttu-id="fad9f-115">Pour clôturer fiscalement l'exercice, cliquez sur le bouton **Oui**.</span><span class="sxs-lookup"><span data-stu-id="fad9f-115">To fiscally close the year, choose the **Yes** button.</span></span>  

<span data-ttu-id="fad9f-116">Lorsque l'exercice comptable est clôturé fiscalement, le champ **Clôturé fiscalement** est sélectionné pour toutes les périodes de l'exercice.</span><span class="sxs-lookup"><span data-stu-id="fad9f-116">When the fiscal year is fiscally closed, the **Fiscally Closed** field for all the periods in the year is selected.</span></span> <span data-ttu-id="fad9f-117">Vous ne pouvez plus rouvrir l'exercice clôturé fiscalement, ni désactiver le champ **Clôturé fiscalement**.</span><span class="sxs-lookup"><span data-stu-id="fad9f-117">The fiscally closed year cannot be opened again, and you cannot clear the **Fiscally Closed** field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fad9f-118">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fad9f-118">See Also</span></span>  
 <span data-ttu-id="fad9f-119">[Clôturer fiscalement des exercices](how-to-close-years.md) </span><span class="sxs-lookup"><span data-stu-id="fad9f-119">[Close Years](how-to-close-years.md) </span></span>  
 <span data-ttu-id="fad9f-120">[Vue d'ensemble des processus de fin d'exercice](year-end-processes-overview.md) </span><span class="sxs-lookup"><span data-stu-id="fad9f-120">[Year End Processes Overview](year-end-processes-overview.md) </span></span>  
 <span data-ttu-id="fad9f-121">[Valider l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md) </span><span class="sxs-lookup"><span data-stu-id="fad9f-121">[Post the Year-End Closing Entry](how-to-post-the-year-end-closing-entry.md) </span></span>  
 [<span data-ttu-id="fad9f-122">Clôture des exercices et des périodes</span><span class="sxs-lookup"><span data-stu-id="fad9f-122">Closing Years and Periods</span></span>](../../year-close-years-periods.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]