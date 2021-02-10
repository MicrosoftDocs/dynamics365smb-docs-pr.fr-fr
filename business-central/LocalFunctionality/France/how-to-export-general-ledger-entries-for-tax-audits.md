---
title: Procédure d'exportation des écritures comptables pour les audits fiscaux
description: Cette rubrique explique comment préparer des fichiers d'audit pour se conformer à la réglementation fiscale en France.
author: sorenfriisalexandersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: ac8f85be155a93b74f6efcb72d3d309d19800837
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/17/2020
ms.locfileid: "4752427"
---
# <a name="export-general-ledger-entries-for-tax-audits"></a>Exporter des écritures comptables pour les audits fiscaux
En France, les entreprises doivent fournir des informations relatives à l'impôt sur les sociétés et à la TVA, telles que les transactions et les écritures comptables, pour les audits dans un format de fichier spécifié par les autorités fiscales. Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], ces informations sont enregistrées dans un fichier d’audit standard conçu pour fournir des informations sur les types de comptes qui incluent des entrées comptabilisées.

Vous pouvez inclure des soldes d'ouverture dans le fichier, mais il ne s'agit pas d'entrées comptabilisées réelles. [!INCLUDE[prod_short](../../includes/prod_short.md)] calcule le solde d'ouverture en utilisant des entrées de compte jusqu'à la date de début que vous spécifiez pour le fichier. Le calcul inclut également les écritures de clôture générées par la clôture de l’exercice précédent. Les soldes d'ouverture sont ensuite mappés aux champs obligatoires de l'état.  

Si vous ne fermez pas votre exercice comptable ou n'exécutez pas l'action **Clôturer exercice** avant de générer l'état, le fichier inclura les soldes des comptes de gestion.  

> [!NOTE]  
>  Les soldes d'ouverture sont inclus dans l'état uniquement pour les comptes présentant un solde différent de zéro. Pour identifier les soldes d'ouverture, regardez les valeurs suivantes dans les champs ci-dessous :  
>   
>  -  JournalCode = 0  
> -   JournalLib = BALANCE OUVERTURE  
> -   EcritureNum = 0  
> -   EcritureLib = Comptes commençant par le préfixe BAL OUV  
> -   ValidDate = Date de début spécifiée sur la page de demande de l'état  

> [!NOTE]  
>  Avant d'exporter des écritures comptables, assurez-vous que vous avez marqué les comptes généraux à détailler lors de l'exportation des soldes d'ouverture. C’est généralement une exigence pour les comptes généraux de banque, de client et de fournisseur. L'opération s'effectue en cochant la case dans le champ **Solde détaillé** sur la page **Carte de compte général**.
>   

## <a name="to-export-general-ledger-entries-to-a-text-file-for-a-tax-audit"></a>Pour exporter des écritures comptables ver un fichier texte pour un audit fiscal  
1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Exporter écritures comptables - Audit fiscal**, puis choisissez le lien approprié.  
2.  Sur la page **Exporter écritures comptables - Audit fiscal**, sur le raccourci **Options**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Date début**|Entrez la date à utiliser comme date de début de la période couverte par l'audit.|  
    |**Date fin**|Entrez la date à utiliser comme date de fin de la période couverte par l'audit.|  
    |**Inclure soldes d'ouverture**|Indiquez si vous souhaitez inclure les soldes d'ouverture dans le fichier d'audit. Les soldes sont calculés à partir de la date précédent la première date de la période couverte par l'état.|  

3.  Cliquez sur le bouton **OK** pour exporter le fichier.  

Lorsque vous créez l'état, [!INCLUDE[prod_short](../../includes/prod_short.md)] trie les informations de l'état en fonction des champs **N°** et **Date création** de l'historique des transactions comptables.  

L'état aura le nom suivant : <taxpayername>FEC<YYYYMMDD>  

## <a name="see-also"></a>Voir aussi  
 [Clôturer fiscalement des exercices](how-to-close-years.md)
