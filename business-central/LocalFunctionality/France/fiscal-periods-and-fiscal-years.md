---
title: "Périodes fiscales et exercices comptables"
description: "Un exercice comptable est généralement divisé en 12 périodes fiscales mensuelles. Dans Business Central, deux exercices comptables peuvent être ouverts en même temps."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 30/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 0818b918648ed01590f215a2f25e8288b0092a02
ms.contentlocale: fr-fr
ms.lasthandoff: 03/22/2018

---
# <a name="fiscal-periods-and-fiscal-years"></a><span data-ttu-id="1d48e-104">Périodes fiscales et exercices comptables</span><span class="sxs-lookup"><span data-stu-id="1d48e-104">Fiscal Periods and Fiscal Years</span></span>
<span data-ttu-id="1d48e-105">Un exercice comptable est généralement divisé en 12 périodes fiscales mensuelles.</span><span class="sxs-lookup"><span data-stu-id="1d48e-105">A fiscal year is typically divided into 12 monthly fiscal periods.</span></span> <span data-ttu-id="1d48e-106">Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], deux exercices comptables peuvent être ouverts en même temps.</span><span class="sxs-lookup"><span data-stu-id="1d48e-106">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can have two fiscal years open at the same time.</span></span> <span data-ttu-id="1d48e-107">Vous ne pouvez pas créer un troisième exercice comptable si deux exercices comptables sont ouverts.</span><span class="sxs-lookup"><span data-stu-id="1d48e-107">You cannot create a third fiscal year if there are two fiscal years open.</span></span>  

<span data-ttu-id="1d48e-108">Pour clôturer un exercice comptable, vous devez clôturer les périodes comptables de cet exercice.</span><span class="sxs-lookup"><span data-stu-id="1d48e-108">To close a fiscal year, you must close the accounting periods within that year.</span></span>  

<span data-ttu-id="1d48e-109">Vous ne pouvez rouvrir une période comptable clôturée que si elle fait partie d'un exercice comptable ouvert.</span><span class="sxs-lookup"><span data-stu-id="1d48e-109">You can only reopen a closed accounting period if the period falls within an open fiscal year.</span></span> <span data-ttu-id="1d48e-110">Pour plus d'informations, voir [Clôture des exercices](how-to-close-years.md).</span><span class="sxs-lookup"><span data-stu-id="1d48e-110">For more information, see [Close Years](how-to-close-years.md).</span></span> <span data-ttu-id="1d48e-111">Vous ne pouvez pas rouvrir un exercice comptable clôturé.</span><span class="sxs-lookup"><span data-stu-id="1d48e-111">You cannot reopen a closed fiscal year.</span></span>  

## <a name="closing-fiscal-periods-and-fiscal-years"></a><span data-ttu-id="1d48e-112">Clôture de périodes fiscales et d'exercices comptables</span><span class="sxs-lookup"><span data-stu-id="1d48e-112">Closing Fiscal Periods and Fiscal Years</span></span>  
<span data-ttu-id="1d48e-113">À la fin d'un exercice comptable, vous devez clôturer les périodes comptables de cet exercice comptable.</span><span class="sxs-lookup"><span data-stu-id="1d48e-113">After a fiscal year is complete, you must close the accounting periods within that fiscal year.</span></span> <span data-ttu-id="1d48e-114">Cela garantit que des écritures comptables ne sont pas validées pour cette période.</span><span class="sxs-lookup"><span data-stu-id="1d48e-114">This is to ensure that general ledger entries are not posted for that period.</span></span> <span data-ttu-id="1d48e-115">Pour plus d'informations, voir [Clôturer fiscalement des périodes comptables](how-to-fiscally-close-years.md).</span><span class="sxs-lookup"><span data-stu-id="1d48e-115">For more information, see [Fiscally Close Accounting Periods](how-to-fiscally-close-years.md).</span></span>  

<span data-ttu-id="1d48e-116">Un exercice comptable peut être clôturé si tous les critères suivants sont remplis :</span><span class="sxs-lookup"><span data-stu-id="1d48e-116">A fiscal year can be closed if all of the following criteria are met:</span></span>  

- <span data-ttu-id="1d48e-117">Les dates comptabilisation dans la fenêtre **Paramètres utilisateur** et la fenêtre **Paramètres comptabilité** ne font pas partie de l'exercice que vous clôturez.</span><span class="sxs-lookup"><span data-stu-id="1d48e-117">The posting dates in the **User Setup** window and the **General Ledger Setup** window do not fall within the year that you are closing.</span></span> <span data-ttu-id="1d48e-118">Pour plus d'informations, voir Paramètres utilisateur et Paramètres comptabilité.</span><span class="sxs-lookup"><span data-stu-id="1d48e-118">For more information, see User Setup and General Ledger Setup.</span></span>  

- <span data-ttu-id="1d48e-119">L'exercice comptable a été clôturé à l'aide de la fonction **Clôturer exercice** dans la fenêtre **Périodes comptables**.</span><span class="sxs-lookup"><span data-stu-id="1d48e-119">The fiscal year has been closed using the **Close Year** function in the **Accounting Periods** window.</span></span> <span data-ttu-id="1d48e-120">Pour plus d'informations, voir [Clôture des exercices et des périodes](../../year-close-years-periods.md).</span><span class="sxs-lookup"><span data-stu-id="1d48e-120">For more information, see [Closing Years and Periods](../../year-close-years-periods.md).</span></span>  

