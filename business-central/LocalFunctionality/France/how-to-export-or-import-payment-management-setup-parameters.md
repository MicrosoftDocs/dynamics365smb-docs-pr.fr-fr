---
title: Procédure d'exportation ou d'importation des paramètres de configuration de la gestion des paiements
description: Vous pouvez exporter ou importer les paramètres de configuration de la gestion des paiements vers un disque externe afin de pouvoir utiliser les mêmes paramètres pour une autre société présentant les mêmes exigences.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 62074e92cf1bc5373c88c3c01a8c68f6cd6876a1
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2019
ms.locfileid: "826621"
---
# <a name="export-or-import-payment-management-setup-parameters"></a>Exporter ou importer les paramètres de configuration de la gestion des paiements
Vous pouvez exporter ou importer les paramètres de configuration de la gestion des paiements vers un disque externe afin de pouvoir utiliser les mêmes paramètres pour une autre société présentant les mêmes exigences.  

Vous pouvez utiliser les formats suivants pour exporter les paramètres de configuration de la gestion des paiements :  

- ETEBAC (XMLport 10860) – Permet de créer une remise de lettre de change.  
- Prélèvement (XMLport 10861) – Permet de créer un prélèvement de paiement client (débit direct).  
- Transfert (XMLport 10862) – Permet de créer un transfert de paiement fournisseur (transfert de crédit).  

Vous pouvez sélectionner ces formats lorsque vous configurez le statut de règlement pour votre type de règlement. Pour plus d'informations, voir [Paramétrer des types de règlement](how-to-set-up-payment-classes.md).  

## <a name="to-export-or-import-payment-management-setup-parameters"></a>Pour exporter ou importer les paramètres de configuration de la gestion des paiements  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Paramètres bordereau paiement**, puis sélectionnez le lien approprié.  
2.  Sur la page **Type règlement**, sélectionnez l'action **Exporter paramètres**.  

    Pour importer un paramètre, choisissez l'action **Importer paramètres**, sélectionnez le fichier, puis choisissez le bouton **Ouvrir**.  

3.  Choisissez le bouton **Enregistrer** pour ouvrir la page **Enregistrer sous** et accéder à l'emplacement où le fichier doit être enregistré.  
4.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Gestion des paiements](payment-management.md)   
 [Paramétrer des types de règlement](how-to-set-up-payment-classes.md)   
 [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md)   
 [Paramétrer des étapes règlement](how-to-set-up-payment-steps.md)   
 [Configurer des adresses de paiement](how-to-set-up-payment-addresses.md)   
 [Créer bordereaux paiement](how-to-create-payment-slips.md)   
 [Archiver les bordereaux de paiement](how-to-archive-payment-slips.md)
