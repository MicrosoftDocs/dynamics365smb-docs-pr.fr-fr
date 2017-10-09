---
title: "Recouvrement prélèvement SEPA | Microsoft Docs"
description: "Créez un recouvrement prélèvement et exportez un fichier XML que vous envoyez ou chargez vers votre banque électronique en vue de son traitement."
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct-debit, collection, payment, sepa
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: dbecf91050dbdf299ca11e8e5650b2a63b4ccc16
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-create-sepa-direct-debit-collection-entries-and-export-to-a-bank-file"></a><span data-ttu-id="1250a-103">Procédure : créer des écritures de collection prélèvement automatique SEPA et les exporter vers un fichier bancaire</span><span class="sxs-lookup"><span data-stu-id="1250a-103">How to: Create SEPA Direct Debit Collection Entries and Export to a Bank File</span></span>
<span data-ttu-id="1250a-104">Pour demander à la banque de transférer le montant du paiement du compte bancaire du client vers le compte de votre société, vous créez une écriture de collection de prélèvement, qui conserve des informations sur le compte bancaire du client, les factures de vente concernées et le mandat de prélèvement.</span><span class="sxs-lookup"><span data-stu-id="1250a-104">To instruct the bank to transfer the payment amount from the customer’s bank account to your company’s account, you create a direct-debit collection, which holds information about the customer’s bank account, the affected sales invoices, and the direct-debit mandate.</span></span> <span data-ttu-id="1250a-105">À partir de l'écriture de collection prélèvement automatique qui en résulte, vous exportez ensuite un fichier XML que vous envoyez ou transférez à votre banque électronique pour traitement.</span><span class="sxs-lookup"><span data-stu-id="1250a-105">From the resulting direct-debit collection entry, you then export an XML file that you send or upload to your electronic bank for processing.</span></span> <span data-ttu-id="1250a-106">La banque vous communiquera tous les paiements qu'elle n'a pas pu traiter, et vous devez rejeter manuellement les écritures de collection prélèvement automatique en question.</span><span class="sxs-lookup"><span data-stu-id="1250a-106">Any payments that could not be processed by the bank will be communicated to you by your bank, and you must then manually reject the direct debit-collection entries in question.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="1250a-107">Pour réunir les paiements à l'aide du prélèvement SEPA, la devise sur la facture vente doit être l'EURO.</span><span class="sxs-lookup"><span data-stu-id="1250a-107">To collect payments using SEPA Direct Debit, the currency on the sales invoice must be EURO.</span></span>  

