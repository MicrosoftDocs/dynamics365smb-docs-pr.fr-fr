---
title: Gestion des paiements
description: Vous pouvez gérer des lettres de change, des paiements électroniques et des paiements fournisseur à l'aide de la fonction de gestion des paiements.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: fbe48dafa2393f22418771bdb321f47c5dd71f3a
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/17/2020
ms.locfileid: "4749645"
---
# <a name="payment-management"></a><span data-ttu-id="dda8b-103">Gestion des paiements</span><span class="sxs-lookup"><span data-stu-id="dda8b-103">Payment Management</span></span>
[!INCLUDE[prod_short](../../includes/prod_short.md)] <span data-ttu-id="dda8b-104">vous permet de gérer des lettres de change, des paiements électroniques et des paiements fournisseur à l'aide de la fonction de gestion des paiements.</span><span class="sxs-lookup"><span data-stu-id="dda8b-104">allows you to manage bills of exchange, electronic payments, and vendor payments using the payment management function.</span></span>  

<span data-ttu-id="dda8b-105">Vous pouvez gérer les paiements fournisseur et client à l'aide des bordereaux paiement.</span><span class="sxs-lookup"><span data-stu-id="dda8b-105">You can manage customer and vendor payments using payment slips.</span></span> <span data-ttu-id="dda8b-106">Avant de créer un bordereau paiement, vous devez définir les paramétrages suivants :</span><span class="sxs-lookup"><span data-stu-id="dda8b-106">Before you create a payment slip, you must set up the following prerequisites:</span></span>  

- <span data-ttu-id="dda8b-107">Type de règlement – Type de règlement que vous souhaitez effectuer, comme par exemple, une lettre de change, un paiement électronique ou un chèque.</span><span class="sxs-lookup"><span data-stu-id="dda8b-107">Payment class – The type of payment that you want to perform, for example, bill of exchange, electronic payment, or check.</span></span> <span data-ttu-id="dda8b-108">Pour plus d'informations, voir [Paramétrer des types de règlement](how-to-set-up-payment-classes.md).</span><span class="sxs-lookup"><span data-stu-id="dda8b-108">For more information, see [Set Up Payment Classes](how-to-set-up-payment-classes.md).</span></span>  

- <span data-ttu-id="dda8b-109">Statut règlement – Niveau de progression d'un document règlement.</span><span class="sxs-lookup"><span data-stu-id="dda8b-109">Payment status – The progress level of a payment document.</span></span> <span data-ttu-id="dda8b-110">Vous devez définir un ensemble de statuts pour chaque type de règlement.</span><span class="sxs-lookup"><span data-stu-id="dda8b-110">You must define a set of statuses for each payment class.</span></span> <span data-ttu-id="dda8b-111">Pour plus d'informations, voir [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md).</span><span class="sxs-lookup"><span data-stu-id="dda8b-111">For more information, see [Set Up Payment Statuses](how-to-set-up-payment-statuses.md).</span></span>  

- <span data-ttu-id="dda8b-112">Étapes de règlement – Paiement qui est exécuté à un moment spécifié.</span><span class="sxs-lookup"><span data-stu-id="dda8b-112">Payment steps – A payment that is executed at a specified time.</span></span> <span data-ttu-id="dda8b-113">Une fois l'étape de règlement exécutée, vous pouvez passer d'un statut du document règlement à un autre.</span><span class="sxs-lookup"><span data-stu-id="dda8b-113">After a payment step is completed, you can move the payment document from one status to another.</span></span> <span data-ttu-id="dda8b-114">Si une étape nécessite la validation d'enregistrements débiteurs ou créditeurs, vous devez définir d'autres actions dans la table **Etape règlement : Comptabilisation**.</span><span class="sxs-lookup"><span data-stu-id="dda8b-114">If a step involves posting debit or credit entries, you must define additional actions in the **Payment Step Ledger** table.</span></span> <span data-ttu-id="dda8b-115">Pour plus d'informations, voir [Paramétrer des étapes de règlement](how-to-set-up-payment-steps.md).</span><span class="sxs-lookup"><span data-stu-id="dda8b-115">For more information, see [Set Up Payment Steps](how-to-set-up-payment-steps.md).</span></span>  

- <span data-ttu-id="dda8b-116">Adresse de règlement pour les fournisseurs et les clients – Adresse qui est utilisée pour un fournisseur ou un client au moment du règlement.</span><span class="sxs-lookup"><span data-stu-id="dda8b-116">Payment address for vendors and customers – The address that is used for a vendor or a customer at the time of settlement.</span></span> <span data-ttu-id="dda8b-117">L'adresse de règlement peut être différente de celle par défaut du client ou du fournisseur.</span><span class="sxs-lookup"><span data-stu-id="dda8b-117">The payment address can be different from the vendor’s or customer's default address.</span></span> <span data-ttu-id="dda8b-118">Pour plus d'informations, voir [Paramétrer des adresses de règlement](how-to-set-up-payment-addresses.md).</span><span class="sxs-lookup"><span data-stu-id="dda8b-118">For more information, see [Set Up Payment Addresses](how-to-set-up-payment-addresses.md).</span></span>  

<span data-ttu-id="dda8b-119">Vous pouvez également transférer vos informations de configuration de la gestion des paiements vers un disque externe afin de pouvoir utiliser les mêmes paramètres pour une autre société présentant les mêmes exigences.</span><span class="sxs-lookup"><span data-stu-id="dda8b-119">You can also transfer your payment management setup information to an external disk so that you can use the same parameters for another company with similar requirements.</span></span> <span data-ttu-id="dda8b-120">Vous pouvez exporter les données de paiement dans les formats suivants :</span><span class="sxs-lookup"><span data-stu-id="dda8b-120">You can export the payment data in the following formats:</span></span>  

