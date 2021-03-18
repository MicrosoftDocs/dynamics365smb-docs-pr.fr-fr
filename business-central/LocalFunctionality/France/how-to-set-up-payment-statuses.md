---
title: Procédure de paramétrage des statuts règlement
description: Pour utiliser le module de gestion des paiements, vous devez paramétrer des statuts règlement pour définir les niveaux de progression des documents règlement. Vous devez définir un ensemble de statuts pour chaque type de règlement.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 835d7dd2e018e38783d83f420dde73600e634d4b
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5381785"
---
# <a name="set-up-payment-statuses"></a><span data-ttu-id="d026e-104">Paramétrer des statuts règlement</span><span class="sxs-lookup"><span data-stu-id="d026e-104">Set Up Payment Statuses</span></span>
<span data-ttu-id="d026e-105">Pour utiliser le module de gestion des paiements, vous devez paramétrer des statuts règlement pour définir les niveaux de progression des documents règlement.</span><span class="sxs-lookup"><span data-stu-id="d026e-105">To use payment management, you must set up payment statuses to define payment document progress levels.</span></span> <span data-ttu-id="d026e-106">Vous devez définir un ensemble de statuts pour chaque type de règlement.</span><span class="sxs-lookup"><span data-stu-id="d026e-106">You must define a set of statuses for each payment class.</span></span> <span data-ttu-id="d026e-107">Pour plus d'informations, voir [Paramétrer des types de règlement](how-to-set-up-payment-classes.md).</span><span class="sxs-lookup"><span data-stu-id="d026e-107">For more information, see [Set Up Payment Classes](how-to-set-up-payment-classes.md).</span></span>  

## <a name="to-set-up-payment-statuses"></a><span data-ttu-id="d026e-108">Pour paramétrer des statuts règlement</span><span class="sxs-lookup"><span data-stu-id="d026e-108">To set up payment statuses</span></span>  

1.  <span data-ttu-id="d026e-109">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Paramètres bordereau paiement**, puis choisissez le lien associé.</span><span class="sxs-lookup"><span data-stu-id="d026e-109">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Slip Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d026e-110">Sélectionnez un type de règlement, puis cliquez sur **Statut**.</span><span class="sxs-lookup"><span data-stu-id="d026e-110">Select a payment class, and then choose the **Status** action.</span></span>  
3.  <span data-ttu-id="d026e-111">Sur la page **Statut règlement**, sélectionnez l'action **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="d026e-111">On the **Payment Status** page, choose the **New** action.</span></span>  
4.  <span data-ttu-id="d026e-112">Renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="d026e-112">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="d026e-113">Champ</span><span class="sxs-lookup"><span data-stu-id="d026e-113">Field</span></span>|<span data-ttu-id="d026e-114">Désignation</span><span class="sxs-lookup"><span data-stu-id="d026e-114">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="d026e-115">**Nom**</span><span class="sxs-lookup"><span data-stu-id="d026e-115">**Name**</span></span>|<span data-ttu-id="d026e-116">Description du statut de règlement.</span><span class="sxs-lookup"><span data-stu-id="d026e-116">The payment status description.</span></span>|  
    |<span data-ttu-id="d026e-117">**RIB**</span><span class="sxs-lookup"><span data-stu-id="d026e-117">**RIB**</span></span>|<span data-ttu-id="d026e-118">Permet d'indiquer que les informations relatives au Relevé d'Identité Bancaire (RIB) du client ou du fournisseur doivent être affichées dans les lignes paiement.</span><span class="sxs-lookup"><span data-stu-id="d026e-118">Select to indicate that information about the Relevé d Identité Bancaire (RIB) statement for the customer or vendor must be displayed in the payment lines.</span></span> <span data-ttu-id="d026e-119">Les informations du RIB incluent le code établissement, le code agence, le numéro de compte bancaire, le nom de la banque, la clé RIB et la clé de vérification.</span><span class="sxs-lookup"><span data-stu-id="d026e-119">The RIB information includes the bank branch number, agency code, bank account number, bank name, RIB key, and key verification.</span></span>|  
    |<span data-ttu-id="d026e-120">**Consultation**</span><span class="sxs-lookup"><span data-stu-id="d026e-120">**Look**</span></span>|<span data-ttu-id="d026e-121">Permet d'indiquer que les lignes document de règlement qui ont atteint ce statut peuvent être modifiées et affichées sur la page **Afficher/Éditer ligne paiement**.</span><span class="sxs-lookup"><span data-stu-id="d026e-121">Select to indicate that the payment document lines that have reached this payment status can be edited and viewed on the **View/Edit Payment Line** page.</span></span><br /><br /> <span data-ttu-id="d026e-122">Pour plus d'informations, voir Afficher/Éditer ligne paiement.</span><span class="sxs-lookup"><span data-stu-id="d026e-122">For more information, see View-Edit Payment Line.</span></span>|  
    |<span data-ttu-id="d026e-123">**ReportMenu**</span><span class="sxs-lookup"><span data-stu-id="d026e-123">**ReportMenu**</span></span>|<span data-ttu-id="d026e-124">Permet d'indiquer que les documents de règlement qui ont atteint ce statut peuvent être imprimés.</span><span class="sxs-lookup"><span data-stu-id="d026e-124">Select to indicate that the documents that have reached this payment status can be printed.</span></span>|  
    |<span data-ttu-id="d026e-125">**Montant**</span><span class="sxs-lookup"><span data-stu-id="d026e-125">**Amount**</span></span>|<span data-ttu-id="d026e-126">Permet d'afficher le montant dans les lignes règlement.</span><span class="sxs-lookup"><span data-stu-id="d026e-126">Select to display the amount in the payment lines.</span></span>|  
    |<span data-ttu-id="d026e-127">**Paiement en cours**</span><span class="sxs-lookup"><span data-stu-id="d026e-127">**Payment in Progress**</span></span>|<span data-ttu-id="d026e-128">Permet d'indiquer que toutes les lignes de facturation et paiement ayant ce statut doivent être prises en compte lors du calcul des paiements en cours.</span><span class="sxs-lookup"><span data-stu-id="d026e-128">Select to indicate that all billing and payment lines with this status must be considered when calculating the payments in progress.</span></span>|  
    |<span data-ttu-id="d026e-129">**Archivage autorisé**</span><span class="sxs-lookup"><span data-stu-id="d026e-129">**Archiving Authorized**</span></span>|<span data-ttu-id="d026e-130">Permet d'indiquer que les bordereaux avec ce statut peuvent être archivés.</span><span class="sxs-lookup"><span data-stu-id="d026e-130">Select to indicate that payment headers with this payment status can be archived.</span></span>|  

