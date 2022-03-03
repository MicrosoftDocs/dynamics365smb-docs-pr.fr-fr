---
title: Périodes fiscales et exercices comptables (FR)
description: Un exercice comptable est généralement divisé en 12 périodes fiscales mensuelles. Dans la version française de Business Central, deux exercices peuvent être ouverts en même temps.
author: edupont04
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 174cab32c045adee14209c5176ac8e42a3398ece
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2022
ms.locfileid: "8132265"
---
# <a name="fiscal-periods-and-fiscal-years-in-the-french-version"></a>Périodes fiscales et années fiscales dans la version française

Un exercice comptable est généralement divisé en 12 périodes fiscales mensuelles. Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], deux exercices comptables peuvent être ouverts en même temps. Vous ne pouvez pas créer un troisième exercice comptable si deux exercices comptables sont ouverts.  

Pour clôturer un exercice comptable, vous devez clôturer les périodes comptables de cet exercice.  

Vous ne pouvez rouvrir une période comptable clôturée que si elle fait partie d’un exercice comptable ouvert. Pour plus d’informations, voir [Clôture des exercices](how-to-close-years.md). Vous ne pouvez pas rouvrir un exercice comptable clôturé.  

## <a name="closing-fiscal-periods-and-fiscal-years"></a>Clôture de périodes fiscales et d’exercices comptables

À la fin d’un exercice comptable, vous devez clôturer les périodes comptables de cet exercice comptable. Cela garantit que des écritures comptables ne sont pas validées pour cette période. Pour plus d’informations, voir [Clôturer fiscalement des périodes comptables](how-to-fiscally-close-years.md).  

Un exercice comptable peut être clôturé si tous les critères suivants sont remplis :  

- Les dates comptabilisation sur la page **Paramètres utilisateur** et la page **Paramètres comptabilité** ne font pas partie de l’exercice que vous clôturez. Pour plus d’informations, consultez [Définir des périodes de validation](../../finance-how-specify-posting-periods.md) et [Description des écritures comptables et du plan comptable](../../finance-general-ledger.md).  

- L’exercice comptable a été clôturé à l’aide de la fonction **Clôturer exercice** sur la page **Périodes comptables**. Pour plus d’informations, voir [Clôture des exercices et des périodes](../../year-close-years-periods.md).  

- Toutes les lignes feuille non validées pour l’exercice ont été validées ou supprimées.  

- Toutes les écritures de clôture sont à jour.  

Lorsque vous clôturez une période fiscale, la plus ancienne période fiscale ouverte est clôturée. Le champ **Début période validation** sur la page **Paramètres comptabilité** est mis à jour avec la date de début de la période ouverte suivante, si la date existante dans ce champ n’est pas déjà une date postérieure. Si le champ **Fin période validation** sur la page **Paramètres comptabilité** se situe dans la période clôturée, la valeur du champ **Fin période validation** est mise à jour avec la date de fin de la première période fiscale ouverte. Pour plus d’informations, voir [Description des écritures comptables et du plan comptable](../../finance-general-ledger.md).  

À la fin de l’exercice, vous devez effectuer les opérations suivantes :  

- clôturer l’exercice comptable à l’aide de la fonction **Clôturer exercice** ;  
- générer une écriture de clôture d’exercice ;  
- valider l’écriture de clôture d’exercice et compenser les écritures comptables de fonds propres ;  
- clôturer l’exercice comptable à l’aide de la fonction **Clôturer l’exercice fiscalement**.  

## <a name="see-also"></a>Voir aussi

[Valider l’écriture de clôture d’exercice](how-to-post-the-year-end-closing-entry.md)  
[Clôturer fiscalement des périodes comptables](how-to-fiscally-close-accounting-periods.md)  
[Clôture des exercices et des périodes](../../year-close-years-periods.md)  
[Valider l’écriture de clôture d’exercice](how-to-post-the-year-end-closing-entry.md)  
[Clôturer fiscalement des exercices](how-to-fiscally-close-years.md)  
[Rouvrir des périodes comptables](how-to-reopen-accounting-periods.md)  
[Clôturer les comptes de gestion](how-to-close-income-statement-accounts.md)  
[Définir des périodes de validation](../../finance-how-specify-posting-periods.md)  
[Description des écritures comptables et du plan comptable](../../finance-general-ledger.md)  
[Fonctionnalité locale, France](france-local-functionality.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]