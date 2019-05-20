---
title: Procédure de clôture des exercices
description: Lorsqu'un exercice comptable est terminé, vous devez clôturer les périodes qui le composent.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/01/2017
ms.author: sgroespe
ms.openlocfilehash: 4c7b156320fab12a75e5b16f1a8ca579dfd47685
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/29/2019
ms.locfileid: "1237462"
---
# <a name="close-years"></a><span data-ttu-id="f5b9b-103">Clôturer fiscalement des exercices</span><span class="sxs-lookup"><span data-stu-id="f5b9b-103">Close Years</span></span>
<span data-ttu-id="f5b9b-104">Lorsqu'un exercice comptable est terminé, vous devez clôturer les périodes qui le composent.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-104">When a fiscal year is over, you must close the periods that it comprises.</span></span>  

## <a name="to-close-a-year"></a><span data-ttu-id="f5b9b-105">Pour clôturer un exercice</span><span class="sxs-lookup"><span data-stu-id="f5b9b-105">To close a year</span></span>  
1.  <span data-ttu-id="f5b9b-106">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Périodes comptables**, puis sélectionnez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Accounting Periods**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="f5b9b-107">Choisissez l'action **Clôturer exercice**.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-107">Choose the **Close Year** action.</span></span>  

    <span data-ttu-id="f5b9b-108">Si plusieurs exercices comptables sont ouverts, le plus ancien doit être clôturé.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-108">If more than one fiscal year is open, the earliest one should be closed.</span></span> <span data-ttu-id="f5b9b-109">Un message s'affiche pour identifier l'exercice à clôturer. Il détaille également les conséquences de cette opération.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-109">A message appears to identify the year that should be closed and explains the consequences of closing it.</span></span>  

3.  <span data-ttu-id="f5b9b-110">Pour clôturer l'exercice, cliquez sur **Oui**.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-110">To close the year, choose the **Yes** button.</span></span>  

<span data-ttu-id="f5b9b-111">Lorsque l'exercice comptable est clôturé, les champs **Fermé** et **Verrouillage date** sont sélectionnés pour toutes les périodes de l'exercice.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-111">When the fiscal year is closed, the **Closed** and **Date Locked** fields are selected for all the periods in the year.</span></span> <span data-ttu-id="f5b9b-112">À ce stade, vous ne pouvez pas rouvrir l'exercice comptable, ni désactiver les champs **Fermé** et **Verrouillage date**.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-112">At this point the fiscal year cannot be opened again, and you cannot clear the **Closed** or **Date Locked** fields.</span></span>  

> [!WARNING]  
> <span data-ttu-id="f5b9b-113">Vous ne pouvez pas clôturer un exercice comptable avant d'en créer un nouveau.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-113">You cannot close a fiscal year before you create a new one.</span></span> <span data-ttu-id="f5b9b-114">Lorsqu'un exercice comptable est clôturé, vous ne pouvez pas modifier la date de début de l'exercice comptable suivant.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-114">When a fiscal year has been closed, you cannot change the starting date of the following fiscal year.</span></span>  

<span data-ttu-id="f5b9b-115">Même si un exercice comptable a été clôturé, vous pouvez toujours y valider des écritures comptables jusqu'à ce que vous le clôturiez fiscalement.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-115">Even though a fiscal year has been closed, you can still post general ledger entries to it until you fiscally close the fiscal year.</span></span> <span data-ttu-id="f5b9b-116">Dans ce cas, les écritures sont marquées comme validées dans un exercice comptable clôturé et le champ Ecr. exercice précédent est activé.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-116">When you do this, the entries will be marked as posted to a closed fiscal year, and the Prior-Year Entry field will be selected.</span></span> <span data-ttu-id="f5b9b-117">Pour plus d'informations, voir [Clôturer fiscalement des exercices](how-to-fiscally-close-years.md).</span><span class="sxs-lookup"><span data-stu-id="f5b9b-117">For more information, see [Fiscally Close Years](how-to-fiscally-close-years.md).</span></span>  

<span data-ttu-id="f5b9b-118">Une fois qu'un exercice comptable a été clôturé, vous devez clôturer les comptes de gestion et transférer les résultats de l'exercice sur un compte du bilan.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-118">After a fiscal year is closed, you must close the income statement accounts and transfer the year's results to an account in the balance sheet.</span></span> <span data-ttu-id="f5b9b-119">Vous pouvez répéter cette opération pour chaque validation dans l'exercice comptable clôturé.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-119">You can repeat this each time you post to the closed fiscal year.</span></span>  

<span data-ttu-id="f5b9b-120">Après avoir été clôturé fiscalement, un exercice comptable ne peut plus être rouvert et aucune écriture comptable ne peut y être validée.</span><span class="sxs-lookup"><span data-stu-id="f5b9b-120">After a fiscal year is fiscally closed, it cannot be opened again, and general ledger entries cannot be posted.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f5b9b-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f5b9b-121">See Also</span></span>  
 <span data-ttu-id="f5b9b-122">[Clôturer fiscalement des exercices](how-to-fiscally-close-years.md) </span><span class="sxs-lookup"><span data-stu-id="f5b9b-122">[Fiscally Close Years](how-to-fiscally-close-years.md) </span></span>  
 <span data-ttu-id="f5b9b-123">[Vue d'ensemble des processus de fin d'exercice](year-end-processes-overview.md) </span><span class="sxs-lookup"><span data-stu-id="f5b9b-123">[Year End Processes Overview](year-end-processes-overview.md) </span></span>  
 <span data-ttu-id="f5b9b-124">[Valider l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md) </span><span class="sxs-lookup"><span data-stu-id="f5b9b-124">[Post the Year-End Closing Entry](how-to-post-the-year-end-closing-entry.md) </span></span>  
 [<span data-ttu-id="f5b9b-125">Clôture des exercices et des périodes</span><span class="sxs-lookup"><span data-stu-id="f5b9b-125">Closing Years and Periods</span></span>](../../year-close-years-periods.md)