### <a name="to-create-a-direct-debit-collection"></a><span data-ttu-id="1250a-108">Pour créer une collection prélèvement automatique</span><span class="sxs-lookup"><span data-stu-id="1250a-108">To create a direct-debit collection</span></span>  
1. <span data-ttu-id="1250a-109">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Recouvrements prélèvement**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="1250a-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Direct Debit Collections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1250a-110">Dans la fenêtre **Recouvrements prélèvement**, sous l'onglet **Accueil**, dans le groupe **Nouveau**, choisissez **Créer collection prélèvement automatique**.</span><span class="sxs-lookup"><span data-stu-id="1250a-110">In the **Direct Debit Collections** window, on the **Home** tab, in the **New** group, choose **Create Direct Debit Collection**.</span></span>  
3. <span data-ttu-id="1250a-111">Dans la fenêtre **Créer recouvrement prélèvement**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="1250a-111">In the **Create Direct Debit Collection** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="1250a-112">Champ</span><span class="sxs-lookup"><span data-stu-id="1250a-112">Field</span></span>|<span data-ttu-id="1250a-113">Désignation</span><span class="sxs-lookup"><span data-stu-id="1250a-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="1250a-114">**Date d'échéance début**</span><span class="sxs-lookup"><span data-stu-id="1250a-114">**From Due Date**</span></span>|<span data-ttu-id="1250a-115">Spécifie la date d'échéance de paiement la plus proche sur les factures vente pour lesquelles vous souhaitez créer une collection prélèvement automatique.</span><span class="sxs-lookup"><span data-stu-id="1250a-115">Specify the earliest payment due date on sales invoices that you want to create a direct-debit collection for.</span></span>|  
    |<span data-ttu-id="1250a-116">**Date d'échéance fin**</span><span class="sxs-lookup"><span data-stu-id="1250a-116">**To Due Date**</span></span>|<span data-ttu-id="1250a-117">Spécifie la date d'échéance de paiement la plus ancienne sur les factures vente pour lesquelles vous souhaitez créer une collection prélèvement automatique.</span><span class="sxs-lookup"><span data-stu-id="1250a-117">Specify the latest payment due date on sales invoices that you want to create a direct-debit collection for.</span></span>|  
    |<span data-ttu-id="1250a-118">**Type partenaire**</span><span class="sxs-lookup"><span data-stu-id="1250a-118">**Partner Type**</span></span>|<span data-ttu-id="1250a-119">Spécifie si la collection prélèvement automatique est réalisée pour des clients de type **Société** ou **Personne**.</span><span class="sxs-lookup"><span data-stu-id="1250a-119">Specify if the direct-debit collection is made for customers of type **Company** or **Person**.</span></span>|  
    |<span data-ttu-id="1250a-120">**Uniquement les clients avec mandat valide**</span><span class="sxs-lookup"><span data-stu-id="1250a-120">**Only Customers With Valid Mandate**</span></span>|<span data-ttu-id="1250a-121">Spécifie si une collection de prélèvement est créée pour les clients disposant d'un mandat de prélèvement valable.</span><span class="sxs-lookup"><span data-stu-id="1250a-121">Specify if a direct-debit collection is created for customers who have a valid direct-debit mandate.</span></span> <span data-ttu-id="1250a-122">**Remarque :** une collection prélèvement automatique est créée même si le champ **ID mandat de prélèvement** n'est pas rempli sur la facture vente.</span><span class="sxs-lookup"><span data-stu-id="1250a-122">**Note:**  A direct-debit collection is created even if the **Direct Debit Mandate ID** field is not filled on the sales invoice.</span></span>|  
    |<span data-ttu-id="1250a-123">**Uniquement les factures avec mandat valide**</span><span class="sxs-lookup"><span data-stu-id="1250a-123">**Only Invoices With Valid Mandate**</span></span>|<span data-ttu-id="1250a-124">Spécifiez si une collection prélèvement est créée uniquement pour les factures vente si un mandat de prélèvement valide est sélectionné dans le champ **ID mandat de prélèvement** de la facture vente.</span><span class="sxs-lookup"><span data-stu-id="1250a-124">Specify if a direct-debit collection is only created for sales invoices if a valid direct-debit mandate is selected in the **Direct Debit Mandate ID** field on the sales invoice.</span></span>|  
    |<span data-ttu-id="1250a-125">**N° compte bancaire**</span><span class="sxs-lookup"><span data-stu-id="1250a-125">**Bank Account No.**</span></span>|<span data-ttu-id="1250a-126">Spécifie les comptes bancaires de votre société sur lesquels le paiement collecté sera transféré à partir du compte bancaire du client.</span><span class="sxs-lookup"><span data-stu-id="1250a-126">Specify which of your company’s bank accounts the collected payment will be transferred to from the customer’s bank account.</span></span>|  
    |<span data-ttu-id="1250a-127">**Nom compte bancaire**</span><span class="sxs-lookup"><span data-stu-id="1250a-127">**Bank Account Name**</span></span>|<span data-ttu-id="1250a-128">Spécifie le nom du compte bancaire que vous sélectionnez dans le champ **N° compte bancaire**.</span><span class="sxs-lookup"><span data-stu-id="1250a-128">Specifies the name of the bank account that you select in the **Bank Account No.** field.</span></span> <span data-ttu-id="1250a-129">Ce champ est complété automatiquement.</span><span class="sxs-lookup"><span data-stu-id="1250a-129">This field is filled automatically.</span></span>|  

