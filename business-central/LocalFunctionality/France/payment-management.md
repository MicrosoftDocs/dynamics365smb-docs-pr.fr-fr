---
title: Gestion des paiements
description: Vous pouvez gérer des lettres de change, des paiements électroniques et des paiements fournisseur à l'aide de la fonction de gestion des paiements.
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
ms.author: edupont
ms.openlocfilehash: e5818f654948969078482f26025c1269b17d7dd2
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778627"
---
# <a name="payment-management"></a>Gestion des paiements
[!INCLUDE[d365fin](../../includes/d365fin_md.md)] vous permet de gérer des lettres de change, des paiements électroniques et des paiements fournisseur à l'aide de la fonction de gestion des paiements.  

Vous pouvez gérer les paiements fournisseur et client à l'aide des bordereaux paiement. Avant de créer un bordereau paiement, vous devez définir les paramétrages suivants :  

- Type de règlement – Type de règlement que vous souhaitez effectuer, comme par exemple, une lettre de change, un paiement électronique ou un chèque. Pour plus d'informations, voir [Paramétrer des types de règlement](how-to-set-up-payment-classes.md).  

- Statut règlement – Niveau de progression d'un document règlement. Vous devez définir un ensemble de statuts pour chaque type de règlement. Pour plus d'informations, voir [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md).  

- Étapes de règlement – Paiement qui est exécuté à un moment spécifié. Une fois l'étape de règlement exécutée, vous pouvez passer d'un statut du document règlement à un autre. Si une étape nécessite la validation d'enregistrements débiteurs ou créditeurs, vous devez définir d'autres actions dans la table **Etape règlement : Comptabilisation**. Pour plus d'informations, voir [Paramétrer des étapes de règlement](how-to-set-up-payment-steps.md).  

- Adresse de règlement pour les fournisseurs et les clients – Adresse qui est utilisée pour un fournisseur ou un client au moment du règlement. L'adresse de règlement peut être différente de celle par défaut du client ou du fournisseur. Pour plus d'informations, voir [Paramétrer des adresses de règlement](how-to-set-up-payment-addresses.md).  

Vous pouvez également transférer vos informations de configuration de la gestion des paiements vers un disque externe afin de pouvoir utiliser les mêmes paramètres pour une autre société présentant les mêmes exigences. Vous pouvez exporter les données de paiement dans les formats suivants :  

- ETEBAC – Permet de créer une remise de lettre de change.  
- Prélèvement – Permet de créer un prélèvement de paiement client (débit direct).  
- Transfert – Permet de créer un transfert de paiement fournisseur (transfert de crédit).  

## <a name="managing-payment-slips-and-files"></a>Gestion des bordereaux et des fichiers paiement  
Vous pouvez créer des bordereaux paiement pour gérer les paiements client et fournisseur. Après avoir créé le bordereau paiement, vous devez le valider.  

Ces bordereaux paiement peuvent être convertis en fichiers de paiement, qui peuvent être envoyés à la banque par voie électronique.  

Pour plus d'informations, consultez [Créer des bordereaux paiement](how-to-create-payment-slips.md).  

## <a name="archiving-payment-slips"></a>Archivage des bordereaux paiement  
Vous pouvez séparer un bordereau paiement entièrement traité des bordereaux paiement actifs en l'archivant. Vous pouvez archiver un bordereau paiement manuellement ou vous pouvez archiver un lot de bordereaux automatiquement. Pour plus d'informations, consultez [Archiver des bordereaux paiement](how-to-archive-payment-slips.md).  

## <a name="see-also"></a>Voir aussi  
 [Paramétrer des types de règlement](how-to-set-up-payment-classes.md)   
 [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md)   
 [Paramétrer des étapes règlement](how-to-set-up-payment-steps.md)   
 [Configurer des adresses de paiement](how-to-set-up-payment-addresses.md)   
 [Créer bordereaux paiement](how-to-create-payment-slips.md)   
 [Valider des bordereaux paiement](how-to-post-payment-slips.md)   
 [Archiver les bordereaux de paiement](how-to-archive-payment-slips.md)   
 [Exporter ou importer les paramètres de configuration de la gestion des paiements](how-to-export-or-import-payment-management-setup-parameters.md)   
 [Fonctionnalité locale, France](france-local-functionality.md)
