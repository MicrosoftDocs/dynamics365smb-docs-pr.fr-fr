---
title: Définition de la présentation d’un état
description: Découvrez comment définir la présentation utilisée sur un état lors de la prévisualisation et de l’impression.
author: jswymer
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.search.form: 9652, 9650
ms.date: 03/07/2022
ms.author: jswymer
ms.openlocfilehash: 9cc827630c5acfeba2efc860d8baf67cd31bb404
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2022
ms.locfileid: "8525092"
---
# <a name="setting-the-layout-used-by-a-report"></a>Définition de la présentation utilisée par un état

> **S’APPLIQUE À :** Business Central Online, Business Central sur site (version 2022, vague de lancement 1 et ultérieures). Pour les versions antérieures, allez [ici](ui-how-change-layout-currently-used-report.md).

La présentation d’un état détermine l’apparence de ce dernier. Elle détermine les champs de données d’un jeu de données d’état qui s’affichent, leur organisation, leur style, etc. Un état peut être créé avec plus d’une présentation, que vous pouvez ensuite changer au besoin.

Lorsqu’il y a plusieurs sociétés dans l’application, les présentations sont définies pour chaque société. Ainsi, le même état dans une société peut avoir une présentation différente dans une autre société.

## <a name="get-started"></a>Démarrer

Il existe deux manières de définir la présentation utilisée par un état. Une façon consiste à aller sur la page **Sélection présentation état**. L’autre façon consiste à aller sur la page **Présentations d’état**. Chaque page a des avantages, par exemple : 

- La page **Sélection présentation état** affiche la liste de tous les états.

  Cette page indique la présentation actuelle d’un état. De plus, vous pouvez définir des présentations dans différentes sociétés, sans avoir à changer celle avec laquelle vous travaillez.

- La page **Présentations d’état** affiche toutes les présentations disponibles pour chaque état dans la société actuelle.

  Il est facile de trouver une présentation spécifique en triant ou en filtrant la liste. Une fois que vous avez trouvé la présentation, vous pouvez la définir pour un état avec une seule sélection.

  > [!NOTE]
  > Vous ne pouvez pas utiliser la page **Présentations d’état** pour les présentations Word et RDLC qui ont été créées à l’aide de la fonctionnalité **Présentations personnalisées** héritée. En fait, vous ne verrez même pas ces présentations personnalisées répertoriées sur la page **Présentations d’état**. Vous ne pouvez définir ces présentations qu’en utilisant la page **Sélection présentation état**.

## <a name="set-the-layout-from-the-report-layouts-page"></a>Définir la présentation à partir de la page Présentations d’état

[!INCLUDE[open-report-layouts-page](includes/open-report-layouts-page.md)]
2. Recherchez la présentation dans la liste, sélectionnez-la, puis sélectionnez l’action **Définir par défaut** en haut de la page.

## <a name="set-the-layout-from-report-layout-selection-page"></a>Définir la présentation à partir de la page Sélection présentation état

1. Sélectionnez l’icône en forme ![d’ampoule qui ouvre la fonction Tell Me 1.](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Sélection présentation état**, puis sélectionnez le lien associé.
  
   La page répertorie tous les états disponibles pour la société spécifiée dans le champ **Société** en haut de la page. Le champ **Description présentation** spécifie la présentation qui est actuellement utilisée sur l’état.
2. Définissez le champ **Société** en haut de la page sur la société qui inclut l’état.
3. Recherchez et sélectionnez l’état dans la liste, puis effectuez l’une des étapes suivantes :

   - Si la présentation vers laquelle vous souhaitez basculer est d’un type différent de la présentation actuelle, sélectionnez le champ **Type présentation**, puis choisissez le type de présentation que vous souhaitez définir sur l’état. 
   - Si la présentation vers laquelle vous souhaitez basculer a le même type que la présentation actuelle, sélectionnez l’action **Sélectionner présentation** en haut.

4. Dans la page **Présentations d’état**, sélectionnez une présentation, puis cliquez sur **OK**.

## <a name="revert-to-the-original-default-layout"></a>Revenir à la présentation par défaut d’origine

Les états sont conçus pour utiliser une présentation par défaut. Vous pouvez revenir à la présentation par défaut d’origine à partir de la page **Sélection présentation état**. Sélectionnez simplement l’état, puis sélectionnez l’action **Restaurer la sélection par défaut** en haut de la page.

## <a name="see-related-training-at-microsoft-learn"></a>Voir la formation associée sur [Microsoft Learn](/learn/modules/change-documents-dynamics-365-business-central/index)

## <a name="see-also"></a>Voir aussi

[Gestion des présentations d’état](ui-manage-report-layouts.md)  
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]