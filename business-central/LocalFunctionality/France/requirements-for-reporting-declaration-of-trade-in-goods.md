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
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 73c627248b7dc878ca82dd1f19a4d2239485a0b6
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/01/2020
ms.locfileid: "3920102"
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


[!INCLUDE[footer-include](../../includes/footer-banner.md)]