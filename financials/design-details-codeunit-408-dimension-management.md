---
title: "Détails de conception - Codeunit 408 Gestion des axes analytiques | Microsoft Docs"
description: "Codeunit 408 Gestion des axes analytiques est une bibliothèque de fonctions qui gère les tâches courantes qui sont liées aux axes analytiques, tels que copier d'une table à une autre ou d'un document à un autre."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 32f67c058570f03d4aa1c84d9bb32289b1f07bec
ms.contentlocale: fr-fr
ms.lasthandoff: 12/14/2017

---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="7a27c-103">Détails de conception : Codeunit 408 Gestion des axes analytiques</span><span class="sxs-lookup"><span data-stu-id="7a27c-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="7a27c-104">Codeunit 408 Gestion des axes analytiques est une bibliothèque de fonctions qui gère les tâches courantes qui sont liées aux axes analytiques, tels que copier d'une table à une autre ou d'un document à un autre.</span><span class="sxs-lookup"><span data-stu-id="7a27c-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="7a27c-105">Cette rubrique répertorie les fonctions modifiées dans Microsoft Dynamics NAV 2013 R2 et spécifie ce qui doit être effectué sur les fonctions.</span><span class="sxs-lookup"><span data-stu-id="7a27c-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="7a27c-106">La plupart des fonctions sont supprimées parce qu'il n'y a pas besoin de copier entre les tables axe analytique.</span><span class="sxs-lookup"><span data-stu-id="7a27c-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="7a27c-107">Fonctions modifiées</span><span class="sxs-lookup"><span data-stu-id="7a27c-107">Modified Functions</span></span>  

|<span data-ttu-id="7a27c-108">Nom de fonction</span><span class="sxs-lookup"><span data-stu-id="7a27c-108">Function Name</span></span>|<span data-ttu-id="7a27c-109">Description de modification</span><span class="sxs-lookup"><span data-stu-id="7a27c-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="7a27c-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="7a27c-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="7a27c-111">Nouvelle fonction qui remplace les autres fonctions de contrôle et prend un ID d'ensemble de dimensions dans un argument au lieu d'une table axe analytique.</span><span class="sxs-lookup"><span data-stu-id="7a27c-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="7a27c-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="7a27c-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="7a27c-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="7a27c-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="7a27c-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="7a27c-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="7a27c-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="7a27c-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="7a27c-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="7a27c-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="7a27c-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="7a27c-117">CheckDimValueComb</span></span>|<span data-ttu-id="7a27c-118">Supprimer.</span><span class="sxs-lookup"><span data-stu-id="7a27c-118">Delete.</span></span> <span data-ttu-id="7a27c-119">L'ensemble de l'activité doit être changé en CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="7a27c-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="7a27c-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-120">GetDefaultDim</span></span>|<span data-ttu-id="7a27c-121">Modifiez pour renvoyer un ID d'ensemble de dimensions entier au lieu d'un ensemble d'enregistrements.</span><span class="sxs-lookup"><span data-stu-id="7a27c-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="7a27c-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="7a27c-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="7a27c-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="7a27c-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="7a27c-126">Modifier pour utiliser DimSetID -> ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="7a27c-127">Fonctions supprimées</span><span class="sxs-lookup"><span data-stu-id="7a27c-127">Deleted Functions</span></span>  
 <span data-ttu-id="7a27c-128">Les fonctions supprimées du codeunit 408 en relation avec la fonction Écritures de l'ensemble de dimensions sont répertoriées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="7a27c-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="7a27c-129">Lors de la mise à niveau du code d'application depuis Microsoft Dynamics NAV 2009 ou des versions antérieures vers Microsoft Dynamics NAV 2016, les fonctions suivantes ne sont pas disponibles dans Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="7a27c-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="7a27c-130">Si des personnalisations utilisent une ou plusieurs fonctions, vous devez mettre à niveau ce code en conséquence.</span><span class="sxs-lookup"><span data-stu-id="7a27c-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="7a27c-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="7a27c-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="7a27c-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="7a27c-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="7a27c-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-136">InsertDocDim</span></span>  

 <span data-ttu-id="7a27c-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="7a27c-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="7a27c-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="7a27c-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="7a27c-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-141">InsertServContractDim</span></span>  

 <span data-ttu-id="7a27c-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="7a27c-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="7a27c-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="7a27c-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-144">GetDocDim</span></span>  

 <span data-ttu-id="7a27c-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-145">GetProdDocDim</span></span>  

 <span data-ttu-id="7a27c-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="7a27c-146">TypeToTableID1</span></span>  

 <span data-ttu-id="7a27c-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="7a27c-147">TypeToTableID2</span></span>  

 <span data-ttu-id="7a27c-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="7a27c-148">TypeToTableID3</span></span>  

 <span data-ttu-id="7a27c-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="7a27c-149">TypeToTableID4</span></span>  

 <span data-ttu-id="7a27c-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="7a27c-150">TypeToTableID5</span></span>  

 <span data-ttu-id="7a27c-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-152">DeleteDocDim</span></span>  

 <span data-ttu-id="7a27c-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="7a27c-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="7a27c-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="7a27c-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="7a27c-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="7a27c-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-160">ShowDocDim</span></span>  

 <span data-ttu-id="7a27c-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-161">SaveDocDim</span></span>  

 <span data-ttu-id="7a27c-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="7a27c-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="7a27c-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-164">ShowTempDim</span></span>  

 <span data-ttu-id="7a27c-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-165">SaveTempDim</span></span>  

 <span data-ttu-id="7a27c-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="7a27c-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="7a27c-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-168">SaveServContractDim</span></span>  

 <span data-ttu-id="7a27c-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="7a27c-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="7a27c-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="7a27c-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="7a27c-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="7a27c-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="7a27c-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="7a27c-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="7a27c-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="7a27c-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="7a27c-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="7a27c-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="7a27c-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="7a27c-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="7a27c-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="7a27c-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="7a27c-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="7a27c-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="7a27c-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="7a27c-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="7a27c-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="7a27c-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="7a27c-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="7a27c-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="7a27c-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="7a27c-198">TestDimValue</span></span>  

 <span data-ttu-id="7a27c-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="7a27c-199">TestNewDimValue</span></span>  

 <span data-ttu-id="7a27c-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="7a27c-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="7a27c-201">(Supprimé, car la table ItemBudgetDim est supprimée.)</span><span class="sxs-lookup"><span data-stu-id="7a27c-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="7a27c-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-202">GetServContractDim</span></span>  

 <span data-ttu-id="7a27c-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="7a27c-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="7a27c-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="7a27c-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="7a27c-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="7a27c-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="7a27c-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="7a27c-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="7a27c-207">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7a27c-207">See Also</span></span>
 <span data-ttu-id="7a27c-208">[Détails de conception : écritures d'ensemble de dimensions](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="7a27c-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="7a27c-209">[Détails de conception : aperçu des écritures de l'ensemble de dimensions](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="7a27c-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="7a27c-210">[Détails de conception : recherche des croisements analytiques](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="7a27c-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 <span data-ttu-id="7a27c-211">[Détails de conception : structure de la table](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="7a27c-211">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 [<span data-ttu-id="7a27c-212">Détails de conception : exemples de code de motifs modifiés dans les modifications</span><span class="sxs-lookup"><span data-stu-id="7a27c-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)

