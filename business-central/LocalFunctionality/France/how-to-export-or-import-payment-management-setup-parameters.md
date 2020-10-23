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
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 889069be54af7ed84ee090daca7d96d164348f9f
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/01/2020
ms.locfileid: "3920138"
---
# <a name="export-or-import-payment-management-setup-parameters"></a><span data-ttu-id="8fbe3-103">Exporter ou importer les paramètres de configuration de la gestion des paiements</span><span class="sxs-lookup"><span data-stu-id="8fbe3-103">Export or Import Payment Management Setup Parameters</span></span>
<span data-ttu-id="8fbe3-104">Vous pouvez exporter ou importer les paramètres de configuration de la gestion des paiements vers un disque externe afin de pouvoir utiliser les mêmes paramètres pour une autre société présentant les mêmes exigences.</span><span class="sxs-lookup"><span data-stu-id="8fbe3-104">You can export or import payment management setup parameters to an external disk so that you can use the same parameters for another company with similar requirements.</span></span>  

<span data-ttu-id="8fbe3-105">Vous pouvez utiliser les formats suivants pour exporter les paramètres de configuration de la gestion des paiements :</span><span class="sxs-lookup"><span data-stu-id="8fbe3-105">You can use the following formats to export payment setup parameters:</span></span>  

- <span data-ttu-id="8fbe3-106">ETEBAC (XMLport 10860) – Permet de créer une remise de lettre de change.</span><span class="sxs-lookup"><span data-stu-id="8fbe3-106">ETEBAC (XMLport 10860) – To create a bill of exchange remittance.</span></span>  
- <span data-ttu-id="8fbe3-107">Prélèvement (XMLport 10861) – Permet de créer un prélèvement de paiement client (débit direct).</span><span class="sxs-lookup"><span data-stu-id="8fbe3-107">Withdraw (XMLport 10861) – To create a customer payment withdrawal (direct debit).</span></span>  
- <span data-ttu-id="8fbe3-108">Transfert (XMLport 10862) – Permet de créer un transfert de paiement fournisseur (transfert de crédit).</span><span class="sxs-lookup"><span data-stu-id="8fbe3-108">Transfer (XMLport 10862) – To create a vendor payment transfer (credit transfer).</span></span>  

<span data-ttu-id="8fbe3-109">Vous pouvez sélectionner ces formats lorsque vous configurez le statut de règlement pour votre type de règlement.</span><span class="sxs-lookup"><span data-stu-id="8fbe3-109">You can select these formats when you set up the payment status for your payment class.</span></span> <span data-ttu-id="8fbe3-110">Pour plus d'informations, voir [Paramétrer des types de règlement](how-to-set-up-payment-classes.md).</span><span class="sxs-lookup"><span data-stu-id="8fbe3-110">For more information, see [Set Up Payment Classes](how-to-set-up-payment-classes.md).</span></span>  

## <a name="to-export-or-import-payment-management-setup-parameters"></a><span data-ttu-id="8fbe3-111">Pour exporter ou importer les paramètres de configuration de la gestion des paiements</span><span class="sxs-lookup"><span data-stu-id="8fbe3-111">To export or import payment management setup parameters</span></span>  

1.  <span data-ttu-id="8fbe3-112">Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Paramètres bordereau paiement**, puis choisissez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="8fbe3-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Slip Setup**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="8fbe3-113">Sur la page **Type règlement**, sélectionnez l'action **Exporter paramètres**.</span><span class="sxs-lookup"><span data-stu-id="8fbe3-113">On the **Payment Class** page, choose the **Export Parameters** action.</span></span>  

    <span data-ttu-id="8fbe3-114">Pour importer un paramètre, choisissez l'action **Importer paramètres**, sélectionnez le fichier, puis choisissez le bouton **Ouvrir**.</span><span class="sxs-lookup"><span data-stu-id="8fbe3-114">To import a parameter, choose the **Import Parameter** action, select the file, and then choose the **Open** button.</span></span>  

3.  <span data-ttu-id="8fbe3-115">Choisissez le bouton **Enregistrer** pour ouvrir la page **Enregistrer sous** et accéder à l'emplacement où le fichier doit être enregistré.</span><span class="sxs-lookup"><span data-stu-id="8fbe3-115">Choose the **Save** button to open the **Save As** page and navigate to the location where the file should be saved.</span></span>  
4.  <span data-ttu-id="8fbe3-116">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="8fbe3-116">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8fbe3-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8fbe3-117">See Also</span></span>  
 <span data-ttu-id="8fbe3-118">[Gestion des paiements](payment-management.md) </span><span class="sxs-lookup"><span data-stu-id="8fbe3-118">[Payment Management](payment-management.md) </span></span>  
 <span data-ttu-id="8fbe3-119">[Paramétrer des types de règlement](how-to-set-up-payment-classes.md) </span><span class="sxs-lookup"><span data-stu-id="8fbe3-119">[Set Up Payment Classes](how-to-set-up-payment-classes.md) </span></span>  
 <span data-ttu-id="8fbe3-120">[Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md) </span><span class="sxs-lookup"><span data-stu-id="8fbe3-120">[Set Up Payment Statuses](how-to-set-up-payment-statuses.md) </span></span>  
 <span data-ttu-id="8fbe3-121">[Paramétrer des étapes règlement](how-to-set-up-payment-steps.md) </span><span class="sxs-lookup"><span data-stu-id="8fbe3-121">[Set Up Payment Steps](how-to-set-up-payment-steps.md) </span></span>  
 <span data-ttu-id="8fbe3-122">[Configurer des adresses de paiement](how-to-set-up-payment-addresses.md) </span><span class="sxs-lookup"><span data-stu-id="8fbe3-122">[Set Up Payment Addresses](how-to-set-up-payment-addresses.md) </span></span>  
 <span data-ttu-id="8fbe3-123">[Créer bordereaux paiement](how-to-create-payment-slips.md) </span><span class="sxs-lookup"><span data-stu-id="8fbe3-123">[Create Payment Slips](how-to-create-payment-slips.md) </span></span>  
 [<span data-ttu-id="8fbe3-124">Archiver les bordereaux de paiement</span><span class="sxs-lookup"><span data-stu-id="8fbe3-124">Archive Payment Slips</span></span>](how-to-archive-payment-slips.md)
