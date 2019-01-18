---
title: "Procédure de création des bordereaux paiement"
description: "Vous pouvez créer des bordereaux paiement pour gérer les paiements fournisseur et client. Avant de créer des bordereaux paiement, vous devez paramétrer des types de règlement."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: a2b313bee90f53590b6baf8be33cd75925f794ab
ms.contentlocale: fr-fr
ms.lasthandoff: 11/26/2018

---
# <a name="create-payment-slips"></a>Créer bordereaux paiement
Vous pouvez créer des bordereaux paiement pour gérer les paiements fournisseur et client. Avant de créer des bordereaux paiement, vous devez paramétrer des types de règlement. Pour plus d'informations, voir [Paramétrer des types de règlement](how-to-set-up-payment-classes.md).  

La procédure suivante décrit comment créer des bordereaux paiement pour les règlements fournisseur, mais les mêmes étapes s'appliquent également à la création des bordereaux paiement pour les règlements client.  

## <a name="to-create-a-payment-slip-for-vendors"></a>Pour créer un bordereau de paiement pour les fournisseurs  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Bordereaux paiement**, puis sélectionnez le lien approprié.  
2.  Sélectionnez l'action **Nouveau**.  
3.  Sur la page **Bordereau paiement**, sélectionnez un champ pour ouvrir la page **Liste des types de règlement**.  
4.  Sélectionnez un type de règlement, puis choisissez le bouton **OK**.  
5.  Sous le raccourci **Général**, renseignez les champs comme indiqué dans le tableau ci-dessous.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Code devise**|Spécifiez le code devise à utiliser pour les lignes paiement.|  
    |**Date de validation**|Spécifiez une date comptabilisation.|  
    |**Date document**|Spécifiez la date du document.|  
    |**Montant DS**|Montant total des lignes paiement. Ce champ est mis à jour automatiquement à chaque modification des montants nets des lignes.<br /><br />|  

6.  Sous le raccourci **Lignes**, renseignez les champs comme indiqué dans le tableau ci-dessous.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Type compte**|Type de compte sur lequel la ligne bordereau est validée.|  
    |**N° compte**|Numéro d'identification unique pour le compte sur lequel l'écriture est validée.|  

7.  Dans le champ **Code compte bancaire**, sélectionnez un nom bancaire dans la liste, puis choisissez **Avancé**.  
8.  Éventuellement, pour SEPA, sur la page **Sélectionner – Liste des comptes fournisseur**, puis cliquez sur l'action **Modifier**.  

    Renseignez les champs suivants, si nécessaire :  

    - **Code pays/région**. Dans la liste, choisissez **Avancé**, puis assurez-vous que la case à cocher **SEPA autorisé** est sélectionnée pour le code que vous sélectionnez.  
    - **Code SWIFT**  
    - **IBAN**  

    Cliquez sur le bouton **OK** pour fermer la page.  

9. Éventuellement, pour SEPA, choisissez l'action **Relevé d'identité bancaire**. Sélectionnez le champ **Code pays/région banque**, puis choisissez **Avancé**. Assurez-vous que la case à cocher **SEPA autorisé** est sélectionnée. Assurez-vous également que les champs **IBAN** et **Code SWIFT** sont renseignés.  

10. Choisissez l'action **Proposer paiements fournisseur**.  

    > [!NOTE]  
    >  Vous pouvez également renseigner manuellement les lignes paiement.  

11. Dans le traitement par lots **Proposer paiements fournisseur**, sur le raccourci **Options**, renseignez les champs comme indiqué dans le tableau suivant.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Dernière date échéance**|Dernière date de paiement pour les écritures comptables fournisseur à inclure dans le traitement par lots.|  
    |**Rechercher les escomptes**|Sélectionnez d'inclure les écritures comptables fournisseur pour lesquelles vous pouvez obtenir un escompte.|  
    |**Totaliser par**|Critères de totalisation de la ligne paiement.|  
    |**Utiliser priorité fournisseur**|Sélectionnez de trier les paiements proposés en fonction de la valeur du champ **Priorité** sur les fiches fournisseur. Pour plus d'informations, voir Priorité.|  
    |**Montant disponible DS**|Montant maximal qui est disponible pour les paiements en devise société.|  
    |**Filtre devise**|Code de la devise à inclure dans le traitement par lots.|  

12. Sur le raccourci **Fournisseur**, sélectionnez les filtres appropriés.  
13. Choisissez le bouton **OK**.  

    Les lignes paiement sont automatiquement créées.  

14. Sur la page **Bordereau paiement**, sous le raccourci **Validation**, renseignez les champs comme indiqué dans le tableau ci-dessous.  

    |Champ|Désignation|  
    |---------------------------------|---------------------------------------|  
    |**Code journal**|Code source du bordereau paiement.|  
    |**Code emplacement immo**|Code axe analytique approprié.|  
    |**Code projet**|Code axe analytique approprié.|  
    |**Type compte**|Type de compte vers et à partir duquel les paiements seront transférés.|  
    |**N° compte**|Numéro de compte vers et à partir duquel les paiements seront transférés.|  

15. Éventuellement, pour SEPA, dans le champ **N° compte**, choisissez l'option **Avancé**.  

    1. Sur la page **Liste des comptes bancaires**, sélectionnez l'action **Modifier**.  
    2. Renseignez les champs suivants, si nécessaire :  

        - Raccourci **Général**  
        - **Code pays/région**  
        - Raccourci **Transfert**  
        - **Code SWIFT**  
        - **IBAN**  
        - Raccourci **RIB**  
        - **Format exportation paiement** : SEPA  
        - **Souches de n° ID Msg Virement SEPA** : Banque  

16. Cliquez sur le bouton **OK**.  

Après avoir créé un bordereau de paiement, vous pouvez générer des fichiers de paiement et les envoyer à la banque par voie électronique.  

> [!NOTE]  
>  Un fichier de paiement peut être créé si le bordereau de paiement affiche **Fichier** dans le champ **Type action**.

## <a name="to-create-a-payment-file"></a>Pour créer un fichier de paiement  

1.  Sélectionnez l'icône ![Page ou état pour la recherche](../../media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Bordereaux paiement**, puis sélectionnez le lien approprié.  
2.  Sélectionnez un bordereau paiement, puis cliquez sur **Modifier**.  
3.  Sur la page **Bordereau paiement**, sélectionnez **Générer fichier**.  
4.  Cliquez sur le bouton **Oui**, puis sur le bouton **OK**.  

    Le fichier de paiement est généré et exporté en fonction du type d'exportation spécifié sur la page **Étape règlement**.  

5.  En cas d'erreur, consultez les erreurs répertoriées dans le récapitulatif **Erreurs exportation fichier** et prenez la mesure appropriée.  

## <a name="see-also"></a>Voir aussi  
 [Gestion des paiements](payment-management.md)   
 [Paramétrer des types de règlement](how-to-set-up-payment-classes.md)   
 [Paramétrer des statuts règlement](how-to-set-up-payment-statuses.md)   
 [Paramétrer des étapes règlement](how-to-set-up-payment-steps.md)   
 [Configurer des adresses de paiement](how-to-set-up-payment-addresses.md)   
 [Valider des bordereaux paiement](how-to-post-payment-slips.md)   
 [Archiver les bordereaux de paiement](how-to-archive-payment-slips.md)   
 [Exporter ou importer les paramètres de configuration de la gestion des paiements](how-to-export-or-import-payment-management-setup-parameters.md)

