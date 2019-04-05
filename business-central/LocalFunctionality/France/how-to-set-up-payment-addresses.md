---
title: Procédure de paramétrage des adresses de règlement
description: Pour utiliser le module Gestion des paiements, vous devez paramétrer les adresses de règlement qui sont utilisées pour les fournisseurs et clients au moment du règlement. L'adresse de règlement peut différer de l'adresse par défaut.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: fe778b4125db66fb288f2a09b5e372fc8e3d065b
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2019
ms.locfileid: "826633"
---
# <a name="set-up-payment-addresses"></a><span data-ttu-id="0d66c-104">Configurer des adresses de paiement</span><span class="sxs-lookup"><span data-stu-id="0d66c-104">Set Up Payment Addresses</span></span>
<span data-ttu-id="0d66c-105">Pour utiliser le module Gestion des paiements, vous devez paramétrer les adresses de règlement qui sont utilisées pour les fournisseurs et clients au moment du règlement.</span><span class="sxs-lookup"><span data-stu-id="0d66c-105">To use payment management, you must set up payment addresses that will be used for vendors and customers at the time of settlement.</span></span> <span data-ttu-id="0d66c-106">L'adresse de règlement peut différer de l'adresse par défaut.</span><span class="sxs-lookup"><span data-stu-id="0d66c-106">The payment address can differ from the default address.</span></span>  

<span data-ttu-id="0d66c-107">La procédure suivante décrit comment paramétrer une adresse de règlement pour un fournisseur, mais les mêmes étapes s'appliquent pour le paramétrage d'une adresse de règlement pour un client.</span><span class="sxs-lookup"><span data-stu-id="0d66c-107">The following procedure describes how to set up a payment address for a vendor, but the same steps apply to setting up a payment address for a customer.</span></span>  

## <a name="to-set-up-a-payment-address"></a><span data-ttu-id="0d66c-108">Pour paramétrer une adresse de règlement</span><span class="sxs-lookup"><span data-stu-id="0d66c-108">To set up a payment address</span></span>  

1.  <span data-ttu-id="0d66c-109">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Fournisseurs**, puis sélectionnez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="0d66c-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="0d66c-110">Sélectionnez un fournisseur, puis cliquez sur **Modifier**.</span><span class="sxs-lookup"><span data-stu-id="0d66c-110">Select a vendor, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="0d66c-111">Choisissez l'option **Adresses de règlement**.</span><span class="sxs-lookup"><span data-stu-id="0d66c-111">Choose the **Payment Addresses** action.</span></span>  
4.  <span data-ttu-id="0d66c-112">Renseignez les champs requis comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="0d66c-112">Fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="0d66c-113">Champ</span><span class="sxs-lookup"><span data-stu-id="0d66c-113">Field</span></span>|<span data-ttu-id="0d66c-114">Désignation</span><span class="sxs-lookup"><span data-stu-id="0d66c-114">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="0d66c-115">**Code**</span><span class="sxs-lookup"><span data-stu-id="0d66c-115">**Code**</span></span>|<span data-ttu-id="0d66c-116">Code adresse de règlement.</span><span class="sxs-lookup"><span data-stu-id="0d66c-116">The payment address code.</span></span>|  
    |<span data-ttu-id="0d66c-117">**Valeur par défaut**</span><span class="sxs-lookup"><span data-stu-id="0d66c-117">**Default Value**</span></span>|<span data-ttu-id="0d66c-118">Permet d'utiliser cette adresse comme adresse de règlement par défaut.</span><span class="sxs-lookup"><span data-stu-id="0d66c-118">Select to use this address as the default payment address.</span></span> <span data-ttu-id="0d66c-119">Vous pouvez sélectionner une adresse de règlement par défaut.</span><span class="sxs-lookup"><span data-stu-id="0d66c-119">You can select one default payment address.</span></span>|  
    |<span data-ttu-id="0d66c-120">**Nom**</span><span class="sxs-lookup"><span data-stu-id="0d66c-120">**Name**</span></span>|<span data-ttu-id="0d66c-121">Nom associé à l'adresse de règlement.</span><span class="sxs-lookup"><span data-stu-id="0d66c-121">The name associated with the payment address.</span></span>|  
    |<span data-ttu-id="0d66c-122">**Adresse**</span><span class="sxs-lookup"><span data-stu-id="0d66c-122">**Address**</span></span>|<span data-ttu-id="0d66c-123">Adresse de règlement.</span><span class="sxs-lookup"><span data-stu-id="0d66c-123">The payment address.</span></span>|  

    5.  <span data-ttu-id="0d66c-124">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="0d66c-124">Choose the **OK** button.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0d66c-125">Si une adresse de règlement n'est pas configurée, l'adresse indiquée sur la fiche fournisseur ou client est définie comme valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="0d66c-125">If a payment address is not set up, the address in the vendor or customer card is set as the default value.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0d66c-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0d66c-126">See Also</span></span>  
 <span data-ttu-id="0d66c-127">[Gestion des paiements](payment-management.md) </span><span class="sxs-lookup"><span data-stu-id="0d66c-127">[Payment Management](payment-management.md) </span></span>  
 <span data-ttu-id="0d66c-128">[Paramétrer des types de règlement](how-to-set-up-payment-classes.md) </span><span class="sxs-lookup"><span data-stu-id="0d66c-128">[Set Up Payment Classes](how-to-set-up-payment-classes.md) </span></span>  
 <span data-ttu-id="0d66c-129">[Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md) </span><span class="sxs-lookup"><span data-stu-id="0d66c-129">[Set Up Payment Statuses](how-to-set-up-payment-statuses.md) </span></span>  
 <span data-ttu-id="0d66c-130">[Paramétrer des étapes règlement](how-to-set-up-payment-steps.md) </span><span class="sxs-lookup"><span data-stu-id="0d66c-130">[Set Up Payment Steps](how-to-set-up-payment-steps.md) </span></span>  
 <span data-ttu-id="0d66c-131">[Créer bordereaux paiement](how-to-create-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="0d66c-131">[Create Payment Slips](how-to-create-payment-slips.md) </span></span>  
 <span data-ttu-id="0d66c-132">[Valider des bordereaux paiement](how-to-post-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="0d66c-132">[Post Payment Slips](how-to-post-payment-slips.md) </span></span>  
 <span data-ttu-id="0d66c-133">[Archiver les bordereaux de paiement](how-to-archive-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="0d66c-133">[Archive Payment Slips](how-to-archive-payment-slips.md) </span></span>  
 <span data-ttu-id="0d66c-134">[Exporter ou importer les paramètres de configuration de la gestion des paiements](how-to-export-or-import-payment-management-setup-parameters.md)</span><span class="sxs-lookup"><span data-stu-id="0d66c-134">[Export or Import Payment Management Setup Parameters](how-to-export-or-import-payment-management-setup-parameters.md)s</span></span>
