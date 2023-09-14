---
title: 'Paramétrer des types de règlement [FR]'
description: 'Pour utiliser le module Gestion des paiements dans la version française, vous devez paramétrer des types de règlement pour définir des types d’opération, tels que des lettres de change, des paiements électroniques ou des chèques.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.form: '10868, 10870, 10860, 10861, 10864, 10865, 10866, 10871, 10872, 10873, 10874, 10877, 10878, 10879, 10869, 10867, 10882, 10880'
ms.date: 07/07/2021
ms.author: bholtorf
---
# <a name="set-up-payment-classes"></a>Paramétrer des types de règlement

Pour utiliser le module Gestion des paiements dans la version française de [!INCLUDE [prod_short](../../includes/prod_short.md)], vous devez paramétrer des types de règlement pour définir des types d’opération, tels que des lettres de change, des paiements électroniques ou des chèques. Les classes de paiement sont définies sur la page **Paramètres bordereau de paiement**.  

Pour chaque type d’opération, vous définissez ensuite les différents statuts que peut avoir le type d’opération, et vous associez à chaque statut des étapes pour définir comment le paiement passe d’un statut à l’autre.  

## <a name="to-set-up-a-payment-class"></a>Pour paramétrer un type de règlement

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Configuration bordereau de paiement**, puis sélectionnez le lien pertinent.  
2. Sur la page **Configuration bordereau de paiement**, sélectionnez l’action **Nouveau**.  
3. Renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Activer**|Permet d’activer l’utilisation du type de règlement.|  
    |**Code**|Code d’identification unique du type de règlement.|  
    |**Nom**|Description du type de règlement.|  
    |**N° de souche en-tête**|Code souche de numéros pour l’en-tête du bordereau paiement.|  
    |**N° de souche lignes**|Code souche de numéros pour les lignes du bordereau paiement. Si vous laissez ce champ vide, le numéro de chaque ligne paiement est créé en se basant sur le numéro d’en-tête du bordereau paiement.|  
    |**Propositions**|Type de proposition de règlement qui peut être créé automatiquement sur un bordereau paiement.|  
    |**Contrepassation de TVA sur encaissement**|Spécifiez la méthode pour gérer la TVA sur encaissement.<br /><br /> Si vous sélectionnez **Lettrage**, la TVA sera réalisée lors de la validation du lettrage de la facture et du paiement.<br /><br /> Si vous sélectionnez **En retard**, vous devez définir l’étape de règlement au cours de laquelle la TVA doit être réalisée, en sélectionnant le champ **Réaliser TVA** sur la page **Fiche étape règlement**.|  
    |**Type transfert SEPA**|Spécifiez le format d’exportation SEPA, **Virement** ou **Prélèvement**. Vous spécifiez le format d’exportation pour les virements SEPA dans les étapes de paiement pour la classe de paiement.|  

## <a name="to-set-up-payment-statuses-for-a-payment-class"></a>Pour paramétrer les statuts de paiement pour une classe de paiement

1. Sur la page **Configuration bordereau paiement**, sélectionnez un type de règlement, puis sélectionnez l’action **Statut**.  
2. Sur la page **Statut règlement**, sélectionnez l’action **Nouveau**.  
3. Remplissez les champs. [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]  

    Par exemple, le champ **RIB** indique que les informations relatives au Relevé d’Identité Bancaire (RIB) du client ou du fournisseur doivent être affichées dans les lignes paiement. Les informations du RIB incluent le code établissement, le code agence, le numéro de compte bancaire, le nom de la banque, la clé RIB et la clé de vérification.

4. Lorsque vous avez défini les statuts souhaités pour cette classe de paiement, revenez à la page **Configuration bordereau paiement**.  

Ensuite, vous devez définir les étapes pour chaque type de règlement. Les étapes de paiement définissent comment le paiement passe d’un état à l’autre, comme *Création de documents*, *Documents créés* et *Création de paiements*.  

## <a name="to-set-up-payment-steps-for-a-payment-class"></a>Pour paramétrer les étapes de paiement pour une classe de paiement

1. Sur la page **Configuration bordereau paiement**, sélectionnez un type de règlement, puis sélectionnez l’action **Étapes**.  
2. Dans la liste **Étape de paiement**, ajoutez les étapes pertinentes pour cette classe de paiement. Pour chaque étape, vous pouvez entrer 50 caractères alphanumériques maximum.  
3. Sélectionnez la première étape, puis cliquez sur l’action **Modifier**.  
4. Sur la page **Fiche Étape règlement**, renseignez le champs. [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]

> [!TIP]
> Le champ **Statut précédent** définit le statut précédent, à partir duquel l’étape a été exécutée pour la dernière fois. La valeur par défaut est 0, et la première étape aura 0 comme valeur du champ **Statut précédent**.
>
> Pour rendre une étape facultative et potentiellement répétable, définissez le statut précédent pour qu’il soit égal au statut suivant.
>
> Les champs **Type d’action**, **Type d’exportation** et **N° d’exportation** sont associés. Par exemple, pour les fichiers de virement SEPA, définissez **Type d’exportation** sur **XMLport**, puis définissez le champ **N° d’exportation** sur 1000. Pour les dossiers de prélèvement SEPA, spécifiez **XMLport**, puis définissez le champ **N° exportation** sur 1010.

Si le type d’action de l’étape règlement est **Comptabilité**, vous devez définir des informations supplémentaires pour l’étape règlement.  

### <a name="to-set-up-ledger-information-for-a-payment-step"></a>Pour définir des informations de comptabilité lors d’une étape de paiement

1. Sur la page **Fiche étape règlement** de l’étape règlement, choisissez l’action **Comptabilité**.  
2. Sur la page **Etape comptabilisation règlement**, sélectionnez l’action **Nouveau**.  
3. Renseignez les autres champs, comme nécessaire. [!INCLUDE [tooltip-inline-tip_md](../../includes/tooltip-inline-tip_md.md)]

## <a name="see-also"></a>Voir aussi

 [Gestion des paiements](payment-management.md)  
 [Configurer des adresses de paiement](how-to-set-up-payment-addresses.md)  
 [Exporter ou importer les paramètres de configuration de la gestion des paiements](how-to-export-or-import-payment-management-setup-parameters.md)  
 [Créer bordereaux paiement](how-to-create-payment-slips.md)  
 [Valider des bordereaux paiement](how-to-post-payment-slips.md)  
 [Archiver les bordereaux de paiement](how-to-archive-payment-slips.md)

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
