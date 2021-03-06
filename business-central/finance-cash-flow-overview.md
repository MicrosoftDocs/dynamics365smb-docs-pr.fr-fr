---
title: Aperçu de trésorerie
description: Aperçu des encaissements et des décaissements pour aider à prévoir les montants à recevoir et à payer.
author: jill-kotel-andersson
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cash flow, money flow, expense and income, liquidity, cash receipts minus cash payments
ms.date: 06/08/2021
ms.author: a-jillk
ms.reviewer: edupont
ms.openlocfilehash: 8359d95b36d6c16b179de2fce400c44fd93ec0f1
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/09/2021
ms.locfileid: "6216359"
---
# <a name="cash-flow-overview"></a>Aperçu de trésorerie

La compréhension des encaissements et des décaissements est essentielle pour la gestion fructueuse d’une activité. La trésorerie vous permet de créer facilement des prévisions à court terme, qui prévoient les moyens et les délais de réception et de règlement au sein de votre société. Il est important de savoir que votre société aura suffisamment de fonds pour payer ses créditeurs et ses dépenses à échéance.

## <a name="definition-of-cash-flow"></a>Définition du terme Trésorerie

Le terme *Trésorerie* désigne les encaissements moins les espèces sur une période donnée. Il s’agit d’une estimation de fonds à encaisser et décaisser au sein de votre société. Tous les produits et toutes les dépenses prévus en font partie.

## <a name="cash-flow-overview"></a>Aperçu de trésorerie

La figure ci-après décrit comment utiliser la trésorerie.

![Aperçu de trésorerie](media/finance_cash_flow_overview.png "Aperçu de trésorerie")

- Vous paramétrez les prévisions de trésorerie.  

- Vous obtenez des sources de prévision de trésorerie à partir des sections suivantes :  

  - Comptabilité – Informations sur les fonds liquides, les revenus et les dépenses budgétés de la société.  
  - Achats - Informations sur les comptes fournisseur actuels et les dettes prévues à partir des commandes achat ouvertes.  
  - Ventes - Informations sur les comptes client actuels et les réceptions prévues à partir des commandes vente ouvertes.  
  - Service – Informations sur les commandes de service ouvertes.  
  - Immobilisations – Informations sur la cession planifiée et les achats budgétés d’immobilisations.  
  - Opérations diverses positives et négatives – Gestion des opérations diverses positives et négatives, et leur intégration dans les prévisions de trésorerie.  
- Si vous utilisez un traitement par lots pour transférer les informations des zones Comptabilité, Achats, Ventes, Service et Immobilisationsvers la feuille trésorerie, vous enregistrez des lignes de feuille d’activité pour effectuer une prévision de trésorerie.  
- Vous utilisez plusieurs fenêtres, états et graphiques pour analyser et imprimer des prévisions de trésorerie concernant des aperçus de disponibilité et de planning.  

## <a name="making-a-cash-flow-forecast"></a>Réalisation d’une prévision de trésorerie

En fonction des lignes de feuille d’activité enregistrées, vous pouvez effectuer périodiquement des prévisions de trésorerie. La présentation suivante est fréquemment utilisée pour des prévisions de trésorerie. La présentation est constituée de trois sections :

  - Règlements  
  - Décaissements  
  - Trésorerie nette ou encaisse  

Les règlements fournissent des détails sur les produits reçus par la société.

*règlements totaux* = *créances* + *commandes vente ouvertes* + *commandes service ouvertes* + *cessions d’immobilisations* + *opérations diverses positives* + *revenus budgétés*

> [!NOTE]
> Les opérations diverses positives sont des éléments, tels que les revenus de location, les intérêts d’actifs financiers ou le nouveau capital privé. Vous pouvez planifier des opérations diverses positives pour une certaine période et les utiliser dans le calcul des prévisions de trésorerie.

Les décaissements fournissent des détails de paiements effectués par la société.

*décaissements totaux* = *soldes dus* + *commandes achat ouvertes* + *investissement en immobilisations* + *opérations diverses négatives* + *dépenses budgétées*

> [!NOTE]
> Les opérations diverses négatives sont des éléments, tels que les salaires, les intérêts de crédit ou les consommations privées. Vous pouvez planifier des opérations diverses négatives pour une certaine période et les utiliser dans le calcul des prévisions de trésorerie.

La trésorerie nette ou l’encaisse est calculée comme suit : règlements totaux moins décaissements totaux à la fin de chaque période.

*trésorerie nette* = *règlements totaux* – *décaissements totaux* + *fonds liquides*

La prévision peut ensuite être utilisée comme un outil interne de décision en gestion pour préparer l’avenir et prendre des décisions stratégiques importantes pour la société.

## <a name="see-also"></a>Voir aussi
[Configuration d’une analyse de trésorerie](finance-setup-cash-flow-analyses.md)  
[Analyser les flux de trésorerie](finance-analyze-cash-flow.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
