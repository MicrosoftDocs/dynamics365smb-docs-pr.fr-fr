---
title: Procédure de paramétrage des types de règlement
description: Pour utiliser le module Gestion des paiements, vous devez paramétrer des types de règlement pour définir des types d'opération, tels que des lettres de change, des paiements électroniques ou des chèques.
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
ms.openlocfilehash: 0808575e789208178fd4d7dc2cd9db2e83f6beae
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/01/2020
ms.locfileid: "3181188"
---
# <a name="set-up-payment-classes"></a><span data-ttu-id="b02a4-103">Paramétrer des types de règlement</span><span class="sxs-lookup"><span data-stu-id="b02a4-103">Set Up Payment Classes</span></span>
<span data-ttu-id="b02a4-104">Pour utiliser le module Gestion des paiements, vous devez paramétrer des types de règlement pour définir des types d'opération, tels que des lettres de change, des paiements électroniques ou des chèques.</span><span class="sxs-lookup"><span data-stu-id="b02a4-104">To use payment management, you must set up payment classes to define operation types, such as bills of exchange, electronic payments, or checks.</span></span>  

## <a name="to-set-up-a-payment-class"></a><span data-ttu-id="b02a4-105">Pour paramétrer un type de règlement</span><span class="sxs-lookup"><span data-stu-id="b02a4-105">To set up a payment class</span></span>  

1.  <span data-ttu-id="b02a4-106">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Icône Page ou état pour la recherche"), entrez **Paramètres bordereau paiement**, puis sélectionnez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="b02a4-106">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Slip Setup**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="b02a4-107">Sur la page **Type de règlement**, sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="b02a4-107">On the **Payment Class** page, choose the **New** action.</span></span>  
3.  <span data-ttu-id="b02a4-108">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="b02a4-108">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="b02a4-109">Champ</span><span class="sxs-lookup"><span data-stu-id="b02a4-109">Field</span></span>|<span data-ttu-id="b02a4-110">Désignation</span><span class="sxs-lookup"><span data-stu-id="b02a4-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="b02a4-111">**Activer**</span><span class="sxs-lookup"><span data-stu-id="b02a4-111">**Enable**</span></span>|<span data-ttu-id="b02a4-112">Permet d'activer l'utilisation du type de règlement.</span><span class="sxs-lookup"><span data-stu-id="b02a4-112">Select to enable usage of the payment class.</span></span>|  
    |<span data-ttu-id="b02a4-113">**Code**</span><span class="sxs-lookup"><span data-stu-id="b02a4-113">**Code**</span></span>|<span data-ttu-id="b02a4-114">Code d'identification unique du type de règlement.</span><span class="sxs-lookup"><span data-stu-id="b02a4-114">The unique identification code for the payment class.</span></span>|  
    |<span data-ttu-id="b02a4-115">**Nom**</span><span class="sxs-lookup"><span data-stu-id="b02a4-115">**Name**</span></span>|<span data-ttu-id="b02a4-116">Description du type de règlement.</span><span class="sxs-lookup"><span data-stu-id="b02a4-116">The payment class description.</span></span>|  
    |<span data-ttu-id="b02a4-117">**N° de souche en-tête**</span><span class="sxs-lookup"><span data-stu-id="b02a4-117">**Header No. Series**</span></span>|<span data-ttu-id="b02a4-118">Code souche de numéros pour l'en-tête du bordereau paiement.</span><span class="sxs-lookup"><span data-stu-id="b02a4-118">The number series code for the payment slip header.</span></span>|  
    |<span data-ttu-id="b02a4-119">**N° de souche lignes**</span><span class="sxs-lookup"><span data-stu-id="b02a4-119">**Line No. Series**</span></span>|<span data-ttu-id="b02a4-120">Code souche de numéros pour les lignes du bordereau paiement.</span><span class="sxs-lookup"><span data-stu-id="b02a4-120">The number series code for the payment slip lines.</span></span> <span data-ttu-id="b02a4-121">Si vous laissez ce champ vide, le numéro de chaque ligne paiement est créé en se basant sur le numéro d'en-tête du bordereau paiement.</span><span class="sxs-lookup"><span data-stu-id="b02a4-121">If you leave this field blank, the number for each payment line is created based on the payment header number.</span></span>|  
    |<span data-ttu-id="b02a4-122">**Propositions**</span><span class="sxs-lookup"><span data-stu-id="b02a4-122">**Suggestions**</span></span>|<span data-ttu-id="b02a4-123">Type de proposition de règlement qui peut être créé automatiquement sur un bordereau paiement.</span><span class="sxs-lookup"><span data-stu-id="b02a4-123">The type of payment proposals that can be created automatically on a payment slip.</span></span>|  
    |<span data-ttu-id="b02a4-124">**Contrepassation de TVA sur encaissement**</span><span class="sxs-lookup"><span data-stu-id="b02a4-124">**Unrealized VAT Reversal**</span></span>|<span data-ttu-id="b02a4-125">Spécifiez la méthode pour gérer la TVA sur encaissement.</span><span class="sxs-lookup"><span data-stu-id="b02a4-125">Specify the method to handle unrealized VAT.</span></span><br /><br /> <span data-ttu-id="b02a4-126">Si vous sélectionnez **Lettrage**, la TVA sera réalisée lors de la validation du lettrage de la facture et du paiement.</span><span class="sxs-lookup"><span data-stu-id="b02a4-126">If you select **Application**, VAT will be realized when you post the invoice application and payment application.</span></span><br /><br /> <span data-ttu-id="b02a4-127">Si vous sélectionnez **En retard**, vous devez définir l'étape de règlement au cours de laquelle la TVA doit être réalisée, en sélectionnant le champ **Réaliser TVA** sur la page **Fiche étape règlement**.</span><span class="sxs-lookup"><span data-stu-id="b02a4-127">If you select **Delayed**, you must define the payment step during which VAT must be realized, by selecting the **Realize VAT** field on the **Payment Step Card** page.</span></span> <span data-ttu-id="b02a4-128">Pour plus d'informations, voir Réaliser TVA et Étape règlement.</span><span class="sxs-lookup"><span data-stu-id="b02a4-128">For more information, see Realize VAT and Payment Step.</span></span>|  
    |<span data-ttu-id="b02a4-129">**Type transfert SEPA**</span><span class="sxs-lookup"><span data-stu-id="b02a4-129">**SEPA Transfer Type**</span></span>|<span data-ttu-id="b02a4-130">Spécifiez le format d'exportation SEPA, **Virement** ou **Prélèvement**.</span><span class="sxs-lookup"><span data-stu-id="b02a4-130">Specify the SEPA export format, either **Credit Transfer** or **Direct Debit**.</span></span>|  

