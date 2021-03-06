---
title: Utilisation des documents entrants| Microsoft Docs
description: Vous pouvez gérer les documents commerciaux externes entrants, tels que des reçus de paiement ou des fichiers PDF, gérer des tâches OCR, et convertir des fichiers en documents électroniques et enregistrements.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 8e02cd4627219c7ea439155b2b91b61e03534dc2
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788482"
---
# <a name="incoming-documents"></a>Documents entrants

Certaines transactions d’entreprise ne sont pas enregistrées dans [!INCLUDE[prod_short](includes/prod_short.md)] dès le départ. À la place, un document provenant d’entreprise externe arrive dans votre société comme la pièce jointe d’un e-mail, ou une copie papier que vous pouvez scanner pour la classer. Cela est classique dans le cas des commandes, lorsque ces fichiers de documents entrants sont des reçus de paiements pour des dépenses ou de petits achats.

À partir de fichiers PDF ou image représentant des documents entrants, un service OCR externe (reconnaissance optique de caractères) peut générer des documents électroniques qui peuvent ensuite être convertis en enregistrements de document au sein de [!INCLUDE[prod_short](includes/prod_short.md)]. Choisissez un package de services adapté à votre organisation et/ou votre pays/région. Vous pouvez également créer des écritures manuellement pour représenter les documents externes.  

Sur la page **Documents entrants**, vous pouvez utiliser différentes fonctions pour examiner les reçus de dépenses, gérer les tâches ROC et convertir les fichiers document entrants, manuellement ou automatiquement, en documents ou lignes feuille appropriés. Les fichiers externes peuvent être joints à n’importe quelle étape du processus, notamment en ce qui concerne les documents validés et au fournisseur, au client qui en résulte, et dans les écritures comptables.

Le processus de document entrant est composé des activités principales suivantes :

* Enregistrez les documents externes dans [!INCLUDE[prod_short](includes/prod_short.md)] en créant des lignes sur la page **Documents entrants** de l’une des manières suivantes :
  * Manuellement, à l’aide de fonctions simples, à partir d’un PC ou d’un périphérique mobile, de l’une des manières suivantes :
    * Utilisez le bouton **Créer à partir d’un fichier**, puis renseignez les champs appropriés sur la page **Document entrant**. Le fichier est automatiquement joint.  
    * Utilisez le bouton **Nouveau**, renseignez les champs appropriés sur la page **Document entrant**, puis joignez manuellement le fichier associé.
    * À partir d’une tablette ou d’un téléphone, utilisez le bouton **Créer à partir de l’appareil photo** pour créer un enregistrement de document entrant, puis envoyez l’image au service OCR, par exemple.
  * Automatiquement en recevant le document du service OCR en tant que document électronique après avoir envoyé par e-mail le fichier PDF ou image associé au service OCR. Le raccourci **Informations financières** est automatiquement renseigné sur la page **Document entrant**.
* Utilisez le service ROC pour convertir des fichiers PDF ou image en documents électroniques pouvant être convertis en enregistrements de document dans [!INCLUDE[prod_short](includes/prod_short.md)].
* Créez des documents ou des lignes feuille comptabilité à partir d’enregistrements document entrants en saisissant les informations telles que vous les lisez à partir des fichiers document entrants.
* Joignez des fichiers document entrant à des documents vente et achat de tout statut, notamment au fournisseur, client, et écritures comptables qui résultent de la validation.
* Affichez les enregistrements document entrant et leurs pièces jointes à partir de tout document achat et vente ou de toute écriture, ou recherchez toutes les écritures comptables sans enregistrement document entrant sur la page **Plan comptable**.

| À | Voir |
| --- | --- |
| Configurer la fonctionnalité Documents entrants et le service OCR. |[Configurer des documents entrants](across-how-setup-income-documents.md) |
| Créer des enregistrements document entrant, joindre des fichiers, utiliser le service OCR pour convertir des fichiers PDF en documents électroniques, convertir les documents électroniques en enregistrements de document, auditer les enregistrements document entrant à partir de documents vente et achat validés. |[Traitement des documents entrants](across-process-income-documents.md) |

## <a name="see-related-training-at-microsoft-learn"></a>Voir la formation associée sur [Microsoft Learn](/learn/modules/incoming-documents-dynamics-365-business-central/index)

## <a name="see-also"></a>Voir aussi

[Achats](purchasing-manage-purchasing.md)  
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]