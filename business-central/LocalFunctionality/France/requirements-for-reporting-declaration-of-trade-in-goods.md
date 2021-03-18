---
title: Configuration requise pour la déclaration d'échanges de biens
description: Cette rubrique présente la liste des champs requis pour la déclaration d'échanges de biens (DEB) au format DTI+.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: ff3cdeb230b4e24ce4f2f3d24ee75e4fa4951b7f
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5381872"
---
# <a name="requirements-for-reporting-declaration-of-trade-in-goods"></a><span data-ttu-id="81c73-103">Configuration requise pour la déclaration d'échanges de biens</span><span class="sxs-lookup"><span data-stu-id="81c73-103">Requirements for Reporting Declaration of Trade in Goods</span></span>
<span data-ttu-id="81c73-104">Cette rubrique présente la liste des champs requis pour la déclaration d'échanges de biens (DEB) au format DTI+.</span><span class="sxs-lookup"><span data-stu-id="81c73-104">This topic shows a list of required fields that are needed for reporting Declaration of Trade in Goods (DEB) based on the DTI+ format.</span></span> <span data-ttu-id="81c73-105">Pour plus d'informations, voir Exporter DEB DTI.</span><span class="sxs-lookup"><span data-stu-id="81c73-105">For more information, see Export DEB DTI.</span></span>  

<span data-ttu-id="81c73-106">Les champs suivants sont requis pour la déclaration d'échanges de biens :</span><span class="sxs-lookup"><span data-stu-id="81c73-106">The following fields are required for reporting DEB:</span></span>  

- <span data-ttu-id="81c73-107">**CISD** dans la table **Informations société**.</span><span class="sxs-lookup"><span data-stu-id="81c73-107">**CISD** from the **Company Information** table.</span></span>  
- <span data-ttu-id="81c73-108">**N° SIRET** dans la table **Informations société**.</span><span class="sxs-lookup"><span data-stu-id="81c73-108">**Registration No.** from the **Company Information** table.</span></span>  
- <span data-ttu-id="81c73-109">**N° identif. intracomm.** dans la table **Informations société**.</span><span class="sxs-lookup"><span data-stu-id="81c73-109">**VAT Registration No.** from the **Company Information** table.</span></span>  
- <span data-ttu-id="81c73-110">**Nom** dans la table **Informations société**.</span><span class="sxs-lookup"><span data-stu-id="81c73-110">**Name** from the **Company Information** table.</span></span>  
- <span data-ttu-id="81c73-111">**Date** de la période statistique dans la table **Ligne feuille intracomm**.</span><span class="sxs-lookup"><span data-stu-id="81c73-111">**Date** for the statistics period from the **Intrastat Jnl. Line** table.</span></span>  
- <span data-ttu-id="81c73-112">**Régime** dans la table **Ligne feuille intracomm**.</span><span class="sxs-lookup"><span data-stu-id="81c73-112">**Transaction Specification** from the **Intrastat Jnl. Line** table.</span></span>  
- <span data-ttu-id="81c73-113">La **Quantité** dans la table **Ligne feuille intracomm** doit être supérieure à 0.</span><span class="sxs-lookup"><span data-stu-id="81c73-113">**Quantity** from the **Intrastat Jnl. Line** table must be greater than 0.</span></span>  
- <span data-ttu-id="81c73-114">La **Valeur statistique** dans la table **Ligne feuille intracomm** doit être supérieure à 0.</span><span class="sxs-lookup"><span data-stu-id="81c73-114">**Statistical Value** from the **Intrastat Jnl. Line** table must be greater than 0.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="81c73-115">L'état **Exporter DEB DTI** exporte les expéditions et les réceptions dans un lot.</span><span class="sxs-lookup"><span data-stu-id="81c73-115">The **Export DEB DTI** report exports shipments and receipts in one batch.</span></span> <span data-ttu-id="81c73-116">Si vous souhaitez déclarer uniquement les expéditions ou les réceptions, vous devez définir un filtre pour supprimer les lignes qui ne sont pas nécessaires dans la table **Feuille intracomm**.</span><span class="sxs-lookup"><span data-stu-id="81c73-116">If you want to report only shipments or receipts, then you must set a filter to remove the lines that are not needed in the **Intrastat Journal** table.</span></span>  

## <a name="see-also"></a><span data-ttu-id="81c73-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="81c73-117">See Also</span></span>  
[<span data-ttu-id="81c73-118">Fonctionnalité locale, France</span><span class="sxs-lookup"><span data-stu-id="81c73-118">France Local Functionality</span></span>](france-local-functionality.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]