4.  <span data-ttu-id="b02a4-131">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="b02a4-131">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b02a4-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b02a4-132">See Also</span></span>  
 <span data-ttu-id="b02a4-133">[Gestion des paiements](payment-management.md) </span><span class="sxs-lookup"><span data-stu-id="b02a4-133">[Payment Management](payment-management.md) </span></span>  
 <span data-ttu-id="b02a4-134">[Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md) </span><span class="sxs-lookup"><span data-stu-id="b02a4-134">[Set Up Payment Statuses](how-to-set-up-payment-statuses.md) </span></span>  
 <span data-ttu-id="b02a4-135">[Paramétrer des étapes règlement](how-to-set-up-payment-steps.md) </span><span class="sxs-lookup"><span data-stu-id="b02a4-135">[Set Up Payment Steps](how-to-set-up-payment-steps.md) </span></span>  
 <span data-ttu-id="b02a4-136">[Configurer des adresses de paiement](how-to-set-up-payment-addresses.md) </span><span class="sxs-lookup"><span data-stu-id="b02a4-136">[Set Up Payment Addresses](how-to-set-up-payment-addresses.md) </span></span>  
 <span data-ttu-id="b02a4-137">[Exporter ou importer les paramètres de configuration de la gestion des paiements](how-to-export-or-import-payment-management-setup-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="b02a4-137">[Export or Import Payment Management Setup Parameters](how-to-export-or-import-payment-management-setup-parameters.md) </span></span>  
 <span data-ttu-id="b02a4-138">[Créer bordereaux paiement](how-to-create-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="b02a4-138">[Create Payment Slips](how-to-create-payment-slips.md) </span></span>  
 <span data-ttu-id="b02a4-139">[Valider des bordereaux paiement](how-to-post-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="b02a4-139">[Post Payment Slips](how-to-post-payment-slips.md) </span></span>  
 [<span data-ttu-id="b02a4-140">Archiver les bordereaux de paiement</span><span class="sxs-lookup"><span data-stu-id="b02a4-140">Archive Payment Slips</span></span>](how-to-archive-payment-slips.md)