- <span data-ttu-id="1d48e-121">Toutes les lignes feuille non validées et les écritures de simulation de l'exercice ont été validées ou supprimées.</span><span class="sxs-lookup"><span data-stu-id="1d48e-121">All of the unposted journal lines and simulation entries for the year have been posted or deleted.</span></span>  

- <span data-ttu-id="1d48e-122">Toutes les écritures de clôture sont à jour.</span><span class="sxs-lookup"><span data-stu-id="1d48e-122">All closing entries are up to date.</span></span>  

<span data-ttu-id="1d48e-123">Lorsque vous clôturez une période fiscale, la plus ancienne période fiscale ouverte est clôturée.</span><span class="sxs-lookup"><span data-stu-id="1d48e-123">When you close a fiscal period, the earliest open fiscal period is closed.</span></span> <span data-ttu-id="1d48e-124">Le champ **Début période validation** dans la fenêtre **Paramètres comptabilité** est mis à jour avec la date de début de la période ouverte suivante, si la date existante dans ce champ n'est pas déjà une date postérieure.</span><span class="sxs-lookup"><span data-stu-id="1d48e-124">The **Allow Posting From** field in the **General Ledger Setup** window is updated with the start date for the next open period, if the existing date in this field is not already a later date.</span></span> <span data-ttu-id="1d48e-125">Si le champ **Fin période validation** dans la fenêtre **Paramètres comptabilité** se situe dans la période clôturée, la valeur du champ **Fin période validation** est mise à jour avec la date de fin de la première période fiscale ouverte.</span><span class="sxs-lookup"><span data-stu-id="1d48e-125">If the **Allow Posting To** field in the **General Ledger Setup** window is within the closed period, then the value in the **Allow Posting To** field is updated with the end date for the first open fiscal period.</span></span> <span data-ttu-id="1d48e-126">Pour plus d'informations, voir Paramètres comptabilité.</span><span class="sxs-lookup"><span data-stu-id="1d48e-126">For more information, see General Ledger Setup.</span></span>  

<span data-ttu-id="1d48e-127">À la fin de l'exercice, vous devez effectuer les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="1d48e-127">At the end of the year, you must do the following:</span></span>  

- <span data-ttu-id="1d48e-128">clôturer l'exercice comptable à l'aide de la fonction **Clôturer exercice** ;</span><span class="sxs-lookup"><span data-stu-id="1d48e-128">Close the fiscal year using the **Close Year** function.</span></span>  
- <span data-ttu-id="1d48e-129">générer une écriture de clôture d'exercice ;</span><span class="sxs-lookup"><span data-stu-id="1d48e-129">Generate a year-end closing entry.</span></span>  
- <span data-ttu-id="1d48e-130">valider l'écriture de clôture d'exercice et compenser les écritures comptables de fonds propres ;</span><span class="sxs-lookup"><span data-stu-id="1d48e-130">Post the year-end closing entry, along with the offset equity account entries.</span></span>  
- <span data-ttu-id="1d48e-131">clôturer l'exercice comptable à l'aide de la fonction **Clôturer l'exercice fiscalement**.</span><span class="sxs-lookup"><span data-stu-id="1d48e-131">Close the fiscal year using the **Fiscally Close Year** function.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1d48e-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1d48e-132">See Also</span></span>  
 <span data-ttu-id="1d48e-133">[Valider l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md) </span><span class="sxs-lookup"><span data-stu-id="1d48e-133">[Post the Year-End Closing Entry](how-to-post-the-year-end-closing-entry.md) </span></span>  
 <span data-ttu-id="1d48e-134">[Clôturer fiscalement des périodes comptables](how-to-fiscally-close-accounting-periods.md) </span><span class="sxs-lookup"><span data-stu-id="1d48e-134">[Fiscally Close Accounting Periods](how-to-fiscally-close-accounting-periods.md) </span></span>  
 <span data-ttu-id="1d48e-135">[Clôture des exercices et des périodes](../../year-close-years-periods.md) </span><span class="sxs-lookup"><span data-stu-id="1d48e-135">[Closing Years and Periods](../../year-close-years-periods.md) </span></span>  
 <span data-ttu-id="1d48e-136">[Valider l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md) </span><span class="sxs-lookup"><span data-stu-id="1d48e-136">[Post the Year-End Closing Entry](how-to-post-the-year-end-closing-entry.md) </span></span>  
 <span data-ttu-id="1d48e-137">[Clôturer fiscalement des exercices](how-to-fiscally-close-years.md) </span><span class="sxs-lookup"><span data-stu-id="1d48e-137">[Fiscally Close Years](how-to-fiscally-close-years.md) </span></span>  
 <span data-ttu-id="1d48e-138">[Rouvrir des périodes comptables](how-to-reopen-accounting-periods.md) </span><span class="sxs-lookup"><span data-stu-id="1d48e-138">[Reopen Accounting Periods](how-to-reopen-accounting-periods.md) </span></span>  
 <span data-ttu-id="1d48e-139">[Clôturer les comptes de gestion](how-to-close-income-statement-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="1d48e-139">[Close Income Statement Accounts](how-to-close-income-statement-accounts.md) </span></span>  
 [<span data-ttu-id="1d48e-140">Fonctionnalité locale, France</span><span class="sxs-lookup"><span data-stu-id="1d48e-140">France Local Functionality</span></span>](france-local-functionality.md)

