---
title: Créer une demande de prix pour demander une offre | Microsoft Docs
description: Décrit comment créer une offre vente offrent ou un document de demande de proposition pour enregistrer votre offre à un client pour vendre des produits dans certaines conditions.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: rfq
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 416c5a4e4376932c16a1496f2db2b0c79307d22b
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5772618"
---
# <a name="request-quotes"></a>Demander des devis
Vous pouvez utiliser une demande de prix en tant que phase préliminaire d’une commande achat, et convertir cette commande en facture achat ou en commande.


## <a name="to-create-a-purchase-quote"></a>Pour créer une demande de prix
1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), saisissez **Demandes de prix**, puis sélectionnez le lien associé.
2. Créez un document, de la même manière que vous passez une commande achat. Pour plus d’informations, voir [Enregistrer des achats](purchasing-how-record-purchases.md).

## <a name="to-convert-a-purchase-quote-to-a-purchase-order"></a>Pour convertir une demande de prix en commande achat
Lorsque vous avez accepté le devis du fournisseur, vous pouvez le convertir en facture achat ou en commande pour procéder à l’achat.

1. Ouvrez une demande de prix est prête à être convertie, puis sélectionnez l’action **Créer commande**.

La demande de prix est supprimée de la base de données. Une facture achat ou une commande achat basée sur les informations de la demande de prix et dans laquelle vous pouvez traiter l’achat est créée. Dans le champ **N° devis** de la facture achat ou de la commande achat, vous pouvez visualiser le numéro de la demande de prix à partir de laquelle elle a été réalisée.

## <a name="see-also"></a>Voir aussi
[Achats](purchasing-manage-purchasing.md)  
[Définition des achats](purchasing-setup-purchasing.md)  
[Envoyer des documents par e-mail](ui-how-send-documents-email.md)  
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]