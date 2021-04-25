---
title: Vue d'ensemble des processus de fin d'exercice
description: Une clôture d'exercice dans Business Central implique trois étapes.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: fcbb2c273aad9cd349c811aaea74d5575f1678f7
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5782377"
---
# <a name="year-end-processes-overview"></a>Vue d'ensemble des processus de fin d'exercice

Une clôture d'exercice dans [!INCLUDE[prod_short](../../includes/prod_short.md)] implique trois étapes :  

1. Clôture de l'exercice comptable. Pour plus d'informations, voir [Clôturer fiscalement des périodes comptables](how-to-fiscally-close-accounting-periods.md).  
2. Générer une écriture de clôture d'exercice via l'option **Clôturer exercice comptable** avec la compensation des écritures de compte de fonds propres. Pour plus d'informations, reportez-vous à [Validation de l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md).  
3. Clôture de l'exercice comptable. Pour plus d'informations, voir [Clôturer fiscalement des exercices](how-to-fiscally-close-years.md).  

Selon la norme française *NF Logiciel compatibilité informatisée*, le système doit refuser la création d'un troisième exercice comptable ouvert. Seuls deux exercices comptables peuvent donc être ouverts en même temps.  

Vous devez dès lors clôturer l'exercice en temps voulu. Les détails des transactions ne risquent pas d'être perdus lorsque vous clôturez l'exercice, puisqu'ils sont tous mémorisés, même après avoir clôturé fiscalement l'exercice.  

Lors de la clôture en fin d'exercice, le système déplace vos bénéfices des bénéfices calculés, ou du compte Bénéfices actuels, vers un compte validé, ou le compte Bénéfices non répartis. Le système indique également que l'exercice comptable est « clôturé » et renseigne toutes les entrées suivantes pour l'exercice clôturé comme « écritures de l'exercice précédent ».  

Le système génère ensuite une écriture de clôture mais ne la valide pas automatiquement. Vous avez la possibilité de créer les écritures comptables de fonds propres de décalage qui vous permettent de choisir la manière dont vous voulez affecter votre écriture de clôture. Par exemple, si votre société comprend plusieurs départements, vous pouvez laisser le système générer une écriture de clôture unique pour tous les départements et créer une écriture de décalage pour le compte de fonds propres de chaque département.  

Après avoir clôturé fiscalement un exercice, vous ne pourrez plus rien comptabiliser dans cet exercice.  

## <a name="see-also"></a>Voir aussi

[Clôturer fiscalement des périodes comptables](how-to-fiscally-close-accounting-periods.md)  
[Validation de l'écriture de clôture d'exercice](how-to-post-the-year-end-closing-entry.md)  
[Clôturer fiscalement des exercices](how-to-fiscally-close-years.md)  
[Périodes fiscales et exercices comptables](fiscal-periods-and-fiscal-years.md)  
[Clôture des exercices et des périodes](../../year-close-years-periods.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]