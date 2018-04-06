---
title: "Procédure de paramétrage d'une simulation"
description: "Vous pouvez créer et valider des écritures de simulation dans la comptabilité sans affecter la comptabilité réelle."
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
ms.openlocfilehash: 4c6ca1ef945118f4659bbe30db4d08367c5369bc
ms.contentlocale: fr-fr
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-simulation"></a><span data-ttu-id="d4790-103">Paramétrer une simulation</span><span class="sxs-lookup"><span data-stu-id="d4790-103">Set Up Simulation</span></span>
<span data-ttu-id="d4790-104">Vous pouvez créer et valider des écritures de simulation dans la comptabilité sans affecter la comptabilité réelle.</span><span class="sxs-lookup"><span data-stu-id="d4790-104">You can create and post simulation entries to the general ledger without affecting the real accounting.</span></span>  

<span data-ttu-id="d4790-105">Avant de pouvoir commencer à utiliser la fonctionnalité de simulation, vous devez configurer un code source et une souche de numéros et ajouter ces informations à un modèle feuille comptabilité.</span><span class="sxs-lookup"><span data-stu-id="d4790-105">Before you can start to use the simulation functionality, you must set up a source code and a number series, and you must add this information to a general journal template.</span></span>  

## <a name="to-set-up-simulation"></a><span data-ttu-id="d4790-106">Pour paramétrer une simulation</span><span class="sxs-lookup"><span data-stu-id="d4790-106">To set up simulation</span></span>  

1.  <span data-ttu-id="d4790-107">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Codes sources**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="d4790-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Source Codes**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d4790-108">Dans la fenêtre **Codes sources**, créez un enregistrement et renseignez les champs.</span><span class="sxs-lookup"><span data-stu-id="d4790-108">In the **Source Codes** window, create a new record and fill in the fields.</span></span>  

    > [!IMPORTANT]  
    >  <span data-ttu-id="d4790-109">Sélectionnez le champ **Simulation**.</span><span class="sxs-lookup"><span data-stu-id="d4790-109">Select the **Simulation** field.</span></span>  

3.  <span data-ttu-id="d4790-110">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Souches de n°**, puis sélectionnez le lien associé à la zone **Configuration**.</span><span class="sxs-lookup"><span data-stu-id="d4790-110">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **No. Series**, and then choose the related link for the **Setup** area.</span></span>  
4.  <span data-ttu-id="d4790-111">Dans la fenêtre **Souches de n°**, créez un enregistrement et renseignez les champs.</span><span class="sxs-lookup"><span data-stu-id="d4790-111">In the **No. Series** window, create a new record and fill in the fields.</span></span> <span data-ttu-id="d4790-112">Naviguez jusqu'au champ **N° début**</span><span class="sxs-lookup"><span data-stu-id="d4790-112">Drill down on the **Starting No.**</span></span> <span data-ttu-id="d4790-113">pour paramétrer des informations supplémentaires pour la souche de numéros.</span><span class="sxs-lookup"><span data-stu-id="d4790-113">field to set up additional information for the number series.</span></span>  
5.  <span data-ttu-id="d4790-114">Sélectionnez les champs **N° par défaut** et **N° manuels**.</span><span class="sxs-lookup"><span data-stu-id="d4790-114">Select the **Default Nos.** field and the **Manual Nos.** field.</span></span>  
6.  <span data-ttu-id="d4790-115">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Modèles feuille comptabilité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="d4790-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal Templates**, and then choose the related link.</span></span>  
7.  <span data-ttu-id="d4790-116">Dans la fenêtre **Modèles feuille comptabilité**, créez un enregistrement et renseignez les champs.</span><span class="sxs-lookup"><span data-stu-id="d4790-116">In the **General Journal Templates** window, create a new record and fill in the fields.</span></span> <span data-ttu-id="d4790-117">Dans le champ **Type**, sélectionnez Général et spécifiez la nouvelle souche de numéros et le nouveau code source dans le champ **Souches de n°** et **Code source**.</span><span class="sxs-lookup"><span data-stu-id="d4790-117">In the **Type** field, select General, and specify your new number series and source code in the **No. Series** field and the **Source Code** field.</span></span>  

<span data-ttu-id="d4790-118">Vous pouvez désormais créer des écritures de simulation à l'aide de la feuille comptabilité.</span><span class="sxs-lookup"><span data-stu-id="d4790-118">Now you can create simulation entries using the general journal.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d4790-119">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4790-119">See Also</span></span>  
 <span data-ttu-id="d4790-120">[Créer des écritures de simulation](how-to-create-simulation-entries.md) </span><span class="sxs-lookup"><span data-stu-id="d4790-120">[Create Simulation Entries](how-to-create-simulation-entries.md) </span></span>  
 <span data-ttu-id="d4790-121">[Supprimer des écritures de simulation](how-to-delete-simulation-entries.md) </span><span class="sxs-lookup"><span data-stu-id="d4790-121">[Delete Simulation Entries](how-to-delete-simulation-entries.md) </span></span>  
 [<span data-ttu-id="d4790-122">Transférer des écritures de simulation</span><span class="sxs-lookup"><span data-stu-id="d4790-122">Transfer Simulation Entries</span></span>](how-to-transfer-simulation-entries.md)

