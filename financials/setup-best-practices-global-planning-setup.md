---
title: "Pratiques recommandées pour la configuration du planning général | Microsoft Docs"
description: "Le raccourci **Planning** de la fenêtre **Paramètres production** comporte plusieurs champs permettant de définir les règles globales pour la planification des approvisionnements."
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: f1a4e3a30d4d665a83ab599ad19dfd3760d744b2
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="setup-best-practices-global-planning-setup"></a><span data-ttu-id="514ed-103">Configurer des recommandations : configuration du planning général</span><span class="sxs-lookup"><span data-stu-id="514ed-103">Setup Best Practices: Global Planning Setup</span></span>
<span data-ttu-id="514ed-104">Le raccourci **Planning** de la fenêtre**Paramètres production** comporte plusieurs champs permettant de définir les règles globales pour la planification des approvisionnements.</span><span class="sxs-lookup"><span data-stu-id="514ed-104">The **Planning** FastTab in the **Manufacturing Setup** window contains several fields that define global rules for supply planning.</span></span>  

 <span data-ttu-id="514ed-105">Le tableau suivant fournit les meilleures pratiques sur la procédure de configuration de champs paramètres sélectionnés de planification générale.</span><span class="sxs-lookup"><span data-stu-id="514ed-105">The following table provides best practices on how to set up selected global planning parameter fields.</span></span> <span data-ttu-id="514ed-106">Pour plus d'informations sur un champ donné, sélectionnez le lien correspondant dans la colonne **Configuration d'un champ**.</span><span class="sxs-lookup"><span data-stu-id="514ed-106">For more information about a field, choose the link in the **Setup field** column.</span></span>  

|<span data-ttu-id="514ed-107">Paramétrage de champ</span><span class="sxs-lookup"><span data-stu-id="514ed-107">Setup field</span></span>|<span data-ttu-id="514ed-108">Meilleure pratique</span><span class="sxs-lookup"><span data-stu-id="514ed-108">Best practice</span></span>|<span data-ttu-id="514ed-109">Commentaire</span><span class="sxs-lookup"><span data-stu-id="514ed-109">Comment</span></span>|  
|-----------------|-------------------|-------------|  
|<span data-ttu-id="514ed-110">Prévision sur magasin</span><span class="sxs-lookup"><span data-stu-id="514ed-110">Use Forecast on Locations</span></span>|<span data-ttu-id="514ed-111">Indiquez si vous avez des prévisions pour des entrepôts spécifiques.</span><span class="sxs-lookup"><span data-stu-id="514ed-111">Select if you have forecasts for specific locations.</span></span>||  
|<span data-ttu-id="514ed-112">Mag. composant par déf.</span><span class="sxs-lookup"><span data-stu-id="514ed-112">Components at Location</span></span>|<span data-ttu-id="514ed-113">Si les articles ne sont pas définis comme points de stock, sélectionnez le code magasin de l'entrepôt principal.</span><span class="sxs-lookup"><span data-stu-id="514ed-113">If items are not defined as SKUs, select the location code of your main warehouse.</span></span>|<span data-ttu-id="514ed-114">Cela s'applique également si vous utilisez uniquement la demande achat.</span><span class="sxs-lookup"><span data-stu-id="514ed-114">This also applies if you only use the requisition worksheet.</span></span>|  
|<span data-ttu-id="514ed-115">Niveau de dépassement de capacité vide</span><span class="sxs-lookup"><span data-stu-id="514ed-115">Blank Overflow Level</span></span>|<span data-ttu-id="514ed-116">Sélectionnez **Autoriser calcul par défaut** si vous effectuez une migration de Microsoft Dynamics NAV 5.0 ou d'une version antérieure.</span><span class="sxs-lookup"><span data-stu-id="514ed-116">Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.</span></span>|<span data-ttu-id="514ed-117">Ne l'utilisez que si vous souhaitez autoriser tout ou partie de vos articles à franchir le point de réapprovisionnement.</span><span class="sxs-lookup"><span data-stu-id="514ed-117">Use only if you want to allow all or some of your items to overflow the reorder point.</span></span>|  
|<span data-ttu-id="514ed-118">Période tampon par défaut</span><span class="sxs-lookup"><span data-stu-id="514ed-118">Default Dampener Period</span></span>|<span data-ttu-id="514ed-119">Doit être compris entre 1D et 5D.</span><span class="sxs-lookup"><span data-stu-id="514ed-119">Set between 1D and 5D.</span></span><br /><br /> <span data-ttu-id="514ed-120">Si vous débutez en planification avec [!INCLUDE[d365fin](includes/d365fin_md.md)], définissez une plus longue période.</span><span class="sxs-lookup"><span data-stu-id="514ed-120">If new to planning in [!INCLUDE[d365fin](includes/d365fin_md.md)], then set a longer period.</span></span>|<span data-ttu-id="514ed-121">Quand les utilisateurs sont plus au fait des différents motifs des messages d'action, raccourcissez la période tampon pour autoriser plus de propositions de modification.</span><span class="sxs-lookup"><span data-stu-id="514ed-121">When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions.</span></span>|  
|<span data-ttu-id="514ed-122">Quantité tampon par défaut</span><span class="sxs-lookup"><span data-stu-id="514ed-122">Default Dampener Quantity</span></span>|<span data-ttu-id="514ed-123">Définissez à entre 5 et 20 % de la taille du lot de l'article.</span><span class="sxs-lookup"><span data-stu-id="514ed-123">Set between 5 and 20 percent of the item’s lot size.</span></span>||  

## <a name="see-also"></a><span data-ttu-id="514ed-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="514ed-124">See Also</span></span>  
 <span data-ttu-id="514ed-125">[Pratiques de configuration recommandées : planification de l'approvisionnement](setup-best-practices-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="514ed-125">[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md) </span></span>  
 <span data-ttu-id="514ed-126">[Détails de conception : planification de l'approvisionnement](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="514ed-126">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
 [<span data-ttu-id="514ed-127">Configurer les modules complexes à l'aide des meilleures pratiques</span><span class="sxs-lookup"><span data-stu-id="514ed-127">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="514ed-128">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="514ed-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
