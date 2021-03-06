---
title: Aperçu des tâches de ventilation des coûts et des revenus | Microsoft Docs
description: Décrit les tâches pour ventiler une écriture dans une feuille comptabilité dans différents comptes lorsque vous validez la feuille.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 8fec3a7c079058e73cda2b6f8940e3778b405bac
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775039"
---
# <a name="allocate-costs-and-income"></a>Répartition des coûts et du revenu
Vous pouvez ventiler une écriture dans une feuille comptabilité dans différents comptes lorsque vous validez la feuille. La ventilation peut être effectuée de trois manières différentes :

* Quantité
* Pourcentage (%)
* Montant

Les fonctions de ventilation peuvent être utilisées avec les feuilles abonnement et dans les feuilles immobilisation.
<!--You can also distribute the cost or revenue of a line to an intercompany partner when you post a sales or purchase document. When you post the document, a line will be posted in your general journal, and a corresponding line will be created in the intercompany outbox.-->

Les procédures suivantes décrivent comment se préparer à affecter des coûts dans une feuille abonnement en définissant des clés de ventilation. Lorsque des clés de ventilation sont définies, vous renseignez et validez la feuille comme toute autre feuille abonnement. Pour plus d’informations, voir [Utilisation des feuilles comptabilité](ui-work-general-journals.md).

## <a name="to-set-up-allocation-keys"></a>Pour définir des clés de ventilation
Vous pouvez ventiler une écriture dans une feuille abonnement dans différents comptes lorsque vous validez la feuille. La ventilation peut être effectuée par quantité, pourcentage ou montant.
1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuille abonnement**, puis sélectionnez le lien associé.
2. Sélectionnez le champ **Nom de la feuille** pour ouvrir la page **Noms feuilles comptabilité**.
3. Vous pouvez soit modifier les ventilations sur un lot existant dans la liste ou créer un lot avec des ventilations.
   * Pour créer un lot, sélectionnez l’action **Nouveau**, et passez à l’étape suivante.
   * Pour modifier les ventilations à partir d’une feuille existante, sélectionnez la feuille et passez à l’étape 7.    
4. Dans le champ **Nom**, saisissez le nom du lot, par exemple NETTOYAGE. Dans le champ **Description**, saisissez une description, par exemple Feuille frais de nettoyage.
5. Fermez la page lorsque vous avez terminé. Une nouvelle feuille récurrente vide s’ouvre.
6. Renseignez les champs de la ligne.
7. Sélectionnez l’action **Ventilations**.
8. Ajoutez une ligne pour chaque ventilation. Vous devez renseigner le champ **% ventilation**, **Quantité imputée** ou **Montant**. Vous devez également renseigner le champ **N° compte** et, si vous affectez la transaction à des axes principaux, les champs de ces axes principaux.
9. Si vous saisissez un pourcentage dans une ligne, le montant du champ **Montant** est calculé automatiquement. Ces montants sont dotés du signe opposé à celui du montant total figurant dans le champ **Montant** de la feuille récurrente.
10. Après avoir saisi les lignes de ventilation, cliquez sur **OK** pour revenir à la page **Feuille abonnement**. Le champ **Montant imputé DS** est renseigné et correspond au champ **Montant**.
11. Validez la feuille.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>Pour modifier une clé de ventilation déjà configurée
1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Feuille abonnement**, puis sélectionnez le lien associé.
2. Sur la page **Feuille récurrente**, sélectionnez la feuille contenant la ventilation.
3. Sélectionnez la ligne de la ventilation, puis sélectionnez l’action **Ventilations**.
4. Modifiez les champs appropriés, puis cliquez sur le bouton **OK**.

## <a name="see-also"></a>Voir aussi
[Clôture des exercices et des périodes](year-close-years-periods.md)  
[Utilisation de feuilles comptabilité](ui-work-general-journals.md)    
[Validation des documents et des feuilles](ui-post-documents-journals.md)    
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]