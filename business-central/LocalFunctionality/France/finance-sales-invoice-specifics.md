---
title: Émettre des factures vente avec des spécificités françaises
description: Découvrez comment configurer et utiliser des informations spécifiques à la France dans les factures vente destinées à la France.
author: altotovi
ms.author: altotovi
ms.reviewer: kfend
ms.service: dynamics365-business-central
ms.topic: how-to
ms.date: 05/26/2023
ms.custom: bap-template
ms.search.keywords: 'sales, invoice, order, siren'
ms.search.form: '21, 42, 43, 44'
---

# <a name="deliver-sales-invoices-with-french-specifics" />Émettre des factures vente avec des spécificités françaises

Cet article explique comment configurer et utiliser les informations de facture vente spécifiques à la France.

## <a name="create-a-new-customer" />Créer un client

Lorsque vous créez un client en France, il convient d’inclure certaines informations spécifiques. Pour créer correctement la fiche **Client**, dans l’onglet **Facturation**, saisissez une valeur dans le **N° SIREN** . Ce numéro est nécessaire pour imprimer les factures vente.

Si la fiche **Client** est créée à partir d’une fiche **Contact** existante, la valeur du champ **N° SIREN** est copié à partir du contact.

## <a name="work-with-the-sales-documents" />Utiliser les documents de vente

Lorsque vous créez un document vente, vous pouvez choisir d’imprimer ou non la taxe sur la valeur ajoutée (TVA) acquittée sur les débits. Pour imprimer ces informations, dans l’onglet **Détails de facture**, activez le champ **TVA acquittée sur les débits**.

Lorsque vous imprimez des documents vente, [!INCLUDE[prod_long](../../includes/prod_long.md)] indique automatiquement, dans le commentaire, si une facture vente comprend uniquement des biens, uniquement des services ou à la fois des biens et des services. Cette détermination est basée sur la valeur du champ **Type** sur la fiche **Article** (**Inventaire** ou **Service**), les ressources utilisées ou le compte du grand livre.

> [!NOTE]
> Si vous utilisez une adresse secondaire dans la facture vente, [!INCLUDE[prod_long](../../includes/prod_long.md)] affiche automatiquement cette adresse dans le commentaire du rapport imprimé.

Vous pouvez trouver des informations de formation sur les factures vente sur [Microsoft Learn](/learn/modules/process-intrastat-dynamics-365-business-central/index).

## <a name="see-also" />Voir aussi

[Gestion financière](../../finance.md)  
[Utiliser [!INCLUDE[prod_short](../../includes/prod_short.md)]](../../ui-work-product.md)

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
