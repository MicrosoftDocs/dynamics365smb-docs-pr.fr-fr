---
title: Gestion des paiements [FR]
description: Vous pouvez gérer des lettres de change, des paiements électroniques et des paiements fournisseur à l’aide de la fonction de gestion des paiements dans la version française de Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/07/2021
ms.author: edupont
ms.openlocfilehash: a182b7e1327f70b2585c59e08e28ced2e9a2e491
ms.sourcegitcommit: 2b05661d7e09487398da2e55e30ebbd9173e3298
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/08/2021
ms.locfileid: "6434568"
---
# <a name="payment-management-in-the-french-version"></a>Gestion des paiements dans la version française

[!INCLUDE[prod_short](../../includes/prod_short.md)] vous permet de gérer des lettres de change, des paiements électroniques et des paiements fournisseur à l’aide de la fonction de gestion des paiements.  

Vous pouvez gérer les paiements fournisseur et client à l’aide des bordereaux paiement. Avant de créer un bordereau paiement, vous devez définir les paramétrages suivants :  

- Type de règlement – Type de règlement que vous souhaitez effectuer, comme par exemple, une lettre de change, un paiement électronique ou un chèque. Pour plus d’informations, voir [Paramétrer des types de règlement](how-to-set-up-payment-classes.md).  

- Statut règlement – Niveau de progression d’un document règlement. Vous devez définir un ensemble de statuts pour chaque type de règlement. Pour plus d’informations, consultez [Pour paramétrer les statuts de paiement pour une classe de paiement](how-to-set-up-payment-classes.md#to-set-up-payment-statuses-for-a-payment-class).  

- Étapes de règlement – Paiement qui est exécuté à un moment spécifié. Une fois l’étape de règlement exécutée, vous pouvez passer d’un statut du document règlement à un autre. Si une étape nécessite la validation d’enregistrements débiteurs ou créditeurs, vous devez définir d’autres actions dans la table **Etape règlement : Comptabilisation**. Pour plus d’informations, consultez [Pour paramétrer les étapes de paiement pour une classe de paiement](how-to-set-up-payment-classes.md#to-set-up-payment-steps-for-a-payment-class).  

- Adresse de règlement pour les fournisseurs et les clients – Adresse qui est utilisée pour un fournisseur ou un client au moment du règlement. L’adresse de règlement peut être différente de celle par défaut du client ou du fournisseur. Pour plus d’informations, voir [Paramétrer des adresses de règlement](how-to-set-up-payment-addresses.md).  

Vous pouvez également transférer vos informations de configuration de la gestion des paiements vers un disque externe afin de pouvoir utiliser les mêmes paramètres pour une autre société présentant les mêmes exigences.  

## <a name="managing-payment-slips-and-files"></a>Gestion des bordereaux et des fichiers paiement

Vous pouvez créer des bordereaux paiement pour gérer les paiements client et fournisseur. Après avoir créé le bordereau paiement, vous devez le valider.  

Ces bordereaux paiement peuvent être convertis en fichiers de paiement, qui peuvent être envoyés à la banque par voie électronique.  

Pour plus d’informations, consultez [Créer des bordereaux paiement](how-to-create-payment-slips.md).  

## <a name="archiving-payment-slips"></a>Archivage des bordereaux paiement

Vous pouvez séparer un bordereau paiement entièrement traité des bordereaux paiement actifs en l’archivant. Vous pouvez archiver un bordereau paiement manuellement ou vous pouvez archiver un lot de bordereaux automatiquement. Pour plus d’informations, consultez [Archiver des bordereaux paiement](how-to-archive-payment-slips.md).  

## <a name="see-also"></a>Voir aussi

[Paramétrer des types de règlement](how-to-set-up-payment-classes.md)  
[Configurer des adresses de paiement](how-to-set-up-payment-addresses.md)  
[Créer bordereaux paiement](how-to-create-payment-slips.md)  
[Valider des bordereaux paiement](how-to-post-payment-slips.md)  
[Archiver les bordereaux de paiement](how-to-archive-payment-slips.md)  
[Exporter ou importer les paramètres de configuration de la gestion des paiements](how-to-export-or-import-payment-management-setup-parameters.md)  
[Fonctionnalité locale, France](france-local-functionality.md)  
[Effectuer des paiements](../../payables-make-payments.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]