4. <span data-ttu-id="1250a-130">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="1250a-130">Choose the **OK** button.</span></span>  

     <span data-ttu-id="1250a-131">Une collection prélèvement automatique est ajoutée à la fenêtre **Recouvrements prélèvement** et une ou plusieurs écritures de collection prélèvement automatique sont créées.</span><span class="sxs-lookup"><span data-stu-id="1250a-131">A direct-debit collection is added to the **Direct Debit Collections** window, and one or more direct-debit collection entries are created.</span></span>  

### <a name="to-export-a-direct-debit-collection-entry-to-a-bank-file"></a><span data-ttu-id="1250a-132">Pour exporter une collection prélèvement automatique vers un fichier bancaire</span><span class="sxs-lookup"><span data-stu-id="1250a-132">To export a direct-debit collection entry to a bank file</span></span>  
1. <span data-ttu-id="1250a-133">Dans la fenêtre **Recouvrements prélèvement**, sous l'onglet **Accueil**, dans le groupe **Traitement**, choisissez **Écritures recouvrement prélèvement**.</span><span class="sxs-lookup"><span data-stu-id="1250a-133">In the **Direct Debit Collections** window, on the **Home** tab, in the **Process** group, choose **Direct Debit Collect. Entries**.</span></span>  
2. <span data-ttu-id="1250a-134">Dans la fenêtre **Écritures recouvrement prélèvement**, sélectionnez l'écriture que vous voulez exporter, puis sous l'onglet **Accueil**, dans le groupe **Traitement**, cliquez sur **Créer fichier prélèvement automatique**.</span><span class="sxs-lookup"><span data-stu-id="1250a-134">In the **Direct Debit Collect. Entries** window, select the entry that you want to export, and then, on the **Home** tab, in the **Process** group, choose **Create Direct Debit** File.</span></span>  
3. <span data-ttu-id="1250a-135">Enregistrez le fichier d'exportation à l'emplacement où vous l'envoyez ou transférez\-le à votre banque électronique.</span><span class="sxs-lookup"><span data-stu-id="1250a-135">Save the export file to the location from where you send or upload it to your electronic bank.</span></span>  

     <span data-ttu-id="1250a-136">Dans la fenêtre **Écritures recouvrement prélèvement**, le champ **Statut recouvrement prélèvement** est modifié sur Fichier créé.</span><span class="sxs-lookup"><span data-stu-id="1250a-136">In the **Direct Debit Collect. Entries** window, the **Direct Debit Collection Status** field is changed to File Created.</span></span> <span data-ttu-id="1250a-137">Dans la fenêtre **Mandats de prélèvement SEPA**, le champ **Compteur prélèvements** est mis à jour avec un nombre.</span><span class="sxs-lookup"><span data-stu-id="1250a-137">In the **SEPA Direct Debit Mandates** window, the **Debit Counter** field is updated with one count.</span></span>  

<span data-ttu-id="1250a-138">Si le fichier exporté ne peut pas être traité, par exemple parce que le client est insolvable, vous pouvez rejeter l'écriture de collection prélèvement automatique.</span><span class="sxs-lookup"><span data-stu-id="1250a-138">If the exported file cannot be processed, for example because the customer is insolvent, you can reject the direct-debit collection entry.</span></span> <span data-ttu-id="1250a-139">Si le fichier exporté est correctement traité par la banque, les paiements dus des factures vente impliquées sont collectés automatiquement auprès des clients concernés.</span><span class="sxs-lookup"><span data-stu-id="1250a-139">If the exported file is successfully processed by the bank, the due payments of the involved sales invoices are automatically collected from the involved customers.</span></span> <span data-ttu-id="1250a-140">Dans ce cas, vous pouvez fermer la collection.</span><span class="sxs-lookup"><span data-stu-id="1250a-140">In that case you can close the collection.</span></span>  

