---
title: Procédure de création des bordereaux paiement
description: Vous pouvez créer des bordereaux paiement pour gérer les paiements fournisseur et client. Avant de créer des bordereaux paiement, vous devez paramétrer des types de règlement.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 3ff7838f76ac496c3b2a324fcbfbe6f8af28070d
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/10/2020
ms.locfileid: "3676903"
---
# <a name="create-payment-slips"></a><span data-ttu-id="4058e-104">Créer bordereaux paiement</span><span class="sxs-lookup"><span data-stu-id="4058e-104">Create Payment Slips</span></span>
<span data-ttu-id="4058e-105">Vous pouvez créer des bordereaux paiement pour gérer les paiements fournisseur et client.</span><span class="sxs-lookup"><span data-stu-id="4058e-105">You can create payments slips to manage vendor and customer payments.</span></span> <span data-ttu-id="4058e-106">Avant de créer des bordereaux paiement, vous devez paramétrer des types de règlement.</span><span class="sxs-lookup"><span data-stu-id="4058e-106">Before you create payment slips, you must set up payment classes.</span></span> <span data-ttu-id="4058e-107">Pour plus d'informations, voir [Paramétrer des types de règlement](how-to-set-up-payment-classes.md).</span><span class="sxs-lookup"><span data-stu-id="4058e-107">For more information, see [Set Up Payment Classes](how-to-set-up-payment-classes.md).</span></span>  

<span data-ttu-id="4058e-108">La procédure suivante décrit comment créer des bordereaux paiement pour les règlements fournisseur, mais les mêmes étapes s'appliquent également à la création des bordereaux paiement pour les règlements client.</span><span class="sxs-lookup"><span data-stu-id="4058e-108">The following procedure describes how to create payment slips for vendor payments, but the same steps also apply to creating payment slips for customer payments.</span></span>  

## <a name="to-create-a-payment-slip-for-vendors"></a><span data-ttu-id="4058e-109">Pour créer un bordereau de paiement pour les fournisseurs</span><span class="sxs-lookup"><span data-stu-id="4058e-109">To create a payment slip for vendors</span></span>  

1.  <span data-ttu-id="4058e-110">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Bordereaux de paiement**, puis choisissez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="4058e-110">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Slips**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="4058e-111">Sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="4058e-111">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="4058e-112">Sur la page **Bordereau paiement**, sélectionnez un champ pour ouvrir la page **Liste des types de règlement**.</span><span class="sxs-lookup"><span data-stu-id="4058e-112">On the **Payment Slip** page, choose a field to open the **Payment Class List** page.</span></span>  
4.  <span data-ttu-id="4058e-113">Sélectionnez un type de règlement, puis choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="4058e-113">Select a payment class, and then choose the **OK** button.</span></span>  
5.  <span data-ttu-id="4058e-114">Sous le raccourci **Général**, renseignez les champs comme indiqué dans le tableau ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="4058e-114">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="4058e-115">Champ</span><span class="sxs-lookup"><span data-stu-id="4058e-115">Field</span></span>|<span data-ttu-id="4058e-116">Désignation</span><span class="sxs-lookup"><span data-stu-id="4058e-116">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="4058e-117">**Code devise**</span><span class="sxs-lookup"><span data-stu-id="4058e-117">**Currency Code**</span></span>|<span data-ttu-id="4058e-118">Spécifiez le code devise à utiliser pour les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="4058e-118">Specify the currency code to be used for the payment lines.</span></span>|  
    |<span data-ttu-id="4058e-119">**Date de validation**</span><span class="sxs-lookup"><span data-stu-id="4058e-119">**Posting Date**</span></span>|<span data-ttu-id="4058e-120">Spécifiez une date comptabilisation.</span><span class="sxs-lookup"><span data-stu-id="4058e-120">Specify the posting date.</span></span>|  
    |<span data-ttu-id="4058e-121">**Date document**</span><span class="sxs-lookup"><span data-stu-id="4058e-121">**Document Date**</span></span>|<span data-ttu-id="4058e-122">Spécifiez la date du document.</span><span class="sxs-lookup"><span data-stu-id="4058e-122">Specify the document date.</span></span>|  
    |<span data-ttu-id="4058e-123">**Montant DS**</span><span class="sxs-lookup"><span data-stu-id="4058e-123">**Amount (LCY)**</span></span>|<span data-ttu-id="4058e-124">Montant total des lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="4058e-124">The total amount from the payment lines.</span></span> <span data-ttu-id="4058e-125">Ce champ est mis à jour automatiquement à chaque modification des montants nets des lignes.</span><span class="sxs-lookup"><span data-stu-id="4058e-125">This field is updated automatically when the net line amounts are changed.</span></span><br /><br />|  

