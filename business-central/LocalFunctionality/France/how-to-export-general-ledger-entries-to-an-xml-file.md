---
title: "Procédure d'exportation des écritures comptables vers un fichier XML"
description: "Pour l'archivage externe, et pour une période donnée, vous pouvez exporter des transactions financières vers un fichier XML."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 77de09a2906ceb827aa6c236852c4f875a6b1a25
ms.contentlocale: fr-fr
ms.lasthandoff: 03/22/2018

---
# <a name="export-general-ledger-entries-to-an-xml-file"></a>Exporter des écritures comptables vers un fichier XML
Pour l'archivage externe, et pour une période donnée, vous pouvez exporter des transactions financières vers un fichier XML. À la fin de l'exercice comptable, vous pouvez exporter les transactions comptables pour l'année clôturée en appliquant le filtre de date approprié et en exportant les transactions financières dans la période indiquée vers le fichier XML. Le fichier XML inclut toutes les informations de la transaction comptable, comme la date de validation du document, le type et le numéro du document, le type et le numéro de compte, les montants en crédit et en débit extraits de la fenêtre **Feuille comptabilité**.  

## <a name="to-export-general-ledger-entries-to-an-xml-file"></a>Pour exporter des écritures comptables vers un fichier XML  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Exporter écritures comptables vers un fichier XML**, puis choisissez le lien approprié.  
2.  Dans la fenêtre **Exporter écritures comptables vers un fichier XML**, sur le raccourci **Options**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Date début**|Définit la date de début pour exporter les transactions financières.|  
    |**Date fin**|Définit la date de fin pour exporter les transactions financières.|  

3.  Pour exporter le fichier, cliquez sur le bouton **OK**.  

Vous pouvez enregistrer le fichier généré dans un emplacement spécifié, ou vous pouvez ouvrir le fichier.  

> [!WARNING]  
>  Si vous avez défini les dates de début et de fin pour inclure l'exercice comptable complet, le processus peut prendre quelques minutes.  

## <a name="see-also"></a>Voir aussi  
[Imprimer des états de la comptabilité](how-to-print-general-ledger-reports.md)

