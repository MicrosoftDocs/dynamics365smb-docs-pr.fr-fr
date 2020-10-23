---
title: Vue d'ensemble des processus de fin d'exercice
description: Une clôture d'exercice dans Business Central implique trois étapes.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 7eceeeaaf391e36725f77a5d23bd5cb4620c5eb3
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/01/2020
ms.locfileid: "3920100"
---
# <a name="year-end-processes-overview"></a><span data-ttu-id="440f0-103">Vue d'ensemble des processus de fin d'exercice</span><span class="sxs-lookup"><span data-stu-id="440f0-103">Year End Processes Overview</span></span>

<span data-ttu-id="440f0-104">Une clôture d'exercice dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)] implique trois étapes :</span><span class="sxs-lookup"><span data-stu-id="440f0-104">Year end closing in [!INCLUDE[d365fin](../../includes/d365fin_md.md)] involves three steps:</span></span>  

1. <span data-ttu-id="440f0-105">Clôture de l'exercice comptable.</span><span class="sxs-lookup"><span data-stu-id="440f0-105">Closing the fiscal year.</span></span> <span data-ttu-id="440f0-106">Pour plus d'informations, voir [Clôturer fiscalement des périodes comptables](how-to-fiscally-close-accounting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="440f0-106">For more information, see [Fiscally Close Accounting Periods](how-to-fiscally-close-accounting-periods.md).</span></span>  
2. <span data-ttu-id="440f0-107">Générer une écriture de clôture d'exercice via l'option **Clôturer exercice comptable** avec la compensation des écritures de compte de fonds propres.</span><span class="sxs-lookup"><span data-stu-id="440f0-107">Generating a year-end closing entry using the **Close Income Statement** option along with the offsetting equity account entries.</span></span> <span data-ttu-id="440f0-108">Pour plus d'informations, reportez-vous à [Validation de l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md).</span><span class="sxs-lookup"><span data-stu-id="440f0-108">For more information, see [Posting the year-end closing entry](how-to-post-the-year-end-closing-entry.md).</span></span>  
3. <span data-ttu-id="440f0-109">Clôture de l'exercice comptable.</span><span class="sxs-lookup"><span data-stu-id="440f0-109">Fiscally closing the fiscal year.</span></span> <span data-ttu-id="440f0-110">Pour plus d'informations, voir [Clôturer fiscalement des exercices](how-to-fiscally-close-years.md).</span><span class="sxs-lookup"><span data-stu-id="440f0-110">For more information, see [Fiscally Close Years](how-to-fiscally-close-years.md).</span></span>  

<span data-ttu-id="440f0-111">Selon la norme française *NF Logiciel compatibilité informatisée*, le système doit refuser la création d'un troisième exercice comptable ouvert. Seuls deux exercices comptables peuvent donc être ouverts en même temps.</span><span class="sxs-lookup"><span data-stu-id="440f0-111">According to the French law *NF Logiciel compatibilité informatisée* the system has to refuse the creation of a third open fiscal year, so only two open fiscal years are allowed at the same time.</span></span>  

<span data-ttu-id="440f0-112">Vous devez dès lors clôturer l'exercice en temps voulu.</span><span class="sxs-lookup"><span data-stu-id="440f0-112">So in time you are required to close a year.</span></span> <span data-ttu-id="440f0-113">Les détails des transactions ne risquent pas d'être perdus lorsque vous clôturez l'exercice, puisqu'ils sont tous mémorisés, même après avoir clôturé fiscalement l'exercice.</span><span class="sxs-lookup"><span data-stu-id="440f0-113">You also do not have to worry about losing details of transactions when you close because all details are retained, even after you (fiscally) close the year.</span></span>  

<span data-ttu-id="440f0-114">Lors de la clôture en fin d'exercice, le système déplace vos bénéfices des bénéfices calculés, ou du compte Bénéfices actuels, vers un compte validé, ou le compte Bénéfices non répartis.</span><span class="sxs-lookup"><span data-stu-id="440f0-114">When you close at the end of the year, the system moves your earnings from calculated earnings, or the Current Earnings account, to a posted account, or the Retained Earnings account.</span></span> <span data-ttu-id="440f0-115">Le système indique également que l'exercice comptable est « clôturé » et renseigne toutes les entrées suivantes pour l'exercice clôturé comme « écritures de l'exercice précédent ».</span><span class="sxs-lookup"><span data-stu-id="440f0-115">The system also marks the fiscal year as "closed," and marks all subsequent entries for the closed year as "prior year entries."</span></span>  

<span data-ttu-id="440f0-116">Le système génère ensuite une écriture de clôture mais ne la valide pas automatiquement.</span><span class="sxs-lookup"><span data-stu-id="440f0-116">The system then generates a closing entry, but it does not post the entry automatically.</span></span> <span data-ttu-id="440f0-117">Vous avez la possibilité de créer les écritures comptables de fonds propres de décalage qui vous permettent de choisir la manière dont vous voulez affecter votre écriture de clôture.</span><span class="sxs-lookup"><span data-stu-id="440f0-117">You are given the opportunity to make the offsetting equity account entry or entries, which allows you to decide how to allocate your closing entry.</span></span> <span data-ttu-id="440f0-118">Par exemple, si votre société comprend plusieurs départements, vous pouvez laisser le système générer une écriture de clôture unique pour tous les départements et créer une écriture de décalage pour le compte de fonds propres de chaque département.</span><span class="sxs-lookup"><span data-stu-id="440f0-118">For example, if your company has several divisions, you can let the system generate a single closing entry for all the divisions, and you can then make an offsetting entry for each division's equity account.</span></span>  

<span data-ttu-id="440f0-119">Après avoir clôturé fiscalement un exercice, vous ne pourrez plus rien comptabiliser dans cet exercice.</span><span class="sxs-lookup"><span data-stu-id="440f0-119">Once a year has been fiscally closed you will not be able to post in this fiscal year.</span></span>  

## <a name="see-also"></a><span data-ttu-id="440f0-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="440f0-120">See Also</span></span>

[<span data-ttu-id="440f0-121">Clôturer fiscalement des périodes comptables</span><span class="sxs-lookup"><span data-stu-id="440f0-121">Fiscally Close Accounting Periods</span></span>](how-to-fiscally-close-accounting-periods.md)  
[<span data-ttu-id="440f0-122">Validation de l'écriture de clôture d'exercice</span><span class="sxs-lookup"><span data-stu-id="440f0-122">Posting the year-end closing entry</span></span>](how-to-post-the-year-end-closing-entry.md)  
[<span data-ttu-id="440f0-123">Clôturer fiscalement des exercices</span><span class="sxs-lookup"><span data-stu-id="440f0-123">Fiscally Close Years</span></span>](how-to-fiscally-close-years.md)  
[<span data-ttu-id="440f0-124">Périodes fiscales et exercices comptables</span><span class="sxs-lookup"><span data-stu-id="440f0-124">Fiscal Periods and Fiscal Years</span></span>](fiscal-periods-and-fiscal-years.md)  
[<span data-ttu-id="440f0-125">Clôture des exercices et des périodes</span><span class="sxs-lookup"><span data-stu-id="440f0-125">Closing Years and Periods</span></span>](../../year-close-years-periods.md)  