6.  <span data-ttu-id="4058e-126">Sous le raccourci **Lignes**, renseignez les champs comme indiqué dans le tableau ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="4058e-126">On the **Lines** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="4058e-127">Champ</span><span class="sxs-lookup"><span data-stu-id="4058e-127">Field</span></span>|<span data-ttu-id="4058e-128">Désignation</span><span class="sxs-lookup"><span data-stu-id="4058e-128">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="4058e-129">**Type compte**</span><span class="sxs-lookup"><span data-stu-id="4058e-129">**Account Type**</span></span>|<span data-ttu-id="4058e-130">Type de compte sur lequel la ligne bordereau est validée.</span><span class="sxs-lookup"><span data-stu-id="4058e-130">The account type to which the payment line is posted.</span></span>|  
    |<span data-ttu-id="4058e-131">**N° compte**</span><span class="sxs-lookup"><span data-stu-id="4058e-131">**Account No.**</span></span>|<span data-ttu-id="4058e-132">Numéro d'identification unique pour le compte sur lequel l'écriture est validée.</span><span class="sxs-lookup"><span data-stu-id="4058e-132">The unique identification number for the account to which the entry will be posted.</span></span>|  

7.  <span data-ttu-id="4058e-133">Dans le champ **Code compte bancaire**, sélectionnez un nom bancaire dans la liste, puis choisissez **Avancé**.</span><span class="sxs-lookup"><span data-stu-id="4058e-133">In the **Bank Account Code** field, select a bank name from the list, and then choose **Advanced**.</span></span>  
8.  <span data-ttu-id="4058e-134">Éventuellement, pour SEPA, sur la page **Sélectionner – Liste des comptes fournisseur**, puis cliquez sur l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="4058e-134">Optionally, for SEPA, on the **Select – Vendor Account List** page, and then choose the **Edit** action.</span></span>  

    <span data-ttu-id="4058e-135">Renseignez les champs suivants, si nécessaire :</span><span class="sxs-lookup"><span data-stu-id="4058e-135">Fill in the following fields if needed:</span></span>  

    - <span data-ttu-id="4058e-136">**Code pays/région**.</span><span class="sxs-lookup"><span data-stu-id="4058e-136">**Country/Region Code**.</span></span> <span data-ttu-id="4058e-137">Dans la liste, choisissez **Avancé**, puis assurez-vous que la case à cocher **SEPA autorisé** est sélectionnée pour le code que vous sélectionnez.</span><span class="sxs-lookup"><span data-stu-id="4058e-137">In the list, choose **Advanced**, and make sure that the **SEPA Allowed** check box is selected for the code that you select.</span></span>  
    - <span data-ttu-id="4058e-138">**Code SWIFT**</span><span class="sxs-lookup"><span data-stu-id="4058e-138">**Swift Code**</span></span>  
    - <span data-ttu-id="4058e-139">**IBAN**</span><span class="sxs-lookup"><span data-stu-id="4058e-139">**IBAN**</span></span>  

    <span data-ttu-id="4058e-140">Cliquez sur le bouton **OK** pour fermer la page.</span><span class="sxs-lookup"><span data-stu-id="4058e-140">Choose the **OK** button to close the page.</span></span>  

9. <span data-ttu-id="4058e-141">Éventuellement, pour SEPA, choisissez l'action **Relevé d'identité bancaire**.</span><span class="sxs-lookup"><span data-stu-id="4058e-141">Optionally, for SEPA, choose the **Header RIB** action.</span></span> <span data-ttu-id="4058e-142">Sélectionnez le champ **Code pays/région banque**, puis choisissez **Avancé**.</span><span class="sxs-lookup"><span data-stu-id="4058e-142">Select the **Bank Country/Region Code** field, and then choose **Advanced**.</span></span> <span data-ttu-id="4058e-143">Assurez-vous que la case à cocher **SEPA autorisé** est sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="4058e-143">Make sure the **SEPA Allowed** check box is selected.</span></span> <span data-ttu-id="4058e-144">Assurez-vous également que les champs **IBAN** et **Code SWIFT** sont renseignés.</span><span class="sxs-lookup"><span data-stu-id="4058e-144">Also make sure that the **IBAN** and **SWIFT Code** fields are filled in.</span></span>  

