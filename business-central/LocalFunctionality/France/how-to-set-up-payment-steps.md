---
title: Comment paramétrer des étapes règlement
description: Pour utiliser la gestion des paiements, vous devez configurer les étapes pour les documents de règlement et définir des étapes règlement pour chaque statut de paiement.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 2553630154bb659b20d70b99f44de32e28a70440
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/01/2020
ms.locfileid: "3920110"
---
# <a name="set-up-payment-steps"></a>Paramétrer des étapes règlement
Pour utiliser la gestion des paiements, vous devez configurer les étapes pour les documents de règlement et définir des étapes règlement pour chaque statut de paiement. Par exemple, « Création de documents », « Documents créés » et « Création de paiements ». Pour plus d'informations, voir [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md).  

## <a name="to-set-up-payment-steps"></a>Pour paramétrer des étapes règlement  

1.  Choisissez l'icône ![Ampoule qui ouvre la fonction Tell Me](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Paramètres bordereau paiement**, puis choisissez le lien approprié.  
2.  Sélectionnez un type de règlement, puis cliquez sur **Étapes**.  
3.  Dans le champ **Nom**, entrez un nom pour l'étape règlement. Vous pouvez entrer 50 caractères alphanumériques maximum.  
4.  Choisissez l'action **Modifier**.  
5.  Sur la page **Fiche étape règlement**, renseignez les champs comme indiqué dans le tableau ci-dessous.  

    |**Champ**|**Description**|  
    |---------------------------------|---------------------------------------|  
    |**Nom**|Nom de l'étape règlement entré sur la page **Étape règlement**.|  
    |**Statut précédent**|Statut précédent, à partir duquel l'étape a été exécutée pour la dernière fois. La valeur par défaut est 0. Si le statut précédent est le même que le statut suivant, il n'est pas modifié une fois exécuté. Par conséquent, cette étape règlement est facultative et peut être exécutée indéfiniment.|  
    |**Nom état précédent**|Nom du statut sélectionné dans le champ **Statut précédent**.|  
    |**Statut suivant**|Statut auquel cette étape règlement se termine.|  
    |**Nom état suivant**|Nom du statut sélectionné dans le champ **Statut suivant**. Ce champ ne peut pas être modifié.|  
    |**Type action**|Type d'action à effectuer à cette étape. <br /><br /> **Comptabilité :** si vous spécifiez **Comptabilité**, vous devez définir des informations supplémentaires sur la page **Etape comptabilisation règlement**.<br /><br /> **État :** si vous spécifiez **État**, indiquez l'état dans le champ **N° déclaration** .<br /><br /> **Fichier :**<br /><br /> * Si vous spécifiez **Fichier**, vous spécifiez le type de fichier dans le champ **Type exportation** : **État** ou **XMLPort**.<br /><br /> * Pour les dossiers de virement SEPA, spécifiez **XMLport**, puis définissez le champ **N° exportation** sur 1000.<br /><br /> * Pour les dossiers de prélèvement SEPA, spécifiez **XMLport**, puis définissez le champ **N° exportation** sur 1010.|  
    |**N° déclaration**|Numéro d'identification de l'état. Ce champ est disponible si le champ **Type action** est défini sur **État**.|  
    |**Type exportation**|Type d'exportation du fichier. Ce champ est disponible si le champ **Type action** est défini sur **Fichier**.<br /><br /> Pour obtenir des exemples, voir [Exporter les paiements](how-to-export-payments.md).|  
    |**N° exportation**|Code d'identification du type d'exportation sélectionné. Ce champ est disponible si le champ **Type action** est défini sur **Fichier**.|  
    |**Vérifier RIB lignes**|Sélectionnez pour vérifier que la valeur de clé du Relevé d'Identité Bancaire (RIB) spécifiée sur la ligne bordereau de paiement a été saisie correctement.|  
    |**Vérifier date d'échéance**|Sélectionne pour vérifier que la date d'échéance sur les lignes de facturation et de paiement a été entrée correctement.|  
    |**Code journal**|Code source associé à l'étape règlement.<br /><br /> Ce champ est disponible si le champ **Type action** est défini sur **Comptabilité**.|  
    |**Code motif**|Code motif associé à l'étape règlement.<br /><br /> Ce champ est disponible si le champ **Type action** est défini sur **Comptabilité**.|  
    |**N° de souche en-tête**|Code souche de numéros à utiliser pour affecter des numéros à l'en-tête d'un nouveau bordereau de paiement.<br /><br /> Ce champ est disponible si le champ **Type action** est défini sur **Créer un document**.|  
    |**Correction**|Sélectionnez pour marquer les écritures paiement comme écritures de correction. Ce champ est disponible si le champ **Type action** est défini sur **Comptabilité**.|  
    |**Réaliser TVA**|Sélectionnez pour indiquer que la TVA sur encaissement doit être contre-passée et la TVA déclarée pour cette étape règlement.<br /><br /> Ce champ est disponible si le champ **Contrepassation de TVA sur encaissement** sur la page **Types de règlement** est défini sur **En retard**.|  
    |**Vérifier RIB en-tête**|Sélectionnez pour vérifier que la valeur de clé du RIB spécifiée sur l'ente du bordereau de paiement a été saisie correctement.|  
    |**Code acceptation <> Non**|Sélectionnez pour vérifier que le code acceptation de chaque ligne paiement n'est pas un numéro.|  

