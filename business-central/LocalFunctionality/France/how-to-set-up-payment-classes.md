---
title: "Procédure de paramétrage des types de règlement"
description: "Pour utiliser le module Gestion des paiements, vous devez paramétrer des types de règlement pour définir des types d'opération, tels que des lettres de change, des paiements électroniques ou des chèques."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 5ce479e420aa84ae66386959cc2f170c6d080081
ms.contentlocale: fr-fr
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-payment-classes"></a>Paramétrer des types de règlement
Pour utiliser le module Gestion des paiements, vous devez paramétrer des types de règlement pour définir des types d'opération, tels que des lettres de change, des paiements électroniques ou des chèques.  

## <a name="to-set-up-a-payment-class"></a>Pour paramétrer un type de règlement  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Paramètres bordereau paiement**, puis sélectionnez le lien approprié.  
2.  Dans la fenêtre **Type règlement**, sélectionnez l'action **Nouveau**.  
3.  Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Activer**|Permet d'activer l'utilisation du type de règlement.|  
    |**Code**|Code d'identification unique du type de règlement.|  
    |**Nom**|Description du type de règlement.|  
    |**N° de souche en-tête**|Code souche de numéros pour l'en-tête du bordereau paiement.|  
    |**N° de souche lignes**|Code souche de numéros pour les lignes du bordereau paiement. Si vous laissez ce champ vide, le numéro de chaque ligne paiement est créé en se basant sur le numéro d'en-tête du bordereau paiement.|  
    |**Propositions**|Type de proposition de règlement qui peut être créé automatiquement sur un bordereau paiement.|  
    |**Contrepassation de TVA sur encaissement**|Spécifiez la méthode pour gérer la TVA sur encaissement.<br /><br /> Si vous sélectionnez **Lettrage**, la TVA sera réalisée lors de la validation du lettrage de la facture et du paiement.<br /><br /> Si vous sélectionnez **En retard**, vous devez définir l'étape de règlement au cours de laquelle la TVA doit être réalisée, en sélectionnant le champ **Réaliser TVA** dans la fenêtre **Fiche étape règlement**. Pour plus d'informations, voir Réaliser TVA et Étape règlement.|  
    |**Type transfert SEPA**|Spécifiez le format d'exportation SEPA, **Virement** ou **Prélèvement**.|  

4.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Gestion des paiements](payment-management.md)   
 [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md)   
 [Paramétrer des étapes règlement](how-to-set-up-payment-steps.md)   
 [Configurer des adresses de paiement](how-to-set-up-payment-addresses.md)   
 [Exporter ou importer les paramètres de configuration de la gestion des paiements](how-to-export-or-import-payment-management-setup-parameters.md)   
 [Créer bordereaux paiement](how-to-create-payment-slips.md)   
 [Valider des bordereaux paiement](how-to-post-payment-slips.md)   
 [Archiver les bordereaux de paiement](how-to-archive-payment-slips.md)

