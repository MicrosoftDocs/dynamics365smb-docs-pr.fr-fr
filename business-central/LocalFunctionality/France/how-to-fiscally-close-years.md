---
title: Procédure de clôture fiscale des exercices
description: Lorsqu'un exercice comptable est terminé, vous devez clôturer fiscalement les périodes qui le composent pour veiller à ce qu'aucune autre écriture comptable ne puisse être validée.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: d2d9b4b032aa3dc9bc98162a18b08b5bd3d9838e
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/03/2019
ms.locfileid: "2878930"
---
# <a name="fiscally-close-years"></a>Clôturer fiscalement des exercices
Lorsqu'un exercice comptable est terminé, vous devez clôturer fiscalement les périodes qui le composent pour veiller à ce qu'aucune autre écriture comptable ne puisse être validée.  

Avant que la clôture fiscale ne soit autorisée, vous devez vérifier ce qui suit :  

- l'exercice comptable a été préalablement clôturé ; Pour plus d'informations, voir [Clôture des exercices](how-to-close-years.md).  
- toutes les lignes feuille non validées pour l'exercice sont validées ou supprimées avant la clôture fiscale de l'exercice ;
- toutes les écritures de clôture sont à jour.  

## <a name="to-fiscally-close-years"></a>Pour clôturer fiscalement des exercices  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Icône Page ou état pour la recherche"), entrez **Périodes comptables**, puis sélectionnez le lien approprié.  
2.  Sélectionnez la case à cocher **Clôturer l'exercice fiscalement**.  

    Si plusieurs exercices comptables ne sont pas clôturés fiscalement, le plus ancien doit être clôturé. Un message s'affiche pour identifier l'exercice à clôturer. Il détaille également les conséquences de cette opération.  

3.  Pour clôturer fiscalement l'exercice, cliquez sur le bouton **Oui**.  

Lorsque l'exercice comptable est clôturé fiscalement, le champ **Clôturé fiscalement** est sélectionné pour toutes les périodes de l'exercice. Vous ne pouvez plus rouvrir l'exercice clôturé fiscalement, ni désactiver le champ **Clôturé fiscalement**.  

## <a name="see-also"></a>Voir aussi  
 [Clôturer fiscalement des exercices](how-to-close-years.md)   
 [Vue d'ensemble des processus de fin d'exercice](year-end-processes-overview.md)   
 [Valider l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md)   
 [Clôture des exercices et des périodes](../../year-close-years-periods.md)
