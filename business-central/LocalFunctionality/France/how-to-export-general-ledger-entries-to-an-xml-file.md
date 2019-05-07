---
title: Procédure d'exportation des écritures comptables vers un fichier XML
description: Pour l'archivage externe, et pour une période donnée, vous pouvez exporter des transactions financières vers un fichier XML.
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
ms.openlocfilehash: 708385d43f1f9363d82853110550997ef26c2efd
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2019
ms.locfileid: "915864"
---
# <a name="export-general-ledger-entries-to-an-xml-file"></a><span data-ttu-id="9f27c-103">Exporter des écritures comptables vers un fichier XML</span><span class="sxs-lookup"><span data-stu-id="9f27c-103">Export General Ledger Entries to an XML File</span></span>
<span data-ttu-id="9f27c-104">Pour l'archivage externe, et pour une période donnée, vous pouvez exporter des transactions financières vers un fichier XML.</span><span class="sxs-lookup"><span data-stu-id="9f27c-104">You can export financial transactions for a particular period to an XML file for external archiving.</span></span> <span data-ttu-id="9f27c-105">À la fin de l'exercice comptable, vous pouvez exporter les transactions comptables pour l'année clôturée en appliquant le filtre de date approprié et en exportant les transactions financières dans la période indiquée vers le fichier XML.</span><span class="sxs-lookup"><span data-stu-id="9f27c-105">After the closing of the fiscal year, you can export the general ledger transactions for the closed year by applying the correct date filter and then exporting the financial transactions within the specified period to the XML file.</span></span> <span data-ttu-id="9f27c-106">Le fichier XML inclut toutes les informations de la transaction comptable, comme la date de validation du document, le type et le numéro du document, le type et le numéro de compte, le montant en crédit et en débit extraits de la page **Feuille comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="9f27c-106">The XML file includes all the general ledger transaction information, such as document posting date, document type, document number, account type, account number, credit amount, and debit amount retrieved from the **General Journal** page.</span></span>  

## <a name="to-export-general-ledger-entries-to-an-xml-file"></a><span data-ttu-id="9f27c-107">Pour exporter des écritures comptables vers un fichier XML</span><span class="sxs-lookup"><span data-stu-id="9f27c-107">To export general ledger entries to an XML file</span></span>  

1.  <span data-ttu-id="9f27c-108">Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Exporter écritures comptables vers un fichier XML**, puis choisissez le lien approprié.</span><span class="sxs-lookup"><span data-stu-id="9f27c-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Export G/L Entries to XML**, and then choose the relevant link.</span></span>  
2.  <span data-ttu-id="9f27c-109">Sur la page **Exporter écritures comptables vers un fichier XML**, sur le raccourci **Options**, renseignez les champs comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="9f27c-109">On the **Export G/L Entries to XML** page, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="9f27c-110">Champ</span><span class="sxs-lookup"><span data-stu-id="9f27c-110">Field</span></span>|<span data-ttu-id="9f27c-111">Désignation</span><span class="sxs-lookup"><span data-stu-id="9f27c-111">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="9f27c-112">**Date début**</span><span class="sxs-lookup"><span data-stu-id="9f27c-112">**Starting Date**</span></span>|<span data-ttu-id="9f27c-113">Définit la date de début pour exporter les transactions financières.</span><span class="sxs-lookup"><span data-stu-id="9f27c-113">Sets the starting date to export the financial transactions.</span></span>|  
    |<span data-ttu-id="9f27c-114">**Date fin**</span><span class="sxs-lookup"><span data-stu-id="9f27c-114">**Ending Date**</span></span>|<span data-ttu-id="9f27c-115">Définit la date de fin pour exporter les transactions financières.</span><span class="sxs-lookup"><span data-stu-id="9f27c-115">Sets the ending date to export the financial transactions.</span></span>|  

3.  <span data-ttu-id="9f27c-116">Pour exporter le fichier, cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="9f27c-116">To export the file, choose the **OK** button.</span></span>  

<span data-ttu-id="9f27c-117">Vous pouvez enregistrer le fichier généré dans un emplacement spécifié, ou vous pouvez ouvrir le fichier.</span><span class="sxs-lookup"><span data-stu-id="9f27c-117">You can save the generated file to a specified location, or you can open the file.</span></span>  

> [!WARNING]  
>  <span data-ttu-id="9f27c-118">Si vous avez défini les dates de début et de fin pour inclure l'exercice comptable complet, le processus peut prendre quelques minutes.</span><span class="sxs-lookup"><span data-stu-id="9f27c-118">If you have set the start date and end date to include the entire fiscal year, the process can take several minutes.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9f27c-119">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9f27c-119">See Also</span></span>  
[<span data-ttu-id="9f27c-120">Imprimer des états de la comptabilité</span><span class="sxs-lookup"><span data-stu-id="9f27c-120">Print General Ledger Reports</span></span>](how-to-print-general-ledger-reports.md)
