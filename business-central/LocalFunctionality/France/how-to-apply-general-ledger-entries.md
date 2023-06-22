---
title: 'Lettrer des écritures comptables [FR]'
description: Vous lettrez les écritures comptables pour justifier les soldes des comptes d’actif et de passif.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.search.form: '16, 10842'
ms.date: 06/18/2021
ms.author: bholtorf
---
# <a name="apply-general-ledger-entries-in-the-french-version" />Appliquer les écritures comptables dans la version française

> [!NOTE]
> Les entreprises de tous les pays peuvent bénéficier de la possibilité d’examiner les écritures comptables avant de les valider. Dans une prochaine version, nous rendrons obsolète la fonctionnalité spécifique au pays et la remplacerons par une autre disponible dans toutes les versions nationales. Une fois la fonctionnalité obsolète, vous pouvez l’utiliser pour accéder aux examens précédents, mais pas pour en faire de nouveaux. Nous archiverons vos données conformément aux exigences locales. Pour en savoir plus sur l’obsolescence, accédez à [Fonctionnalités obsolètes dans l’application de base](/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-w1). Pour en savoir plus sur la fonction de remplacement, accédez à [Revoir les montants dans les comptes généraux](../../finance-review-accounts.md).

Vous lettrez les écritures comptables pour justifier les soldes des comptes d’actif et de passif. Par exemple, vous pouvez lettrer des transactions dans les comptes de lettre de change afin d’obtenir une image précise des lettres constituant le solde du compte.  

## <a name="to-apply-general-ledger-entries" />Pour lettrer des écritures comptables

1. Sélectionnez l’icône ![Ampoule qui ouvre la fonction Tell Me.](../../media/ui-search/search_small.png "Dites-moi ce que vous voulez faire") entrez **Plan comptable**, puis choisissez le lien associé.  
2. Sur la page **Plan comptable**, sélectionnez le compte dans lequel vous souhaitez lettrer les écritures, puis choisissez l’action **Écritures ouvertes**.  
3. Sur la page **Lettrage écritures comptables**, sélectionnez les écritures comptables à lettrer.  
4. Choisissez **Définir ID lettrage** pour remplir le champ **ID lettrage** avec le code de l’utilisateur actuel.  
5. Sélectionnez l’action **Valider le lettrage**.  

Le lettrage est effectué en définissant les champ **Lettre** et **Date de la lettre**.  

> [!NOTE]  
> les écritures lettrées peuvent être identifiées par la même combinaison de trois lettres et la même date.

## <a name="see-also" />Voir aussi

[Délettrer des écritures comptables](how-to-unapply-general-ledger-entries.md)  
[Lettrer les paiements fournisseur manuellement](../../payables-how-apply-purchase-transactions-manually.md)

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
