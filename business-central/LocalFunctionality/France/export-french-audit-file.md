---
title: Exporter les écritures pour les audits fiscaux
description: Cet article explique comment préparer et exporter des fichiers d’audit pour se conformer à la réglementation fiscale spécifique en France.
author: altotovi
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.form: null
ms.date: 06/13/2023
ms.author: altotovi
---

# <a name="export-general-ledger-entries-for-tax-audits"></a>Exportation des écritures comptables pour les audits fiscaux

En France, les entreprises doivent fournir des informations relatives à l’impôt sur les sociétés et à la TVA, telles que les transactions et les écritures comptables, pour les audits. Les informations doivent être fournies dans un format de fichier spécifié par les autorités fiscales. Dans [!INCLUDE[prod_short](../../includes/prod_short.md)], ces informations sont enregistrées dans un fichier d’audit standard conçu pour fournir des informations sur les types de comptes qui incluent des entrées comptabilisées.

> [!NOTE]
> Il y a une nouvelle fonctionnalité dans la version 22.1. Pour utiliser cette fonctionnalité, exécutez la page **Document d’exportation des fichiers d’audit**. 

## <a name="export-the-audit-file"></a>Exporter le fichier d’audit

1. Sélectionnez l’icône ![Ampoule qui ouvre la fenêtre de recherche.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Document d’exportation des fichiers d’audit**, puis sélectionnez le lien associé.
2. Sélectionnez **Nouveau** pour créer un processus d’exportation. 
3. Dans le champ **Format d’exportation de fichiers d’audit**, sélectionnez **FEC** pour spécifier le format utilisé pour exporter le fichier d’audit.  
4. Dans le raccourci **FEC**, cochez le champ **Inclure les soldes d’ouverture** pour inclure les soldes d’ouverture dans le fichier de rapport d’audit. Les soldes sont calculés à partir de la date précédent la première date de la période couverte par l’état. 
5. Saisissez le **Code source par défaut** pour spécifier le code journal à utiliser si aucun code n’est spécifié dans l’écriture comptable. 
6. Entrez les informations dans les champs restants comme décrit dans l’article, [Comment exporter des fichiers d’audit](../../finance-how-to-export-audit-files.md).

## <a name="see-also"></a>Voir aussi

[Fonctionnalité locale en français](france-local-functionality.md)
[Comment utiliser l’application Exporter les fichiers d’audit](../../finance-how-to-export-audit-files.md)

[!INCLUDE[footer-include](../../includes/footer-banner.md)]