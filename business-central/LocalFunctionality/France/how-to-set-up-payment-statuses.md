---
title: Procédure de paramétrage des statuts règlement
description: Pour utiliser le module de gestion des paiements, vous devez paramétrer des statuts règlement pour définir les niveaux de progression des documents règlement. Vous devez définir un ensemble de statuts pour chaque type de règlement.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: a6f4201c2c8c3a9f5f72f0c46b6db57c9f440cf2
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/10/2020
ms.locfileid: "3676558"
---
# <a name="set-up-payment-statuses"></a>Paramétrer des statuts règlement
Pour utiliser le module de gestion des paiements, vous devez paramétrer des statuts règlement pour définir les niveaux de progression des documents règlement. Vous devez définir un ensemble de statuts pour chaque type de règlement. Pour plus d'informations, voir [Paramétrer des types de règlement](how-to-set-up-payment-classes.md).  

## <a name="to-set-up-payment-statuses"></a>Pour paramétrer des statuts règlement  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Paramètres bordereau paiement**, puis choisissez le lien associé.  
2.  Sélectionnez un type de règlement, puis cliquez sur **Statut**.  
3.  Sur la page **Statut règlement**, sélectionnez l'action **Nouveau**.  
4.  Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Nom**|Description du statut de règlement.|  
    |**RIB**|Permet d'indiquer que les informations relatives au Relevé d'Identité Bancaire (RIB) du client ou du fournisseur doivent être affichées dans les lignes paiement. Les informations du RIB incluent le code établissement, le code agence, le numéro de compte bancaire, le nom de la banque, la clé RIB et la clé de vérification.|  
    |**Consultation**|Permet d'indiquer que les lignes document de règlement qui ont atteint ce statut peuvent être modifiées et affichées sur la page **Afficher/Éditer ligne paiement**.<br /><br /> Pour plus d'informations, voir Afficher/Éditer ligne paiement.|  
    |**ReportMenu**|Permet d'indiquer que les documents de règlement qui ont atteint ce statut peuvent être imprimés.|  
    |**Montant**|Permet d'afficher le montant dans les lignes règlement.|  
    |**Paiement en cours**|Permet d'indiquer que toutes les lignes de facturation et paiement ayant ce statut doivent être prises en compte lors du calcul des paiements en cours.|  
    |**Archivage autorisé**|Permet d'indiquer que les bordereaux avec ce statut peuvent être archivés.|  

5.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Gestion des paiements](payment-management.md)   
 [Paramétrer des types de règlement](how-to-set-up-payment-classes.md)   
 [Paramétrer des étapes règlement](how-to-set-up-payment-steps.md)   
 [Configurer des adresses de paiement](how-to-set-up-payment-addresses.md)   
 [Créer bordereaux paiement](how-to-create-payment-slips.md)   
 [Valider des bordereaux paiement](how-to-post-payment-slips.md)   
 [Archiver les bordereaux de paiement](how-to-archive-payment-slips.md)   
 [Exporter ou importer les paramètres de configuration de la gestion des paiements](how-to-export-or-import-payment-management-setup-parameters.md)
