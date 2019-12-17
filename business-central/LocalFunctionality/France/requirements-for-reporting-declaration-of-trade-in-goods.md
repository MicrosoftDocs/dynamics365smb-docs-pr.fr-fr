---
title: Configuration requise pour la déclaration d'échanges de biens
description: Cette rubrique présente la liste des champs requis pour la déclaration d'échanges de biens (DEB) au format DTI+.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 76de2a8a78a331471acd4f51105086e8c04df610
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/03/2019
ms.locfileid: "2878188"
---
# <a name="requirements-for-reporting-declaration-of-trade-in-goods"></a>Configuration requise pour la déclaration d'échanges de biens
Cette rubrique présente la liste des champs requis pour la déclaration d'échanges de biens (DEB) au format DTI+. Pour plus d'informations, voir Exporter DEB DTI.  

Les champs suivants sont requis pour la déclaration d'échanges de biens :  

- **CISD** dans la table **Informations société**.  
- **N° SIRET** dans la table **Informations société**.  
- **N° identif. intracomm.** dans la table **Informations société**.  
- **Nom** dans la table **Informations société**.  
- **Date** de la période statistique dans la table **Ligne feuille intracomm**.  
- **Régime** dans la table **Ligne feuille intracomm**.  
- La **Quantité** dans la table **Ligne feuille intracomm** doit être supérieure à 0.  
- La **Valeur statistique** dans la table **Ligne feuille intracomm** doit être supérieure à 0.  

> [!NOTE]  
>  L'état **Exporter DEB DTI** exporte les expéditions et les réceptions dans un lot. Si vous souhaitez déclarer uniquement les expéditions ou les réceptions, vous devez définir un filtre pour supprimer les lignes qui ne sont pas nécessaires dans la table **Feuille intracomm**.  

## <a name="see-also"></a>Voir aussi  
[Fonctionnalité locale, France](france-local-functionality.md)
