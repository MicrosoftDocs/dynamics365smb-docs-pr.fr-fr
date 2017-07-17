---
title: Gestion des comptes client| Microsoft Docs
description: Gestion des comptes client
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customer payment, debtor, balance due, AR
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 62d59546331a5faa5ecb7aea0f9bb8dedea719f9
ms.contentlocale: fr-fr
ms.lasthandoff: 05/04/2017


---
# <a name="managing-receivables"></a>Gestion des comptes client
Une étape normale de n'importe quelle opération financière consiste à rapprocher des comptes bancaires, ce qui nécessite de lettrer les paiements avec des écritures fournisseur ou client pour clôturer les factures vente et les avoirs achat.  

Dans [!INCLUDE[d365fin](includes/d365fin_md.md)], l'une des méthodes les plus rapides pour enregistrer les paiements à partir de la fenêtre **Feuille rapprochement bancaire** consiste à importer un fichier ou un flux de relevé bancaire. Les paiements sont lettrés pour ouvrir des écritures client ou fournisseur selon les correspondances entre le texte de paiement et les informations d'écriture. Vous pouvez consulter et modifier les correspondances avant de valider la feuille, puis clôturer les écritures comptables banque pour les écritures comptables lorsque vous validez la feuille. Le compte bancaire est rapproché lorsque tous les paiements sont lettrés.

Il existe, cependant, d'autres emplacements pratiques pour lettrer les paiements et pour rapprocher des comptes bancaires :  

* La fenêtre **Rapprochements bancaires**, qui vous permet également de vérifier des écritures comptables. Pour plus d'informations, reportez vous à [Procédure : rapprocher des comptes bancaires séparément](bank-how-reconcile-bank-accounts-separately.md).  
* La fenêtre **Enregistrement de paiement** qui vous permet d'appliquer et de vérifier manuellement les paiements reçus en liquide, par chèque ou par transaction bancaire par rapport à une liste générée de documents vente échus. Notez que cette fonctionnalité est uniquement disponible pour les documents vente.  
* La fenêtre **Feuille règlement** où vous pouvez valider manuellement les réceptions dans un compte général, client ou autre en saisissant une ligne règlement. Vous pouvez soit lettrer la réception ou le remboursement avec une ou plusieurs écritures ouvertes avant de valider la feuille règlement, ou à partir des écritures comptables client.  

Une autre tâche de gestion des comptes client consiste à collecter des soldes restants, notamment pour gérer les intérêts de retard et l'émission de relances. [!INCLUDE[d365fin](includes/d365fin_md.md)] offre d'autres méthodes pour effectuer ces opérations. Pour plus d'informations, voir [Procédure : collecte des soldes restants](receivables-collect-outstanding-balances.md).  

Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.  

| Pour | Voir |
| --- | --- |
| Lettrer des paiements aux écritures comptables client ou fournisseur ouvertes sur la base d'un fichier ou flux de relevé bancaire importé, et rapprocher le compte bancaire lorsque tous les paiements sont lettrés. |[Procédure : lettrage automatique des paiements et rapprochement des comptes bancaires](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| Lettrer les paiements aux écritures comptables client ouvertes selon la saisie manuelle dans la liste des documents vente échus. |[Procédure : rapprocher les paiements client manuellement à partir de la liste des documents vente échus](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md) |
| Valider les règlements ou les remboursements pour les clients dans la feuille règlement et lettrer aux écritures comptables client, à partir de la feuille ou des écritures comptables validées. |[Procédure : rapprocher les paiements client manuellement](receivables-how-apply-sales-transactions-manually.md) |
| Rappeler aux clients les soldes échus, calculer les intérêts et les intérêts de retard, et gérer les comptes clients. |[Procédure : collecter des soldes restants](receivables-collect-outstanding-balances.md) |

## <a name="see-also"></a>Voir aussi
[Ventes](sales-manage-sales.md)  
[Gestion des comptes fournisseur](payables-manage-payables.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Fonctionnalités marché](ui-across-business-areas.md)
