---
title: Périodes fiscales et exercices comptables
description: Un exercice comptable est généralement divisé en 12 périodes fiscales mensuelles. Dans Business Central, deux exercices comptables peuvent être ouverts en même temps.
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
ms.openlocfilehash: 9a5a9abad659ba7cbfd044d31e9c91c42f96d732
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/29/2019
ms.locfileid: "1237455"
---
# <a name="fiscal-periods-and-fiscal-years"></a>Périodes fiscales et exercices comptables
Un exercice comptable est généralement divisé en 12 périodes fiscales mensuelles. Dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)], deux exercices comptables peuvent être ouverts en même temps. Vous ne pouvez pas créer un troisième exercice comptable si deux exercices comptables sont ouverts.  

Pour clôturer un exercice comptable, vous devez clôturer les périodes comptables de cet exercice.  

Vous ne pouvez rouvrir une période comptable clôturée que si elle fait partie d'un exercice comptable ouvert. Pour plus d'informations, voir [Clôture des exercices](how-to-close-years.md). Vous ne pouvez pas rouvrir un exercice comptable clôturé.  

## <a name="closing-fiscal-periods-and-fiscal-years"></a>Clôture de périodes fiscales et d'exercices comptables  
À la fin d'un exercice comptable, vous devez clôturer les périodes comptables de cet exercice comptable. Cela garantit que des écritures comptables ne sont pas validées pour cette période. Pour plus d'informations, voir [Clôturer fiscalement des périodes comptables](how-to-fiscally-close-years.md).  

Un exercice comptable peut être clôturé si tous les critères suivants sont remplis :  

- Les dates comptabilisation sur la page **Paramètres utilisateur** et la page **Paramètres comptabilité** ne font pas partie de l'exercice que vous clôturez. Pour plus d'informations, voir Paramètres utilisateur et Paramètres comptabilité.  

- L'exercice comptable a été clôturé à l'aide de la fonction **Clôturer exercice** sur la page **Périodes comptables**. Pour plus d'informations, voir [Clôture des exercices et des périodes](../../year-close-years-periods.md).  

- Toutes les lignes feuille non validées pour l'exercice ont été validées ou supprimées.  

- Toutes les écritures de clôture sont à jour.  

Lorsque vous clôturez une période fiscale, la plus ancienne période fiscale ouverte est clôturée. Le champ **Début période validation** sur la page **Paramètres comptabilité** est mis à jour avec la date de début de la période ouverte suivante, si la date existante dans ce champ n'est pas déjà une date postérieure. Si le champ **Fin période validation** sur la page **Paramètres comptabilité** se situe dans la période clôturée, la valeur du champ **Fin période validation** est mise à jour avec la date de fin de la première période fiscale ouverte. Pour plus d'informations, voir Paramètres comptabilité.  

À la fin de l'exercice, vous devez effectuer les opérations suivantes :  

- clôturer l'exercice comptable à l'aide de la fonction **Clôturer exercice** ;  
- générer une écriture de clôture d'exercice ;  
- valider l'écriture de clôture d'exercice et compenser les écritures comptables de fonds propres ;  
- clôturer l'exercice comptable à l'aide de la fonction **Clôturer l'exercice fiscalement**.  

## <a name="see-also"></a>Voir aussi  
 [Valider l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md)   
 [Clôturer fiscalement des périodes comptables](how-to-fiscally-close-accounting-periods.md)   
 [Clôture des exercices et des périodes](../../year-close-years-periods.md)   
 [Valider l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md)   
 [Clôturer fiscalement des exercices](how-to-fiscally-close-years.md)   
 [Rouvrir des périodes comptables](how-to-reopen-accounting-periods.md)   
 [Clôturer les comptes de gestion](how-to-close-income-statement-accounts.md)   
 [Fonctionnalité locale, France](france-local-functionality.md)
