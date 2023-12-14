---
title: Procédure d’exportation des écritures comptables vers un fichier XML
description: 'Pour l’archivage externe, et pour une période donnée, vous pouvez exporter des transactions financières vers un fichier XML.'
services: project-madeira
documentationcenter: ''
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 04/01/2021
ms.author: bholtorf
---
# <a name="export-general-ledger-entries-to-an-xml-file"></a>Exporter des écritures comptables vers un fichier XML
Pour l’archivage externe, et pour une période donnée, vous pouvez exporter des transactions financières vers un fichier XML. À la fin de l’exercice comptable, vous pouvez exporter les transactions comptables pour l’année clôturée en appliquant le filtre de date approprié et en exportant les transactions financières dans la période indiquée vers le fichier XML. Le fichier XML inclut toutes les informations de la transaction comptable, comme la date de validation du document, le type et le numéro du document, le type et le numéro de compte, le montant en crédit et en débit extraits de la page **Feuille comptabilité**.  

## <a name="to-export-general-ledger-entries-to-an-xml-file"></a>Pour exporter des écritures comptables vers un fichier XML

1.  Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Exporter écritures comptables au format XML**, puis choisissez le lien approprié.  
2.  Sur la page **Exporter écritures comptables vers un fichier XML**, sur le raccourci **Options**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Date début**|Définit la date de début pour exporter les transactions financières.|  
    |**Date fin**|Définit la date de fin pour exporter les transactions financières.|  

3.  Pour exporter le fichier, cliquez sur le bouton **OK**.  

Vous pouvez enregistrer le fichier généré dans un emplacement spécifié, ou vous pouvez ouvrir le fichier.  

> [!WARNING]  
>  Si vous avez défini les dates de début et de fin pour inclure l’exercice comptable complet, le processus peut prendre quelques minutes.  

## <a name="see-also"></a>Voir aussi
[Imprimer des états de la comptabilité](how-to-print-general-ledger-reports.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