### <a name="to-reject-a-direct-debit-collection-entry"></a><span data-ttu-id="1250a-141">Pour rejeter une écriture collection prélèvement automatique</span><span class="sxs-lookup"><span data-stu-id="1250a-141">To reject a direct-debit collection entry</span></span>  
* <span data-ttu-id="1250a-142">Dans la fenêtre **Écritures recouvrement prélèvement**, sélectionnez l'écriture qui n'a pas été traitée, puis sous l'onglet **Accueil**, dans le groupe **Traitement**, cliquez sur **Rejeter écriture**.</span><span class="sxs-lookup"><span data-stu-id="1250a-142">In the **Direct Debit Collect. Entries** window, select the entry that was not successfully processed, and then, on the **Home** tab, in the **Process** group, choose **Reject Entry**.</span></span>  

     <span data-ttu-id="1250a-143">La valeur du champ **Statut** de la fenêtre **Écritures recouvrement prélèvement** est modifiée sur **Rejetée**.</span><span class="sxs-lookup"><span data-stu-id="1250a-143">The value in the **Status** field in the **Direct Debit Collect. Entries** window is changed to **Rejected**.</span></span>  

### <a name="to-close-a-direct-debit-collection"></a><span data-ttu-id="1250a-144">Pour fermer une collection prélèvement automatique</span><span class="sxs-lookup"><span data-stu-id="1250a-144">To close a direct-debit collection</span></span>  
* <span data-ttu-id="1250a-145">Dans la fenêtre **Écritures recouvrement prélèvement**, sélectionnez l'écriture qui a été traitée, puis sous l'onglet **Accueil**, dans le groupe **Traitement**, cliquez sur **Fermer collection**.</span><span class="sxs-lookup"><span data-stu-id="1250a-145">In the **Direct Debit Collect. Entries** window, select the entry that was successfully processed, and then, on the **Home** tab, in the **Process** group, choose **Close Collection**.</span></span>  

     <span data-ttu-id="1250a-146">La collection prélèvement automatique associée est fermée.</span><span class="sxs-lookup"><span data-stu-id="1250a-146">The related direct-debit collection is closed.</span></span>  

<span data-ttu-id="1250a-147">Vous pouvez maintenant valider les réceptions de paiement pour les factures vente impliquées.</span><span class="sxs-lookup"><span data-stu-id="1250a-147">You can now post receipts of payment for the involved sales invoices.</span></span> <span data-ttu-id="1250a-148">Vous pouvez généralement le faire pendant que vous validez des réceptions de paiement, tel que dans la fenêtre **Enregistrement de paiement**, ou vous pouvez valider les réceptions de paiement directement à partir de la fenêtre **Écritures recouvrement prélèvement**.</span><span class="sxs-lookup"><span data-stu-id="1250a-148">You can do this as you typically post payment receipts, such as in the **Payment Registration** window, or you can post the related payment receipts directly from the **Direct Debit Collect. Entries** window.</span></span> <span data-ttu-id="1250a-149">Pour plus d'informations, voir [Procédure : valider des réceptions règlement de prélèvement SEPA](finance-how-to-post-sepa-direct-debit-payment-receipts.md).</span><span class="sxs-lookup"><span data-stu-id="1250a-149">For more information, see [How to: Post SEPA Direct Debit Payment Receipts](finance-how-to-post-sepa-direct-debit-payment-receipts.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="1250a-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1250a-150">See Also</span></span>  
<span data-ttu-id="1250a-151">[Procédure : configurer un prélèvement SEPA](finance-how-to-set-up-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="1250a-151">[How to: Set Up SEPA Direct Debit](finance-how-to-set-up-sepa-direct-debit.md) </span></span>  
<span data-ttu-id="1250a-152">[Procédure : valider des réceptions règlement de prélèvement SEPA](finance-how-to-post-sepa-direct-debit-payment-receipts.md) </span><span class="sxs-lookup"><span data-stu-id="1250a-152">[How to: Post SEPA Direct Debit Payment Receipts](finance-how-to-post-sepa-direct-debit-payment-receipts.md) </span></span>  
[<span data-ttu-id="1250a-153">Recouvrement de paiements par prélèvement automatique SEPA</span><span class="sxs-lookup"><span data-stu-id="1250a-153">Collect Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)   