10. <span data-ttu-id="4058e-145">Choisissez l'action **Proposer paiements fournisseur**.</span><span class="sxs-lookup"><span data-stu-id="4058e-145">Choose the **Suggest Vendor Payments** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="4058e-146">Vous pouvez également renseigner manuellement les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="4058e-146">You can also manually fill in the payment lines.</span></span>  

11. <span data-ttu-id="4058e-147">Dans le traitement par lots **Proposer paiements fournisseur**, sur le raccourci **Options**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="4058e-147">In the **Suggest Vendor Payments** batch job, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="4058e-148">Champ</span><span class="sxs-lookup"><span data-stu-id="4058e-148">Field</span></span>|<span data-ttu-id="4058e-149">Désignation</span><span class="sxs-lookup"><span data-stu-id="4058e-149">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="4058e-150">**Dernière date échéance**</span><span class="sxs-lookup"><span data-stu-id="4058e-150">**Last Payment Date**</span></span>|<span data-ttu-id="4058e-151">Dernière date de paiement pour les écritures comptables fournisseur à inclure dans le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="4058e-151">The last payment date for the vendor ledger entries that are to be included in the batch job.</span></span>|  
    |<span data-ttu-id="4058e-152">**Rechercher les escomptes**</span><span class="sxs-lookup"><span data-stu-id="4058e-152">**Find Payment Discounts**</span></span>|<span data-ttu-id="4058e-153">Sélectionnez d'inclure les écritures comptables fournisseur pour lesquelles vous pouvez obtenir un escompte.</span><span class="sxs-lookup"><span data-stu-id="4058e-153">Select to include vendor ledger entries for which you can receive a payment discount.</span></span>|  
    |<span data-ttu-id="4058e-154">**Totaliser par**</span><span class="sxs-lookup"><span data-stu-id="4058e-154">**Summarize per**</span></span>|<span data-ttu-id="4058e-155">Critères de totalisation de la ligne paiement.</span><span class="sxs-lookup"><span data-stu-id="4058e-155">The criteria for summarizing the payment line.</span></span>|  
    |<span data-ttu-id="4058e-156">**Utiliser priorité fournisseur**</span><span class="sxs-lookup"><span data-stu-id="4058e-156">**Use Vendor Priority**</span></span>|<span data-ttu-id="4058e-157">Sélectionnez de trier les paiements proposés en fonction de la valeur du champ **Priorité** sur les fiches fournisseur.</span><span class="sxs-lookup"><span data-stu-id="4058e-157">Select to sort the suggested payments based on the value in the **Priority** field on the vendor cards.</span></span> <span data-ttu-id="4058e-158">Pour plus d'informations, voir Priorité.</span><span class="sxs-lookup"><span data-stu-id="4058e-158">For more information, see Priority.</span></span>|  
    |<span data-ttu-id="4058e-159">**Montant disponible DS**</span><span class="sxs-lookup"><span data-stu-id="4058e-159">**Available Amount (LCY)**</span></span>|<span data-ttu-id="4058e-160">Montant maximal qui est disponible pour les paiements en devise société.</span><span class="sxs-lookup"><span data-stu-id="4058e-160">The maximum amount that is available for payments in local currency.</span></span>|  
    |<span data-ttu-id="4058e-161">**Filtre devise**</span><span class="sxs-lookup"><span data-stu-id="4058e-161">**Currency Filter**</span></span>|<span data-ttu-id="4058e-162">Code de la devise à inclure dans le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="4058e-162">The code for the currency to be included in the batch job.</span></span>|  

12. <span data-ttu-id="4058e-163">Sur le raccourci **Fournisseur**, sélectionnez les filtres appropriés.</span><span class="sxs-lookup"><span data-stu-id="4058e-163">On the **Vendor** FastTab, select the appropriate filters.</span></span>  
13. <span data-ttu-id="4058e-164">Choisissez le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="4058e-164">Choose the **OK** button.</span></span>  

    <span data-ttu-id="4058e-165">Les lignes paiement sont automatiquement créées.</span><span class="sxs-lookup"><span data-stu-id="4058e-165">The payment lines are automatically created.</span></span>  

