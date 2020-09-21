---
title: Procédure de définition des périodes de validation
description: En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/23/2020
ms.author: edupont
ms.openlocfilehash: 22f6a6c49f4790637dbf39fc3a5a2ef5ccc604e3
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778634"
---
# <a name="specify-posting-periods-in-the-french-version"></a><span data-ttu-id="d166a-103">Définir les périodes de validation dans la version française</span><span class="sxs-lookup"><span data-stu-id="d166a-103">Specify Posting Periods In the French Version</span></span>

<span data-ttu-id="d166a-104">En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée.</span><span class="sxs-lookup"><span data-stu-id="d166a-104">When you specify posting periods, you limit the period in which posting is allowed.</span></span>  

## <a name="to-specify-posting-periods"></a><span data-ttu-id="d166a-105">Pour définir des périodes de validation</span><span class="sxs-lookup"><span data-stu-id="d166a-105">To specify posting periods</span></span>  

1. <span data-ttu-id="d166a-106">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Paramètres comptabilité**, puis sélectionnez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="d166a-106">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d166a-107">Sur la page **Paramètres comptabilité**, dans le champ **Début période validation**, spécifiez la date de début de la période de validation.</span><span class="sxs-lookup"><span data-stu-id="d166a-107">On the **General Ledger Setup** page, in the **Allow Posting From** field, specify the start date of the posting period.</span></span>  
3. <span data-ttu-id="d166a-108">Dans le champ **Fin période validation**, spécifiez la date de fin de la période de validation.</span><span class="sxs-lookup"><span data-stu-id="d166a-108">In the **Allow Posting To** field, specify the end date of the posting period.</span></span>  

    <span data-ttu-id="d166a-109">Les dates sont validées dans les plages de validation autorisées pour garantir leur appartenance aux exercices comptables ouverts.</span><span class="sxs-lookup"><span data-stu-id="d166a-109">The dates are validated against the allowed posting ranges to make sure that they belong to open fiscal years.</span></span> <span data-ttu-id="d166a-110">Pour plus d'informations, voir Plage de validation autorisée.</span><span class="sxs-lookup"><span data-stu-id="d166a-110">For more information, see Allowed Posting Range.</span></span>  

4. <span data-ttu-id="d166a-111">Pour vérifier quelle est la plage de validation autorisée, choisissez l'action **Extraire plage de validation autorisée**.</span><span class="sxs-lookup"><span data-stu-id="d166a-111">To verify what the allowed posting range is, choose the **Get Allowed Posting Range** action.</span></span>  

<span data-ttu-id="d166a-112">Les dates définies ici s'appliquent à l'ensemble de la société, c'est-à-dire à tous les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="d166a-112">The dates that you define here apply to the whole company, that is, to all users.</span></span>  

> [!NOTE]  
> <span data-ttu-id="d166a-113">Vous pouvez définir différentes périodes de comptabilisation pour divers utilisateurs et appliquer une période de validation à un utilisateur sur la page **Paramètres utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="d166a-113">You can define different posting periods for different users and apply a posting period to a user on the **User Setup** page.</span></span>

<span data-ttu-id="d166a-114">Si vous entrez des dates ici, les dates entrées sur la page **Paramètres comptabilité** ne s'appliquent pas à ces utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="d166a-114">If you enter dates here, the dates entered on the **General Ledger Setup** page will not apply to these users.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d166a-115">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d166a-115">See Also</span></span>

[<span data-ttu-id="d166a-116">Périodes fiscales et exercices comptables</span><span class="sxs-lookup"><span data-stu-id="d166a-116">Fiscal Periods and Fiscal Years</span></span>](fiscal-periods-and-fiscal-years.md)