5.  <span data-ttu-id="d026e-131">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="d026e-131">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d026e-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d026e-132">See Also</span></span>  
 <span data-ttu-id="d026e-133">[Gestion des paiements](payment-management.md) </span><span class="sxs-lookup"><span data-stu-id="d026e-133">[Payment Management](payment-management.md) </span></span>  
 <span data-ttu-id="d026e-134">[Paramétrer des types de règlement](how-to-set-up-payment-classes.md) </span><span class="sxs-lookup"><span data-stu-id="d026e-134">[Set Up Payment Classes](how-to-set-up-payment-classes.md) </span></span>  
 <span data-ttu-id="d026e-135">[Paramétrer des étapes règlement](how-to-set-up-payment-steps.md) </span><span class="sxs-lookup"><span data-stu-id="d026e-135">[Set Up Payment Steps](how-to-set-up-payment-steps.md) </span></span>  
 <span data-ttu-id="d026e-136">[Configurer des adresses de paiement](how-to-set-up-payment-addresses.md) </span><span class="sxs-lookup"><span data-stu-id="d026e-136">[Set Up Payment Addresses](how-to-set-up-payment-addresses.md) </span></span>  
 <span data-ttu-id="d026e-137">[Créer bordereaux paiement](how-to-create-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="d026e-137">[Create Payment Slips](how-to-create-payment-slips.md) </span></span>  
 <span data-ttu-id="d026e-138">[Valider des bordereaux paiement](how-to-post-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="d026e-138">[Post Payment Slips](how-to-post-payment-slips.md) </span></span>  
 <span data-ttu-id="d026e-139">[Archiver les bordereaux de paiement](how-to-archive-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="d026e-139">[Archive Payment Slips](how-to-archive-payment-slips.md) </span></span>  
 [<span data-ttu-id="d026e-140">Exporter ou importer les paramètres de configuration de la gestion des paiements</span><span class="sxs-lookup"><span data-stu-id="d026e-140">Export or Import Payment Management Setup Parameters</span></span>](how-to-export-or-import-payment-management-setup-parameters.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]