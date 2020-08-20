---
title: Périodes fiscales et exercices comptables
description: Un exercice comptable est généralement divisé en 12 périodes fiscales mensuelles. Dans Business Central, deux exercices comptables peuvent être ouverts en même temps.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/15/2020
ms.author: edupont
ms.openlocfilehash: 8b3766aedd7a18a0b2522ff115c8fee00ec72d3f
ms.sourcegitcommit: bdb6d18d512aa76d8d4f477d73ccfb284b0047fc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/21/2020
ms.locfileid: "3611687"
---
# <a name="fiscal-periods-and-fiscal-years"></a><span data-ttu-id="018db-104">Périodes fiscales et exercices comptables</span><span class="sxs-lookup"><span data-stu-id="018db-104">Fiscal Periods and Fiscal Years</span></span>

<span data-ttu-id="018db-105">Un exercice comptable est généralement divisé en 12 périodes fiscales mensuelles.</span><span class="sxs-lookup"><span data-stu-id="018db-105">A fiscal year is typically divided into 12 monthly fiscal periods.</span></span> <span data-ttu-id="018db-106">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], deux exercices comptables peuvent être ouverts en même temps.</span><span class="sxs-lookup"><span data-stu-id="018db-106">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can have two fiscal years open at the same time.</span></span> <span data-ttu-id="018db-107">Vous ne pouvez pas créer un troisième exercice comptable si deux exercices comptables sont ouverts.</span><span class="sxs-lookup"><span data-stu-id="018db-107">You cannot create a third fiscal year if there are two fiscal years open.</span></span>  

<span data-ttu-id="018db-108">Pour clôturer un exercice comptable, vous devez clôturer les périodes comptables de cet exercice.</span><span class="sxs-lookup"><span data-stu-id="018db-108">To close a fiscal year, you must close the accounting periods within that year.</span></span>  

<span data-ttu-id="018db-109">Vous ne pouvez rouvrir une période comptable clôturée que si elle fait partie d'un exercice comptable ouvert.</span><span class="sxs-lookup"><span data-stu-id="018db-109">You can only reopen a closed accounting period if the period falls within an open fiscal year.</span></span> <span data-ttu-id="018db-110">Pour plus d'informations, voir [Clôture des exercices](how-to-close-years.md).</span><span class="sxs-lookup"><span data-stu-id="018db-110">For more information, see [Close Years](how-to-close-years.md).</span></span> <span data-ttu-id="018db-111">Vous ne pouvez pas rouvrir un exercice comptable clôturé.</span><span class="sxs-lookup"><span data-stu-id="018db-111">You cannot reopen a closed fiscal year.</span></span>  

## <a name="closing-fiscal-periods-and-fiscal-years"></a><span data-ttu-id="018db-112">Clôture de périodes fiscales et d'exercices comptables</span><span class="sxs-lookup"><span data-stu-id="018db-112">Closing Fiscal Periods and Fiscal Years</span></span>

<span data-ttu-id="018db-113">À la fin d'un exercice comptable, vous devez clôturer les périodes comptables de cet exercice comptable.</span><span class="sxs-lookup"><span data-stu-id="018db-113">After a fiscal year is complete, you must close the accounting periods within that fiscal year.</span></span> <span data-ttu-id="018db-114">Cela garantit que des écritures comptables ne sont pas validées pour cette période.</span><span class="sxs-lookup"><span data-stu-id="018db-114">This is to ensure that general ledger entries are not posted for that period.</span></span> <span data-ttu-id="018db-115">Pour plus d'informations, voir [Clôturer fiscalement des périodes comptables](how-to-fiscally-close-years.md).</span><span class="sxs-lookup"><span data-stu-id="018db-115">For more information, see [Fiscally Close Accounting Periods](how-to-fiscally-close-years.md).</span></span>  

<span data-ttu-id="018db-116">Un exercice comptable peut être clôturé si tous les critères suivants sont remplis :</span><span class="sxs-lookup"><span data-stu-id="018db-116">A fiscal year can be closed if all of the following criteria are met:</span></span>  

