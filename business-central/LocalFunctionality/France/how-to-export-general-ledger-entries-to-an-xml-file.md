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
# <a name="export-general-ledger-entries-to-an-xml-file"></a>Exporter des écritures comptables vers un fichier XML
Pour l'archivage externe, et pour une période donnée, vous pouvez exporter des transactions financières vers un fichier XML. À la fin de l'exercice comptable, vous pouvez exporter les transactions comptables pour l'année clôturée en appliquant le filtre de date approprié et en exportant les transactions financières dans la période indiquée vers le fichier XML. Le fichier XML inclut toutes les informations de la transaction comptable, comme la date de validation du document, le type et le numéro du document, le type et le numéro de compte, le montant en crédit et en débit extraits de la page **Feuille comptabilité**.  

## <a name="to-export-general-ledger-entries-to-an-xml-file"></a>Pour exporter des écritures comptables vers un fichier XML  

1.  Choisissez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Exporter écritures comptables vers un fichier XML**, puis choisissez le lien approprié.  
2.  Sur la page **Exporter écritures comptables vers un fichier XML**, sur le raccourci **Options**, renseignez les champs comme indiqué dans le tableau suivant.  

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
