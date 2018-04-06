---
title: "Procédure de paramétrage d'une simulation"
description: "Vous pouvez créer et valider des écritures de simulation dans la comptabilité sans affecter la comptabilité réelle."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 4c6ca1ef945118f4659bbe30db4d08367c5369bc
ms.contentlocale: fr-fr
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-simulation"></a>Paramétrer une simulation
Vous pouvez créer et valider des écritures de simulation dans la comptabilité sans affecter la comptabilité réelle.  

Avant de pouvoir commencer à utiliser la fonctionnalité de simulation, vous devez configurer un code source et une souche de numéros et ajouter ces informations à un modèle feuille comptabilité.  

## <a name="to-set-up-simulation"></a>Pour paramétrer une simulation  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Codes sources**, puis sélectionnez le lien connexe.  
2.  Dans la fenêtre **Codes sources**, créez un enregistrement et renseignez les champs.  

    > [!IMPORTANT]  
    >  Sélectionnez le champ **Simulation**.  

3.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), saisissez **Souches de n°**, puis sélectionnez le lien associé à la zone **Configuration**.  
4.  Dans la fenêtre **Souches de n°**, créez un enregistrement et renseignez les champs. Naviguez jusqu'au champ **N° début** pour paramétrer des informations supplémentaires pour la souche de numéros.  
5.  Sélectionnez les champs **N° par défaut** et **N° manuels**.  
6.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Modèles feuille comptabilité**, puis sélectionnez le lien connexe.  
7.  Dans la fenêtre **Modèles feuille comptabilité**, créez un enregistrement et renseignez les champs. Dans le champ **Type**, sélectionnez Général et spécifiez la nouvelle souche de numéros et le nouveau code source dans le champ **Souches de n°** et **Code source**.  

Vous pouvez désormais créer des écritures de simulation à l'aide de la feuille comptabilité.  

## <a name="see-also"></a>Voir aussi  
 [Créer des écritures de simulation](how-to-create-simulation-entries.md)   
 [Supprimer des écritures de simulation](how-to-delete-simulation-entries.md)   
 [Transférer des écritures de simulation](how-to-transfer-simulation-entries.md)

