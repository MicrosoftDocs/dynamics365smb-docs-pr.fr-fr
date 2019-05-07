---
title: Procédure d'exportation des écritures comptables pour les audits fiscaux
description: Le fichier d'audit standard utilisé à des fins fiscales enregistre des informations commerciales clés (transactions et validations comptables) dans un fichier au format courant spécifié à des fins d'audit. En France, vous devez fournir au gouvernement ces informations dans un fichier d'audit standard à partir de janvier 2014. Cela s'applique aux sociétés pour les besoins d'audit de l'impôt sur les sociétés et de la TVA.
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
ms.openlocfilehash: 492f43297a622f955d0de63ac920e0d4111e1066
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2019
ms.locfileid: "922498"
---
# <a name="export-general-ledger-entries-for-tax-audits"></a>Exporter des écritures comptables pour les audits fiscaux
Le fichier d'audit standard utilisé à des fins fiscales enregistre des informations commerciales clés (transactions et validations comptables) dans un fichier au format courant spécifié à des fins d'audit. En France, vous devez fournir au gouvernement ces informations dans un fichier d'audit standard à partir de janvier 2014. Cela s'applique aux sociétés pour les besoins d'audit de l'impôt sur les sociétés et de la TVA.  

En général, l'état est conçu pour fournir des informations sur les types de compte contenant des écritures validées.  

Vous pouvez choisir d'inclure les soldes d'ouverture dans le fichier, mais ce ne sont pas les écritures réelles qui sont validées dans [!INCLUDE[d365fin](../../includes/d365fin_md.md)]. Le système calcule le solde d'ouverture à l'aide des écritures d'un compte donné jusqu'à la date de début spécifiée pour le fichier. Les écritures de clôture générées par le processus de clôture de l'exercice précédent sont également incluses dans le calcul. Les soldes d'ouverture sont ensuite mappés dans les champs requis de l'état.  

Si vous ne fermez pas votre exercice comptable ou n'exécutez pas l'action **Clôturer exercice** avant de générer l'état, les comptes de gestion présentent toujours des soldes, qui sont déclarés dans le fichier.  

> [!NOTE]  
>  Les soldes d'ouverture sont uniquement inclus dans l'état pour les comptes présentant un solde différent de zéro. Vous pouvez identifier les soldes d'ouverture à l'aide des valeurs suivantes des champs :  
>   
>  -   JournalCode = 0  
> -   JournalLib = BALANCE OUVERTURE  
> -   EcritureNum = 0  
> -   EcritureLib = Comptes commençant par le préfixe BAL OUV  
> -   ValidDate = Date de début spécifiée sur la page de demande de l'état  

## <a name="to-export-general-ledger-entries-to-a-text-file-for-a-tax-audit"></a>Pour exporter des écritures comptables ver un fichier texte pour un audit fiscal  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Exporter écritures comptables - Audit fiscal**, puis sélectionnez le lien approprié.  
2.  Sur la page **Exporter écritures comptables - Audit fiscal**, sur le raccourci **Options**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Date début**|Entrez la date à utiliser comme date de début de la période couverte par l'audit.|  
    |**Date fin**|Entrez la date à utiliser comme date de fin de la période couverte par l'audit.|  
    |**Inclure soldes d'ouverture**|Indiquez si vous souhaitez inclure les soldes d'ouverture dans le fichier d'audit. Les soldes sont calculés à partir de la date précédent la première date de la période couverte par l'état.|  

3.  Cliquez sur le bouton **OK** pour exporter le fichier.  

Lorsque vous créez l'état, [!INCLUDE[d365fin](../../includes/d365fin_md.md)] trie les informations de l'état en fonction des champs **N°** et **Date création** de l'historique des transactions comptables.  

L'état aura le nom suivant : <taxpayername>FEC<YYYYMMDD>  

## <a name="see-also"></a>Voir aussi  
 [Clôturer fiscalement des exercices](how-to-close-years.md)