- <span data-ttu-id="018db-117">Les dates comptabilisation sur la page **Paramètres utilisateur** et la page **Paramètres comptabilité** ne font pas partie de l'exercice que vous clôturez.</span><span class="sxs-lookup"><span data-stu-id="018db-117">The posting dates on the **User Setup** page and the **General Ledger Setup** page do not fall within the year that you are closing.</span></span> <span data-ttu-id="018db-118">Pour plus d'informations, consultez [Définir des périodes de validation](../../finance-how-specify-posting-periods.md) et [Description des écritures comptables et du plan comptable](../../finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="018db-118">For more information, see [Specify Posting Periods](../../finance-how-specify-posting-periods.md) and [Understanding the General Ledger and the COA](../../finance-general-ledger.md).</span></span>  

- <span data-ttu-id="018db-119">L'exercice comptable a été clôturé à l'aide de la fonction **Clôturer exercice** sur la page **Périodes comptables**.</span><span class="sxs-lookup"><span data-stu-id="018db-119">The fiscal year has been closed using the **Close Year** function on the **Accounting Periods** page.</span></span> <span data-ttu-id="018db-120">Pour plus d'informations, voir [Clôture des exercices et des périodes](../../year-close-years-periods.md).</span><span class="sxs-lookup"><span data-stu-id="018db-120">For more information, see [Closing Years and Periods](../../year-close-years-periods.md).</span></span>  

- <span data-ttu-id="018db-121">Toutes les lignes feuille non validées pour l'exercice ont été validées ou supprimées.</span><span class="sxs-lookup"><span data-stu-id="018db-121">All the unposted journal lines for the year have been posted or deleted.</span></span>  

- <span data-ttu-id="018db-122">Toutes les écritures de clôture sont à jour.</span><span class="sxs-lookup"><span data-stu-id="018db-122">All closing entries are up to date.</span></span>  

<span data-ttu-id="018db-123">Lorsque vous clôturez une période fiscale, la plus ancienne période fiscale ouverte est clôturée.</span><span class="sxs-lookup"><span data-stu-id="018db-123">When you close a fiscal period, the earliest open fiscal period is closed.</span></span> <span data-ttu-id="018db-124">Le champ **Début période validation** sur la page **Paramètres comptabilité** est mis à jour avec la date de début de la période ouverte suivante, si la date existante dans ce champ n'est pas déjà une date postérieure.</span><span class="sxs-lookup"><span data-stu-id="018db-124">The **Allow Posting From** field on the **General Ledger Setup** page is updated with the start date for the next open period, if the existing date in this field is not already a later date.</span></span> <span data-ttu-id="018db-125">Si le champ **Fin période validation** sur la page **Paramètres comptabilité** se situe dans la période clôturée, la valeur du champ **Fin période validation** est mise à jour avec la date de fin de la première période fiscale ouverte.</span><span class="sxs-lookup"><span data-stu-id="018db-125">If the **Allow Posting To** field on the **General Ledger Setup** page is within the closed period, then the value in the **Allow Posting To** field is updated with the end date for the first open fiscal period.</span></span> <span data-ttu-id="018db-126">Pour plus d'informations, voir [Description des écritures comptables et du plan comptable](../../finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="018db-126">For more information, see [Understanding the General Ledger and the COA](../../finance-general-ledger.md).</span></span>  

<span data-ttu-id="018db-127">À la fin de l'exercice, vous devez effectuer les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="018db-127">At the end of the year, you must do the following:</span></span>  

- <span data-ttu-id="018db-128">clôturer l'exercice comptable à l'aide de la fonction **Clôturer exercice** ;</span><span class="sxs-lookup"><span data-stu-id="018db-128">Close the fiscal year using the **Close Year** function.</span></span>  
- <span data-ttu-id="018db-129">générer une écriture de clôture d'exercice ;</span><span class="sxs-lookup"><span data-stu-id="018db-129">Generate a year-end closing entry.</span></span>  
- <span data-ttu-id="018db-130">valider l'écriture de clôture d'exercice et compenser les écritures comptables de fonds propres ;</span><span class="sxs-lookup"><span data-stu-id="018db-130">Post the year-end closing entry, along with the offset equity account entries.</span></span>  
- <span data-ttu-id="018db-131">clôturer l'exercice comptable à l'aide de la fonction **Clôturer l'exercice fiscalement**.</span><span class="sxs-lookup"><span data-stu-id="018db-131">Close the fiscal year using the **Fiscally Close Year** function.</span></span>  

## <a name="see-also"></a><span data-ttu-id="018db-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="018db-132">See Also</span></span>

[<span data-ttu-id="018db-133">Valider l'écriture de clôture d'exercice</span><span class="sxs-lookup"><span data-stu-id="018db-133">Post the Year-End Closing Entry</span></span>](how-to-post-the-year-end-closing-entry.md)  
[<span data-ttu-id="018db-134">Clôturer fiscalement des périodes comptables</span><span class="sxs-lookup"><span data-stu-id="018db-134">Fiscally Close Accounting Periods</span></span>](how-to-fiscally-close-accounting-periods.md)  
[<span data-ttu-id="018db-135">Clôture des exercices et des périodes</span><span class="sxs-lookup"><span data-stu-id="018db-135">Closing Years and Periods</span></span>](../../year-close-years-periods.md)  
[<span data-ttu-id="018db-136">Valider l'écriture de clôture d'exercice</span><span class="sxs-lookup"><span data-stu-id="018db-136">Post the Year-End Closing Entry</span></span>](how-to-post-the-year-end-closing-entry.md)  
[<span data-ttu-id="018db-137">Clôturer fiscalement des exercices</span><span class="sxs-lookup"><span data-stu-id="018db-137">Fiscally Close Years</span></span>](how-to-fiscally-close-years.md)  
[<span data-ttu-id="018db-138">Rouvrir des périodes comptables</span><span class="sxs-lookup"><span data-stu-id="018db-138">Reopen Accounting Periods</span></span>](how-to-reopen-accounting-periods.md)  
[<span data-ttu-id="018db-139">Clôturer les comptes de gestion</span><span class="sxs-lookup"><span data-stu-id="018db-139">Close Income Statement Accounts</span></span>](how-to-close-income-statement-accounts.md)  
[<span data-ttu-id="018db-140">Définir des périodes de validation</span><span class="sxs-lookup"><span data-stu-id="018db-140">Specify Posting Periods</span></span>](../../finance-how-specify-posting-periods.md)  
[<span data-ttu-id="018db-141">Description des écritures comptables et du plan comptable</span><span class="sxs-lookup"><span data-stu-id="018db-141">Understanding the General Ledger and the COA</span></span>](../../finance-general-ledger.md)  
[<span data-ttu-id="018db-142">Fonctionnalité locale, France</span><span class="sxs-lookup"><span data-stu-id="018db-142">France Local Functionality</span></span>](france-local-functionality.md)  