14. <span data-ttu-id="4058e-166">Sur la page **Bordereau paiement**, sous le raccourci **Validation**, renseignez les champs comme indiqué dans le tableau ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="4058e-166">On the **Payment Slip** page, on the **Posting** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="4058e-167">Champ</span><span class="sxs-lookup"><span data-stu-id="4058e-167">Field</span></span>|<span data-ttu-id="4058e-168">Désignation</span><span class="sxs-lookup"><span data-stu-id="4058e-168">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="4058e-169">**Code journal**</span><span class="sxs-lookup"><span data-stu-id="4058e-169">**Source Code**</span></span>|<span data-ttu-id="4058e-170">Code source du bordereau paiement.</span><span class="sxs-lookup"><span data-stu-id="4058e-170">The source code for the payment slip.</span></span>|  
    |<span data-ttu-id="4058e-171">**Code emplacement immo**</span><span class="sxs-lookup"><span data-stu-id="4058e-171">**Department Code**</span></span>|<span data-ttu-id="4058e-172">Code axe analytique approprié.</span><span class="sxs-lookup"><span data-stu-id="4058e-172">The relevant dimension code.</span></span>|  
    |<span data-ttu-id="4058e-173">**Code projet**</span><span class="sxs-lookup"><span data-stu-id="4058e-173">**Project Code**</span></span>|<span data-ttu-id="4058e-174">Code axe analytique approprié.</span><span class="sxs-lookup"><span data-stu-id="4058e-174">The relevant dimension code.</span></span>|  
    |<span data-ttu-id="4058e-175">**Type compte**</span><span class="sxs-lookup"><span data-stu-id="4058e-175">**Account Type**</span></span>|<span data-ttu-id="4058e-176">Type de compte vers et à partir duquel les paiements seront transférés.</span><span class="sxs-lookup"><span data-stu-id="4058e-176">The account type to which or from which the payments will be transferred.</span></span>|  
    |<span data-ttu-id="4058e-177">**N° compte**</span><span class="sxs-lookup"><span data-stu-id="4058e-177">**Account No.**</span></span>|<span data-ttu-id="4058e-178">Numéro de compte vers et à partir duquel les paiements seront transférés.</span><span class="sxs-lookup"><span data-stu-id="4058e-178">The account number to which or from which the payments will be transferred.</span></span>|  

15. <span data-ttu-id="4058e-179">Éventuellement, pour SEPA, dans le champ **N° compte**, choisissez l'option **Avancé**.</span><span class="sxs-lookup"><span data-stu-id="4058e-179">Optionally, for SEPA, in the **Account No.** field, choose the **Advanced** option.</span></span>  

    1. <span data-ttu-id="4058e-180">Sur la page **Liste des comptes bancaires**, sélectionnez l'action **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="4058e-180">On the **Bank Account List** page, choose the **Edit** action.</span></span>  
    2. <span data-ttu-id="4058e-181">Renseignez les champs suivants, si nécessaire :</span><span class="sxs-lookup"><span data-stu-id="4058e-181">Fill in the following fields if needed:</span></span>  

        - <span data-ttu-id="4058e-182">Raccourci **Général**</span><span class="sxs-lookup"><span data-stu-id="4058e-182">**General** FastTab</span></span>  
        - <span data-ttu-id="4058e-183">**Code pays/région**</span><span class="sxs-lookup"><span data-stu-id="4058e-183">**Country/Region Code**</span></span>  
        - <span data-ttu-id="4058e-184">Raccourci **Transfert**</span><span class="sxs-lookup"><span data-stu-id="4058e-184">**Transfer**  FastTab</span></span>  
        - <span data-ttu-id="4058e-185">**Code SWIFT**</span><span class="sxs-lookup"><span data-stu-id="4058e-185">**Swift Code**</span></span>  
        - <span data-ttu-id="4058e-186">**IBAN**</span><span class="sxs-lookup"><span data-stu-id="4058e-186">**IBAN**</span></span>  
        - <span data-ttu-id="4058e-187">Raccourci **RIB**</span><span class="sxs-lookup"><span data-stu-id="4058e-187">**RIB** FastTab</span></span>  
        - <span data-ttu-id="4058e-188">**Format exportation paiement** : SEPA</span><span class="sxs-lookup"><span data-stu-id="4058e-188">**Payment Export Format**: SEPA</span></span>  
        - <span data-ttu-id="4058e-189">**Souches de n° ID Msg Virement SEPA** : Banque</span><span class="sxs-lookup"><span data-stu-id="4058e-189">**SEPA CT Msg. ID No. Series**: Bank</span></span>  

