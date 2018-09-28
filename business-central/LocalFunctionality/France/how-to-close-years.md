---
title: "Procédure de clôture des exercices"
description: "Lorsqu'un exercice comptable est terminé, vous devez clôturer les périodes qui le composent."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 9c2bc3081b0c673db90f5a4c677b660f8118ca6c
ms.contentlocale: fr-fr
ms.lasthandoff: 03/22/2018

---
# <a name="close-years"></a>Clôturer fiscalement des exercices
Lorsqu'un exercice comptable est terminé, vous devez clôturer les périodes qui le composent.  

## <a name="to-close-a-year"></a>Pour clôturer un exercice  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Périodes comptables**, puis sélectionnez le lien approprié.  
2.  Choisissez l'action **Clôturer exercice**.  

    Si plusieurs exercices comptables sont ouverts, le plus ancien doit être clôturé. Un message s'affiche pour identifier l'exercice à clôturer. Il détaille également les conséquences de cette opération.  

3.  Pour clôturer l'exercice, cliquez sur **Oui**.  

Lorsque l'exercice comptable est clôturé, les champs **Fermé** et **Verrouillage date** sont sélectionnés pour toutes les périodes de l'exercice. À ce stade, vous ne pouvez pas rouvrir l'exercice comptable, ni désactiver les champs **Fermé** et **Verrouillage date**.  

> [!WARNING]  
> Vous ne pouvez pas clôturer un exercice comptable avant d'en créer un nouveau. Lorsqu'un exercice comptable est clôturé, vous ne pouvez pas modifier la date de début de l'exercice comptable suivant.  

Même si un exercice comptable a été clôturé, vous pouvez toujours y valider des écritures comptables jusqu'à ce que vous le clôturiez fiscalement. Dans ce cas, les écritures sont marquées comme validées dans un exercice comptable clôturé et le champ Ecr. exercice précédent est activé. Pour plus d'informations, voir [Clôturer fiscalement des exercices](how-to-fiscally-close-years.md).  

Une fois qu'un exercice comptable a été clôturé, vous devez clôturer les comptes de gestion et transférer les résultats de l'exercice sur un compte du bilan. Vous pouvez répéter cette opération pour chaque validation dans l'exercice comptable clôturé.  

Après avoir été clôturé fiscalement, un exercice comptable ne peut plus être rouvert et aucune écriture comptable ne peut y être validée.  

## <a name="see-also"></a>Voir aussi  
 [Clôturer fiscalement des exercices](how-to-fiscally-close-years.md)   
 [Vue d'ensemble des processus de fin d'exercice](year-end-processes-overview.md)   
 [Valider l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md)   
 [Clôture des exercices et des périodes](../../year-close-years-periods.md)

