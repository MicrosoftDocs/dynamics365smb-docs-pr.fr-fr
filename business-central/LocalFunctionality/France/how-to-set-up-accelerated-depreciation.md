---
title: Paramétrer l’amortissement accéléré
description: 'Pour utiliser la fonction de calcul de l’amortissement accéléré, vous devez configurer les lois d’amortissement pour les immobilisations.'
author: edupont04
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.form: '5610, 5611'
ms.date: 02/14/2022
ms.author: edupont
---
# <a name="set-up-accelerated-depreciation" />Paramétrer l’amortissement accéléré

Pour utiliser la fonction de calcul de l’amortissement accéléré, vous devez configurer les lois d’amortissement suivantes pour les immobilisations :  

- la loi d’amortissement comptable (intégrée à la comptabilité) ;  
- la loi d’amortissement fiscal (non intégrée à la comptabilité).  

> [!NOTE]  
> Lorsque vous validez une acquisition, un amortissement ou une cession pour la loi d’amortissement comptable, la transaction est automatiquement dupliquée et validée dans la loi d’amortissement fiscal lorsque la feuille immobilisation est validée.  

L’écart entre la loi d’amortissement comptable et la loi d’amortissement fiscal est géré via les paramètres du raccourci **Intégration** sur la fiche loi d’amortissement comme indiqué dans le tableau suivant.  

|Objet de la loi d’amortissement  |Valeur du champ Dérogatoire  |
|---------|---------|
|Amortissement comptable  | Activé       |
|Amortissement fiscal     | Désactivé |

Le champ **Dérogatoire** indique si vous voulez que les écritures dérogatoires validées sur cette loi d’amortissement soient validées en comptabilité et sur les écritures comptables immobilisation. Si vous avez activé ce champ, vous devez utiliser la feuille comptabilisation immobilisation pour valider les écritures dérogatoires.

Vous spécifiez les comptes généraux qui doivent être utilisés sur la page **Fiche groupe compta. immo.**. Sur la page **Loi d’amortissement**, vous spécifiez le groupe comptabilisation qui doit être utilisé.

Si vous n’activez pas ce champ, vous devez utiliser la feuille immobilisation pour valider les écritures dérogatoires qui ne seront validées que dans la table Ecriture immobilisation.

Pour la loi d’amortissement fiscal, sur le raccourci **Général**, vous spécifiez ensuite la loi d’amortissement comptable pertinente dans le **Calcul dérogatoire** qui calculera l’amortissement dérogatoire. Le champ **Utilisé avec la loi dérogatoire** dans la loi d’amortissement comptable est mis à jour avec le code de la loi d’amortissement fiscal.  

## <a name="derogatory-calculation" />Calcul dérogatoire

Le champ **Calcul dérogatoire** d’une loi d’amortissement comptable spécifie si cette loi est utilisée comme loi d’amortissement fiscal pour le calcul de l’amortissement dérogatoire. Le code spécifié pour la loi d’amortissement comptable établit un paramétrage dérogatoire.

Étant donné que seules les écritures immobilisation sont validées dans la loi d’amortissement fiscal, les cases à cocher sous l’onglet **Intégration** ne peuvent pas être activées.

Lorsque le champ est vide, [!INCLUDE[prod_short](../../includes/prod_short.md)] utilise la loi d’amortissement de manière standard. S’il ne l’est pas, le système calcule l’amortissement dérogatoire.

## <a name="see-also" />Voir aussi

[Amortissement accéléré](accelerated-depreciation.md)  
[Calculer l'amortissement accéléré](how-to-calculate-accelerated-depreciation.md)  
[Configurer un amortissement immobilisation](../../fa-how-setup-depreciation.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