16. <span data-ttu-id="4058e-190">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="4058e-190">Choose the **OK** button.</span></span>  

<span data-ttu-id="4058e-191">Après avoir créé un bordereau de paiement, vous pouvez générer des fichiers de paiement et les envoyer à la banque par voie électronique.</span><span class="sxs-lookup"><span data-stu-id="4058e-191">After you create a payment slip, you can generate payment files and send them to the bank electronically.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="4058e-192">Un fichier de paiement peut être créé si le bordereau de paiement affiche **Fichier** dans le champ **Type action**.</span><span class="sxs-lookup"><span data-stu-id="4058e-192">A payment file can be created if the payment slip displays **File** for the **Action Type** field.</span></span>

## <a name="to-create-a-payment-file"></a><span data-ttu-id="4058e-193">Pour créer un fichier de paiement</span><span class="sxs-lookup"><span data-stu-id="4058e-193">To create a payment file</span></span>  

1.  <span data-ttu-id="4058e-194">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Bordereaux de paiement**, puis choisissez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="4058e-194">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Slips**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="4058e-195">Sélectionnez un bordereau paiement, puis cliquez sur **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="4058e-195">Select a payment slip, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="4058e-196">Sur la page **Bordereau paiement**, sélectionnez **Générer fichier**.</span><span class="sxs-lookup"><span data-stu-id="4058e-196">On the **Payment Slip** page, choose the **Generate file** action.</span></span>  
4.  <span data-ttu-id="4058e-197">Cliquez sur le bouton **Oui**, puis sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="4058e-197">Choose the **Yes** button, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="4058e-198">Le fichier de paiement est généré et exporté en fonction du type d'exportation spécifié sur la page **Étape règlement**.</span><span class="sxs-lookup"><span data-stu-id="4058e-198">The payment file is generated and exported according to the export type that is specified on the **Payment Step** page.</span></span>  

5.  <span data-ttu-id="4058e-199">En cas d'erreur, consultez les erreurs répertoriées dans le récapitulatif **Erreurs exportation fichier** et prenez la mesure appropriée.</span><span class="sxs-lookup"><span data-stu-id="4058e-199">In the case of error, review the errors listed in the **File Export Errors** FactBox, and take the appropriate action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4058e-200">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4058e-200">See Also</span></span>  
 <span data-ttu-id="4058e-201">[Gestion des paiements](payment-management.md) </span><span class="sxs-lookup"><span data-stu-id="4058e-201">[Payment Management](payment-management.md) </span></span>  
 <span data-ttu-id="4058e-202">[Paramétrer des types de règlement](how-to-set-up-payment-classes.md) </span><span class="sxs-lookup"><span data-stu-id="4058e-202">[Set Up Payment Classes](how-to-set-up-payment-classes.md) </span></span>  
 <span data-ttu-id="4058e-203">[Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md) </span><span class="sxs-lookup"><span data-stu-id="4058e-203">[Set Up Payment Statuses](how-to-set-up-payment-statuses.md) </span></span>  
 <span data-ttu-id="4058e-204">[Paramétrer des étapes règlement](how-to-set-up-payment-steps.md) </span><span class="sxs-lookup"><span data-stu-id="4058e-204">[Set Up Payment Steps](how-to-set-up-payment-steps.md) </span></span>  
 <span data-ttu-id="4058e-205">[Configurer des adresses de paiement](how-to-set-up-payment-addresses.md) </span><span class="sxs-lookup"><span data-stu-id="4058e-205">[Set Up Payment Addresses](how-to-set-up-payment-addresses.md) </span></span>  
 <span data-ttu-id="4058e-206">[Valider des bordereaux paiement](how-to-post-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="4058e-206">[Post Payment Slips](how-to-post-payment-slips.md) </span></span>  
 <span data-ttu-id="4058e-207">[Archiver les bordereaux de paiement](how-to-archive-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="4058e-207">[Archive Payment Slips](how-to-archive-payment-slips.md) </span></span>  
 [<span data-ttu-id="4058e-208">Exporter ou importer les paramètres de configuration de la gestion des paiements</span><span class="sxs-lookup"><span data-stu-id="4058e-208">Export or Import Payment Management Setup Parameters</span></span>](how-to-export-or-import-payment-management-setup-parameters.md)