- <span data-ttu-id="dda8b-121">ETEBAC – Permet de créer une remise de lettre de change.</span><span class="sxs-lookup"><span data-stu-id="dda8b-121">ETEBAC – To create a bill of exchange remittance.</span></span>  
- <span data-ttu-id="dda8b-122">Prélèvement – Permet de créer un prélèvement de paiement client (débit direct).</span><span class="sxs-lookup"><span data-stu-id="dda8b-122">Withdraw – To create a customer payment withdrawal (direct debit).</span></span>  
- <span data-ttu-id="dda8b-123">Transfert – Permet de créer un transfert de paiement fournisseur (transfert de crédit).</span><span class="sxs-lookup"><span data-stu-id="dda8b-123">Transfer – To create a vendor payment transfer (credit transfer).</span></span>  

## <a name="managing-payment-slips-and-files"></a><span data-ttu-id="dda8b-124">Gestion des bordereaux et des fichiers paiement</span><span class="sxs-lookup"><span data-stu-id="dda8b-124">Managing Payment Slips and Files</span></span>  
<span data-ttu-id="dda8b-125">Vous pouvez créer des bordereaux paiement pour gérer les paiements client et fournisseur.</span><span class="sxs-lookup"><span data-stu-id="dda8b-125">You can create payment slips to manage customer payments and vendor payments.</span></span> <span data-ttu-id="dda8b-126">Après avoir créé le bordereau paiement, vous devez le valider.</span><span class="sxs-lookup"><span data-stu-id="dda8b-126">After creating the payment slip, you must post it.</span></span>  

<span data-ttu-id="dda8b-127">Ces bordereaux paiement peuvent être convertis en fichiers de paiement, qui peuvent être envoyés à la banque par voie électronique.</span><span class="sxs-lookup"><span data-stu-id="dda8b-127">These payment slips can then be converted into payment files, which can be sent to the bank electronically.</span></span>  

<span data-ttu-id="dda8b-128">Pour plus d'informations, consultez [Créer des bordereaux paiement](how-to-create-payment-slips.md).</span><span class="sxs-lookup"><span data-stu-id="dda8b-128">For more information, see [Create Payment Slips](how-to-create-payment-slips.md).</span></span>  

## <a name="archiving-payment-slips"></a><span data-ttu-id="dda8b-129">Archivage des bordereaux paiement</span><span class="sxs-lookup"><span data-stu-id="dda8b-129">Archiving Payment Slips</span></span>  
<span data-ttu-id="dda8b-130">Vous pouvez séparer un bordereau paiement entièrement traité des bordereaux paiement actifs en l'archivant.</span><span class="sxs-lookup"><span data-stu-id="dda8b-130">You can separate a fully processed payment slip from the active payment slips by archiving it.</span></span> <span data-ttu-id="dda8b-131">Vous pouvez archiver un bordereau paiement manuellement ou vous pouvez archiver un lot de bordereaux automatiquement.</span><span class="sxs-lookup"><span data-stu-id="dda8b-131">You can manually archive an individual payment slip or you can automatically archive a batch of payment slips.</span></span> <span data-ttu-id="dda8b-132">Pour plus d'informations, consultez [Archiver des bordereaux paiement](how-to-archive-payment-slips.md).</span><span class="sxs-lookup"><span data-stu-id="dda8b-132">For more information, see [Archive Payment Slips](how-to-archive-payment-slips.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="dda8b-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dda8b-133">See Also</span></span>  
 <span data-ttu-id="dda8b-134">[Paramétrer des types de règlement](how-to-set-up-payment-classes.md) </span><span class="sxs-lookup"><span data-stu-id="dda8b-134">[Set Up Payment Classes](how-to-set-up-payment-classes.md) </span></span>  
 <span data-ttu-id="dda8b-135">[Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md) </span><span class="sxs-lookup"><span data-stu-id="dda8b-135">[Set Up Payment Statuses](how-to-set-up-payment-statuses.md) </span></span>  
 <span data-ttu-id="dda8b-136">[Paramétrer des étapes règlement](how-to-set-up-payment-steps.md) </span><span class="sxs-lookup"><span data-stu-id="dda8b-136">[Set Up Payment Steps](how-to-set-up-payment-steps.md) </span></span>  
 <span data-ttu-id="dda8b-137">[Configurer des adresses de paiement](how-to-set-up-payment-addresses.md) </span><span class="sxs-lookup"><span data-stu-id="dda8b-137">[Set Up Payment Addresses](how-to-set-up-payment-addresses.md) </span></span>  
 <span data-ttu-id="dda8b-138">[Créer bordereaux paiement](how-to-create-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="dda8b-138">[Create Payment Slips](how-to-create-payment-slips.md) </span></span>  
 <span data-ttu-id="dda8b-139">[Valider des bordereaux paiement](how-to-post-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="dda8b-139">[Post Payment Slips](how-to-post-payment-slips.md) </span></span>  
 <span data-ttu-id="dda8b-140">[Archiver les bordereaux de paiement](how-to-archive-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="dda8b-140">[Archive Payment Slips](how-to-archive-payment-slips.md) </span></span>  
 <span data-ttu-id="dda8b-141">[Exporter ou importer les paramètres de configuration de la gestion des paiements](how-to-export-or-import-payment-management-setup-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="dda8b-141">[Export or Import Payment Management Setup Parameters](how-to-export-or-import-payment-management-setup-parameters.md) </span></span>  
 [<span data-ttu-id="dda8b-142">Fonctionnalité locale, France</span><span class="sxs-lookup"><span data-stu-id="dda8b-142">France Local Functionality</span></span>](france-local-functionality.md)
