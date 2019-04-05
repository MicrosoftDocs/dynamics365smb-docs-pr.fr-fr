---
title: Procédure de calcul de l'amortissement accéléré
description: Dans Business Central, vous calculez l'amortissement périodique des immobilisations à l'aide du traitement par lots Calculer amortissement. La loi d'amortissement liée à l'immobilisation définit la méthode d'amortissement, la date de début de l'amortissement et le groupe comptabilisation immobilisation utilisé par le traitement par lots.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 462952864f99dee1dc732043e816ce796e5453e1
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2019
ms.locfileid: "826613"
---
# <a name="calculate-accelerated-depreciation"></a>Calculer l'amortissement accéléré
Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], vous calculez l'amortissement périodique des immobilisations à l'aide du traitement par lots **Calculer amortissement**. La loi d'amortissement liée à l'immobilisation définit la méthode d'amortissement, la date de début de l'amortissement et le groupe comptabilisation immobilisation utilisé par le traitement par lots.  

Si une loi d'amortissement d'immobilisation est intégrée dans la comptabilité, elle est appelée *loi d'amortissement comptable*. Si une loi d'amortissement d'immobilisation n'est pas intégrée dans la comptabilité, elle est appelée *loi d'amortissement fiscal*.  

Vous ne pouvez calculer l'amortissement accéléré que pour les immobilisations ayant une loi d'amortissement comptable et une loi d'amortissement fiscal. Pour plus d'informations sur le paramétrage des lois d'amortissement fiscal et des lois d'amortissement comptable pour les immobilisations, voir [Paramétrer l'amortissement accéléré](how-to-set-up-accelerated-depreciation.md).  

Les écritures sont transférées vers la feuille immobilisation lorsque vous sélectionnez une loi d'amortissement comptable dans le traitement par lots. Les écritures sont transférées vers la feuille immobilisation lorsque vous sélectionnez la loi d'amortissement fiscal.  

## <a name="to-calculate-accelerated-depreciation"></a>Pour calculer l'amortissement accéléré  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Calculer amortissement**, puis sélectionnez le lien approprié.  
2.  Sur la page **Calculer amortissement**, sur le raccourci **Options**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Loi d'amortissement**|Code d'identification unique de la loi d'amortissement comptable.|  
    |**Date compta. immo.**|Spécifiez la date de fin pour le calcul de l'amortissement, s'il s'agit de la première écriture d'amortissement pour l'immobilisation. La date de début de l'amortissement définie sur la page **Lois d'amortissement immo.** est utilisée comme date de début pour le calcul de l'amortissement. Si vous avez déjà amorti l'immobilisation, la date validation immobilisation de la dernière écriture d'amortissement est utilisée comme date de début pour le calcul de l'amortissement.|  
    |**Utiliser forcer nombre de jours**|Permet d'utiliser le nombre de jours dans le champ **Forcer nombre de jours** pour le calcul de l'amortissement.|  
    |**Forcer nombre de jours**|Nombre de jours pour le calcul de l'amortissement. Vous ne pouvez entrer un nombre dans ce champ que si la case **Utiliser forcer nombre de jours** est cochée.|  
    |**Date de validation**|Date de validation de l'amortissement calculé.<br /><br /> Vous pouvez laisser ce champ vide si le champ **Mêmes dates compta./immo.** dans la loi d'amortissement comptable est sélectionné. La date comptabilisation est copiée sur les lignes feuille.|  
    |**Numéro de document**|Numéro de document de la feuille immobilisation. Ne saisissez rien dans ce champ si vous avez défini des souches de numéros pour la feuille immobilisation sur la page **Souches de n°**. Pour plus d'informations, voir Souches de n°.|  
    |**Libellé écriture**|Libellé écriture pour les écritures feuille immobilisation.|  
    |**Insérer compte contrepartie**|Permet d'insérer automatiquement des comptes contrepartie dans la feuille résultante. Le traitement par lots **Calculer amortissement** utilise uniquement les comptes contrepartie définis dans le groupe comptabilisation immobilisation.|  

3.  Sur le raccourci **Immobilisation**, sélectionnez les filtres appropriés.  
4.  Cliquez sur le bouton **OK**.  

L'amortissement accéléré de l'immobilisation est calculé.  

## <a name="see-also"></a>Voir aussi  
 [Amortissement accéléré](accelerated-depreciation.md)   
 [Paramétrer l'amortissement accéléré](how-to-set-up-accelerated-depreciation.md)   
 [Configurer un amortissement immobilisation](../../fa-how-setup-depreciation.md)  
 [COMPTES D'IMMOBILISATIONS](../../fa-manage.md)
