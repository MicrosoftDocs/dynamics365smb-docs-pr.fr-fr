---
title: Configurer une société | Microsoft Docs
description: Le processus d’implémentation commence avec les éléments requis par la solution Business Central. Vous regroupez toutes ces informations dans des packages configuration.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 3eefa0fcb40b4e925ca653f223f2d97ed10f370e
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777240"
---
# <a name="set-up-company-configuration"></a>Configurer une société
Le processus d’implémentation commence avec le partenaire Microsoft. Le partenaire est responsable des réflexions sur les détails de la configuration et de la création d’un package qu’un client peut facilement appliquer. Avant de créer une nouvelle société, vous devez en planifier la méthode de configuration. Vous devez prendre en compte les données de configuration de base et les types de données requis par la solution [!INCLUDE[prod_short](includes/prod_short.md)]. Vous regroupez toutes ces informations dans des packages configuration.

RapidStart Services fournit également les outils que vous utiliserez pour migrer vos données héritées, telles que les clients et les fournisseurs.  

Il est recommandé de créer des packages configuration dont la plupart des tables de configuration sont déjà renseignées pour permettre aux clients de ne modifier que quelques paramètres après l’application du package. Par exemple, lorsque vous créez une société, les tables **Souches de n°** et **Ligne souche de n°** sont renseignées à l’aide d’un ensemble de souches de numéros et les numéros de début. Les champs **Souches de n°** correspondants des tables de configuration sont également renseignés automatiquement. Il n’est pas nécessaire d’entrer les souches de numéros et autres informations de configuration de base. Vous pouvez également modifier manuellement toutes les données par défaut utilisées avec RapidStart Services à l’aide de la feuille de configuration.  

Les packages configuration sont constitués sur la base d’une société préconfigurée. Après avoir configuré une société qui répond à vos besoins, vous pouvez créer un package configuration qui contient les données pertinentes de cette société. Vous pouvez ensuite les utiliser lorsque vous créez une société que vous voulez configurer de la même manière.  

Pour faciliter l’importation des données principales, par exemple les informations sur le fournisseur et le client, vous pouvez utiliser des modèles de configuration. Les modèles de configuration contiennent un ensemble de paramètres par défaut, qui sont automatiquement affectés aux enregistrements importés dans [!INCLUDE[prod_short](includes/prod_short.md)].

Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.

|**Pour**|**Voir**|  
|------------|-------------|  
|Planifier une configuration de la société en renseignant la feuille de configuration.|[Gérer la configuration de la société dans une feuille](admin-how-to-manage-company-configuration-in-a-worksheet.md)|  
|Créer un package configuration, personnaliser un package, affecter des tables à un package, vérifier ou modifier les données client existantes, créer la société et déplacer les données de test vers l’environnement de production.|[Préparer un package configuration](admin-how-to-prepare-a-configuration-package.md)| 

## <a name="see-also"></a>Voir aussi  
[Configuration d’une société avec RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Administration](admin-setup-and-administration.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]