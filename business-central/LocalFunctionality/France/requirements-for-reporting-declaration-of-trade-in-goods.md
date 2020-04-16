---
title: Configuration requise pour la déclaration d'échanges de biens
description: Cette rubrique présente la liste des champs requis pour la déclaration d'échanges de biens (DEB) au format DTI+.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 71d38f78893f749fe5f970a37d465911f832db0b
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/01/2020
ms.locfileid: "3181181"
---
# <a name="requirements-for-reporting-declaration-of-trade-in-goods"></a><span data-ttu-id="d375f-103">Configuration requise pour la déclaration d'échanges de biens</span><span class="sxs-lookup"><span data-stu-id="d375f-103">Requirements for Reporting Declaration of Trade in Goods</span></span>
<span data-ttu-id="d375f-104">Cette rubrique présente la liste des champs requis pour la déclaration d'échanges de biens (DEB) au format DTI+.</span><span class="sxs-lookup"><span data-stu-id="d375f-104">This topic shows a list of required fields that are needed for reporting Declaration of Trade in Goods (DEB) based on the DTI+ format.</span></span> <span data-ttu-id="d375f-105">Pour plus d'informations, voir Exporter DEB DTI.</span><span class="sxs-lookup"><span data-stu-id="d375f-105">For more information, see Export DEB DTI.</span></span>  

<span data-ttu-id="d375f-106">Les champs suivants sont requis pour la déclaration d'échanges de biens :</span><span class="sxs-lookup"><span data-stu-id="d375f-106">The following fields are required for reporting DEB:</span></span>  

- <span data-ttu-id="d375f-107">**CISD** dans la table **Informations société**.</span><span class="sxs-lookup"><span data-stu-id="d375f-107">**CISD** from the **Company Information** table.</span></span>  
- <span data-ttu-id="d375f-108">**N° SIRET** dans la table **Informations société**.</span><span class="sxs-lookup"><span data-stu-id="d375f-108">**Registration No.** from the **Company Information** table.</span></span>  
- <span data-ttu-id="d375f-109">**N° identif. intracomm.** dans la table **Informations société**.</span><span class="sxs-lookup"><span data-stu-id="d375f-109">**VAT Registration No.** from the **Company Information** table.</span></span>  
- <span data-ttu-id="d375f-110">**Nom** dans la table **Informations société**.</span><span class="sxs-lookup"><span data-stu-id="d375f-110">**Name** from the **Company Information** table.</span></span>  
- <span data-ttu-id="d375f-111">**Date** de la période statistique dans la table **Ligne feuille intracomm**.</span><span class="sxs-lookup"><span data-stu-id="d375f-111">**Date** for the statistics period from the **Intrastat Jnl. Line** table.</span></span>  
- <span data-ttu-id="d375f-112">**Régime** dans la table **Ligne feuille intracomm**.</span><span class="sxs-lookup"><span data-stu-id="d375f-112">**Transaction Specification** from the **Intrastat Jnl. Line** table.</span></span>  
- <span data-ttu-id="d375f-113">La **Quantité** dans la table **Ligne feuille intracomm** doit être supérieure à 0.</span><span class="sxs-lookup"><span data-stu-id="d375f-113">**Quantity** from the **Intrastat Jnl. Line** table must be greater than 0.</span></span>  
- <span data-ttu-id="d375f-114">La **Valeur statistique** dans la table **Ligne feuille intracomm** doit être supérieure à 0.</span><span class="sxs-lookup"><span data-stu-id="d375f-114">**Statistical Value** from the **Intrastat Jnl. Line** table must be greater than 0.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="d375f-115">L'état **Exporter DEB DTI** exporte les expéditions et les réceptions dans un lot.</span><span class="sxs-lookup"><span data-stu-id="d375f-115">The **Export DEB DTI** report exports shipments and receipts in one batch.</span></span> <span data-ttu-id="d375f-116">Si vous souhaitez déclarer uniquement les expéditions ou les réceptions, vous devez définir un filtre pour supprimer les lignes qui ne sont pas nécessaires dans la table **Feuille intracomm**.</span><span class="sxs-lookup"><span data-stu-id="d375f-116">If you want to report only shipments or receipts, then you must set a filter to remove the lines that are not needed in the **Intrastat Journal** table.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d375f-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d375f-117">See Also</span></span>  
[<span data-ttu-id="d375f-118">Fonctionnalité locale, France</span><span class="sxs-lookup"><span data-stu-id="d375f-118">France Local Functionality</span></span>](france-local-functionality.md)
