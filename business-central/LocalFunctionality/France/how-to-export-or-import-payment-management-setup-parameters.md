---
title: Procédure d'exportation ou d'importation des paramètres de configuration de la gestion des paiements
description: Vous pouvez exporter ou importer les paramètres de configuration de la gestion des paiements vers un disque externe afin de pouvoir utiliser les mêmes paramètres pour une autre société présentant les mêmes exigences.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 829a641d94c810277390b552187e1aaacd803f1d
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2019
ms.locfileid: "936525"
---
# <a name="export-or-import-payment-management-setup-parameters"></a><span data-ttu-id="64735-103">Exporter ou importer les paramètres de configuration de la gestion des paiements</span><span class="sxs-lookup"><span data-stu-id="64735-103">Export or Import Payment Management Setup Parameters</span></span>
<span data-ttu-id="64735-104">Vous pouvez exporter ou importer les paramètres de configuration de la gestion des paiements vers un disque externe afin de pouvoir utiliser les mêmes paramètres pour une autre société présentant les mêmes exigences.</span><span class="sxs-lookup"><span data-stu-id="64735-104">You can export or import payment management setup parameters to an external disk so that you can use the same parameters for another company with similar requirements.</span></span>  

<span data-ttu-id="64735-105">Vous pouvez utiliser les formats suivants pour exporter les paramètres de configuration de la gestion des paiements :</span><span class="sxs-lookup"><span data-stu-id="64735-105">You can use the following formats to export payment setup parameters:</span></span>  

- <span data-ttu-id="64735-106">ETEBAC (XMLport 10860) – Permet de créer une remise de lettre de change.</span><span class="sxs-lookup"><span data-stu-id="64735-106">ETEBAC (XMLport 10860) – To create a bill of exchange remittance.</span></span>  
- <span data-ttu-id="64735-107">Prélèvement (XMLport 10861) – Permet de créer un prélèvement de paiement client (débit direct).</span><span class="sxs-lookup"><span data-stu-id="64735-107">Withdraw (XMLport 10861) – To create a customer payment withdrawal (direct debit).</span></span>  
- <span data-ttu-id="64735-108">Transfert (XMLport 10862) – Permet de créer un transfert de paiement fournisseur (transfert de crédit).</span><span class="sxs-lookup"><span data-stu-id="64735-108">Transfer (XMLport 10862) – To create a vendor payment transfer (credit transfer).</span></span>  

<span data-ttu-id="64735-109">Vous pouvez sélectionner ces formats lorsque vous configurez le statut de règlement pour votre type de règlement.</span><span class="sxs-lookup"><span data-stu-id="64735-109">You can select these formats when you set up the payment status for your payment class.</span></span> <span data-ttu-id="64735-110">Pour plus d'informations, voir [Paramétrer des types de règlement](how-to-set-up-payment-classes.md).</span><span class="sxs-lookup"><span data-stu-id="64735-110">For more information, see [Set Up Payment Classes](how-to-set-up-payment-classes.md).</span></span>  

## <a name="to-export-or-import-payment-management-setup-parameters"></a><span data-ttu-id="64735-111">Pour exporter ou importer les paramètres de configuration de la gestion des paiements</span><span class="sxs-lookup"><span data-stu-id="64735-111">To export or import payment management setup parameters</span></span>  

1.  <span data-ttu-id="64735-112">Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Paramètres bordereau paiement**, puis sélectionnez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="64735-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Slip Setup**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="64735-113">Sur la page **Type règlement**, sélectionnez l'action **Exporter paramètres**.</span><span class="sxs-lookup"><span data-stu-id="64735-113">On the **Payment Class** page, choose the **Export Parameters** action.</span></span>  

    <span data-ttu-id="64735-114">Pour importer un paramètre, choisissez l'action **Importer paramètres**, sélectionnez le fichier, puis choisissez le bouton **Ouvrir**.</span><span class="sxs-lookup"><span data-stu-id="64735-114">To import a parameter, choose the **Import Parameter** action, select the file, and then choose the **Open** button.</span></span>  

3.  <span data-ttu-id="64735-115">Choisissez le bouton **Enregistrer** pour ouvrir la page **Enregistrer sous** et accéder à l'emplacement où le fichier doit être enregistré.</span><span class="sxs-lookup"><span data-stu-id="64735-115">Choose the **Save** button to open the **Save As** page and navigate to the location where the file should be saved.</span></span>  
4.  <span data-ttu-id="64735-116">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="64735-116">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="64735-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="64735-117">See Also</span></span>  
 <span data-ttu-id="64735-118">[Gestion des paiements](payment-management.md) </span><span class="sxs-lookup"><span data-stu-id="64735-118">[Payment Management](payment-management.md) </span></span>  
 <span data-ttu-id="64735-119">[Paramétrer des types de règlement](how-to-set-up-payment-classes.md) </span><span class="sxs-lookup"><span data-stu-id="64735-119">[Set Up Payment Classes](how-to-set-up-payment-classes.md) </span></span>  
 <span data-ttu-id="64735-120">[Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md) </span><span class="sxs-lookup"><span data-stu-id="64735-120">[Set Up Payment Statuses](how-to-set-up-payment-statuses.md) </span></span>  
 <span data-ttu-id="64735-121">[Paramétrer des étapes règlement](how-to-set-up-payment-steps.md) </span><span class="sxs-lookup"><span data-stu-id="64735-121">[Set Up Payment Steps](how-to-set-up-payment-steps.md) </span></span>  
 <span data-ttu-id="64735-122">[Configurer des adresses de paiement](how-to-set-up-payment-addresses.md) </span><span class="sxs-lookup"><span data-stu-id="64735-122">[Set Up Payment Addresses](how-to-set-up-payment-addresses.md) </span></span>  
 <span data-ttu-id="64735-123">[Créer bordereaux paiement](how-to-create-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="64735-123">[Create Payment Slips](how-to-create-payment-slips.md) </span></span>  
 [<span data-ttu-id="64735-124">Archiver les bordereaux de paiement</span><span class="sxs-lookup"><span data-stu-id="64735-124">Archive Payment Slips</span></span>](how-to-archive-payment-slips.md)