6.  Cliquez sur le bouton **OK**.  

Si le type d'action de l'étape règlement est **Comptabilité**, vous devez définir des informations supplémentaires pour l'étape règlement.  

## <a name="to-set-up-ledger-information-for-a-payment-step"></a>Pour définir des informations de comptabilité lors d'une étape de paiement  

1.  Sur la page **Fiche étape règlement** de l'étape règlement, choisissez l'action **Comptabilité**.  
2.  Sur la page **Etape comptabilisation règlement**, sélectionnez l'action **Nouveau**.  
3.  Renseignez les champs comme indiqué dans le tableau suivant.  

    |**Champ**|**Description**|  
    |---------------------------------|---------------------------------------|  
    |**Signe**|Type d'écriture validation.|  
    |**Description**|Description de l'écriture.|  
    |**Type comptabilisation**|Type comptabilisation utilisé pour la validation de l'écriture.|  
    |**Type compte**|Type de compte de la validation de l'écriture. Ce champ est disponible si **Type comptabilisation** est **Compte paramétré**.|  
    |**N° compte**|Numéro de compte dans lequel l'écriture est validée. Le numéro de compte est affiché ici en fonction du type sélectionné dans le champ **Type compte**. Ce champ est disponible si **Type comptabilisation** est **Compte paramétré**.|  
    |**Groupe comptabilisation client**|Code du groupe comptabilisation client dans lequel l'écriture est validée. Ce champ est disponible si **Type comptabilisation** est **Compte ligne règlement**, **Compte général associé** ou **Compte en-tête**.|  
    |**Groupe comptabilisation fournisseur**|Code du groupe comptabilisation fournisseur dans lequel l'écriture est validée. Ce champ est disponible si **Type comptabilisation** est **Compte ligne règlement**, **Compte général associé** ou **Compte en-tête**.|  
    |**Racine**|Racine du groupe des comptes généraux. Elle est utilisée si **Type comptabilisation** est **Compte général par mois échéance** ou **Compte général par semaine échéance**.|  
    |**Mémoriser écriture**|Sélectionnez pour indiquer que les écritures comptables créées à cette étape seront conservées et lettrées à de nouvelles écritures validées. Si vous activez cette case à cocher, le champ **Détail** n'est pas disponible.|  
    |**Application**|Méthode pour lettrer les écritures. Si vous n'avez pas activé la case à cocher **Mémoriser écriture**, et que vous avez défini ce champ sur **Aucun**, le champ **Détail** est disponible.|  
    |**Détail**|Méthode de validation des lignes paiement.|  
    |**Type document**|Type de document affecté à l'écriture comptable.|  
    |**Numéro de document**|Méthode d'affectation du numéro document à l'écriture comptable.|  

4.  Cliquez sur le bouton **OK**.  

## <a name="see-also"></a>Voir aussi  
 [Gestion des paiements](payment-management.md)   
 [Paramétrer des types de règlement](how-to-set-up-payment-classes.md)   
 [Configurer des adresses de paiement](how-to-set-up-payment-addresses.md)   
 [Créer bordereaux paiement](how-to-create-payment-slips.md)   
 [Valider des bordereaux paiement](how-to-post-payment-slips.md)   
 [Archiver les bordereaux de paiement](how-to-archive-payment-slips.md)   
 [Exporter ou importer les paramètres de configuration de la gestion des paiements](how-to-export-or-import-payment-management-setup-parameters.md)
