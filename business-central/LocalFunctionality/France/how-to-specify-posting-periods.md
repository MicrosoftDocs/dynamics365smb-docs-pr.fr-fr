---
title: 'Procédure : définition des périodes de validation [FR]'
description: En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/18/2021
ms.author: edupont
ms.openlocfilehash: c3b3b4f88dbe8d14beb9a1891dc4c790c1fdf711
ms.sourcegitcommit: a7cb0be8eae6ece95f5259d7de7a48b385c9cfeb
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/08/2021
ms.locfileid: "6435895"
---
# <a name="specify-posting-periods-in-the-french-version"></a>Définir les périodes de validation dans la version française

En définissant des périodes de validation, vous limitez la période durant laquelle la validation est autorisée.  

## <a name="to-specify-posting-periods"></a>Pour définir des périodes de validation  

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Paramètres comptabilité**, puis choisissez le lien associé.  
2. Sur la page **Paramètres comptabilité**, dans le champ **Début période validation**, spécifiez la date de début de la période de validation.  
3. Dans le champ **Fin période validation**, spécifiez la date de fin de la période de validation.  

    Les dates sont validées dans les plages de validation autorisées pour garantir leur appartenance aux exercices comptables ouverts. Pour plus d’informations, voir Plage de validation autorisée.  

4. Pour vérifier quelle est la plage de validation autorisée, choisissez l’action **Extraire plage de validation autorisée**.  

Les dates définies ici s’appliquent à l’ensemble de la société, c’est-à-dire à tous les utilisateurs.  

> [!NOTE]  
> Vous pouvez définir différentes périodes de comptabilisation pour divers utilisateurs et appliquer une période de validation à un utilisateur sur la page **Paramètres utilisateur**.

Si vous entrez des dates ici, les dates entrées sur la page **Paramètres comptabilité** ne s’appliquent pas à ces utilisateurs.  

## <a name="see-also"></a>Voir aussi

[Périodes fiscales et exercices comptables](fiscal-periods-and-fiscal-years.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]