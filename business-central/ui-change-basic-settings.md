---
title: Modifier les paramètres de base pour l'utilisateur actuel
description: Découvrez comment modifier certains paramètres de base, par exemple, votre tableau de bord, la société ou la date de travail.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: change Role Center, notification, change company, change work date
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: a0a504aa7c06c08d2e9f4251128e4203f0f90dee
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5787451"
---
# <a name="change-basic-settings"></a>Modifier les paramètres de base

Sur la page **Mes paramètres**, vous pouvez afficher et modifier les paramètres de base de votre [!INCLUDE[prod_short](includes/prod_short.md)]. Vos modifications affectent uniquement votre espace de travail, et non les espaces de travail des autres utilisateurs.  

## <a name="role"></a><a name="role-center"></a>Rôle

Le rôle détermine la page d’accueil, un écran de démarrage conçu pour les exigences d’un rôle spécifique dans une organisation. Selon votre rôle, la page d'accueil ou le tableau de bord donne une vue d’ensemble de l’entreprise, de votre département ou de vos tâches personnelles. Il vous permet également d’accéder à vos tâches quotidiennes et de rechercher les tâches qui vous sont affectées.

* En haut, la navigation vous permet de permuter entre les clients, les fournisseurs, les articles et d’autres listes d’informations importantes. De même, les actions vous permettent de lancer des tâches, comme la création d’une facture vente, directement à partir de la page d'accueil.

* Le tableau de bord contient une zone **Activités** qui affiche les données actuelles, vous pouvez cliquer ou appuyer dessus pour afficher des informations plus détaillées. Les indicateurs de performance clés peuvent être configurés afin d’afficher un graphique sélectionné pour une représentation visuelle, par exemple, de la trésorerie ou des revenus et des dépenses. Vous pouvez également générer la liste des clients favoris sur la page d'accueil pour les comptes d'entreprise avec lesquels vous travaillez souvent ou auxquels vous devez accorder une attention particulière.

### <a name="to-change-the-role"></a>Pour modifier le rôle

Le rôle par défaut est **Gestionnaire d’activité**, mais vous pouvez sélectionner un autre rôle pour utiliser un Tableau de bord qui correspond mieux à vos besoins.  

1. Dans le coin supérieur droit, sélectionnez l’icône **Paramètres** ![Paramètres](media/ui-experience/settings_icon_small.png "Icône Paramètres du tableau de bord"), puis choisissez l’action **Mes paramètres**.
2. Sur la page **Mes paramètres**, dans le champ **Rôle** , sélectionnez le rôle que vous souhaitez utiliser par défaut. Par exemple, sélectionnez **Comptable**.
3. Cliquez sur le bouton **OK**.

## <a name="company"></a><a name="company"></a>Société

Dans [!INCLUDE[prod_short](includes/prod_short.md)], une société fonctionne comme un conteneur de données. Il peut y avoir plusieurs sociétés dans une seule base de données, mais une seule peut être sélectionnée à la fois.

La société par défaut est appelée CRONUS et contient uniquement des données de démonstration. Vous pouvez créer une nouvelle société avec des données personnalisées. Pour plus d’informations, voir [Création de sociétés](about-new-company.md).

### <a name="to-change-the-company-name"></a>Pour changer le nom de la société

Le nom de la société est toujours affiché dans le coin supérieur gauche et fonctionne comme une action que vous pouvez choisir pour revenir dans le Tableau de bord. Vous pouvez changer ce nom sur la page **Informations société**.

1. Choisissez simplement l’icône ![Pignon pour ouvrir le menu Paramètres](media/ui-experience/settings_icon_small.png), puis l’action **Informations société**.
2. Dans le champ **Nom**, saisissez le nom de la nouvelle société.
3. Quittez la page. Le système redémarre et affiche la nouvelle société dans le coin supérieur gauche.

### <a name="to-display-a-company-badge-for-quick-access-to-company-information"></a><a name="badge"></a>Pour afficher un badge d’entreprise pour un accès rapide aux informations de la société

Vous pouvez ajouter un badge personnalisé dans le coin supérieur droit, vous pouvez ensuite choisir d’afficher rapidement le nom de la société et les informations sur l’abonné dans une fenêtre contextuelle. Le badge société est également utile lorsque [!INCLUDE[prod_short](includes/prod_short.md)] est intégré dans une autre application, comme Microsoft Teams ou dans une autre application Web. Dans ces cas, parce que le [!INCLUDE[web_client](includes/web_client.md)] affiche moins d’informations contextuelles adjacentes, le badge société est le seul moyen de déterminer à quelle société ou environnement appartient un enregistrement.

1. Choisissez l’icône ![Ampoule qui ouvre la fonction Tell Me](media/ui-search/search_small.png "Dites-moi ce que vous voulez faire"), entrez **Informations société**, puis sélectionnez le lien associé.
2. Sur le raccourci **Badge société**, renseignez les champs, le cas échéant. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].

> [!NOTE]
> Si un badge de société est défini, vous ne pouvez pas modifier le nom de la société comme décrit dans [Pour changer le nom de la société](ui-change-basic-settings.md#to-change-the-company-name)

## <a name="work-date"></a><a name="work-date"></a>Date de travail
La date de travail la plus couramment utilisée est la date du jour. Vous pouvez être amené à modifier temporairement la date de travail pour effectuer des tâches telles que l’exécution de transactions à une date différente de la date du jour.

> [!TIP]  
> Dans tous les champs de date, tapez **t** pour entrer rapidement la date du jour et tapez **w** pour entrer rapidement la date de travail, qui est la valeur du champ **Date de travail** sur la page **Mes paramètres**.

> [!IMPORTANT]  
> Une fois la date de travail modifiée, si vous vous déconnectez ou si vous changez de société, les données de travail reviennent par défaut à la date de travail. Ainsi, la prochaine fois que vous vous connecterez ou lorsque vous reviendrez à la société d’origine, vous devrez peut-être redéfinir la date de travail.

### <a name="work-date-indication"></a>Indication de la date de travail

La date de travail est une information primordiale sur les pages qui peuvent être éditées. Chaque fois que la date de travail n’est pas définie sur la date du jour sur une page modifiable, deux types d’indicateurs apparaissent sur la page :

* Un rappel apparaît en haut de la page pour vous indiquer la date de travail. Le rappel fournit un lien direct vers le paramètre de la date de travail sur la page **Mes paramètres** de sorte que vous pouvez modifier la date si vous voulez. À partir du rappel, vous pouvez également choisir de l’annuler pour le reste de votre session. À moins que vous ne remplaciez la date de travail par « aujourd’hui », le rappel apparaîtra la prochaine fois que vous vous connecterez.

* Si vous refusez le rappel, la date de travail apparaîtra dans le titre de la page.  

Si la date de travail n’est pas définie sur la date actuelle (aujourd’hui), alors la date de travail actuelle s’affiche dans l’angle supérieur gauche sur toutes les pages sur lesquelles vous pouvez modifier les données.

## <a name="region"></a><a name="region"></a> Région

Le paramètre **Région** détermine la manière dont les dates, heures, nombres et devises sont affichés ou mis en forme.

## <a name="language"></a><a name="language"></a> Langue

Modifie la langue d’affichage. Ce champ s’affiche uniquement lorsque vous avez le choix entre plusieurs langues.

La langue initiale est déterminée par l’administrateur ou par les paramètres de votre navigateur lorsque vous vous inscrivez à [!INCLUDE[prod_short](includes/prod_short.md)]. La langue définie est utilisée sur tous les appareils à partir desquels vous vous connectez, par exemple un téléphone ou une tablette.

Des langues supplémentaires pour [!INCLUDE[prod_short](includes/prod_short.md)] peuvent être installées à partir d’AppSource. Même si toutes les langues d’affichage prises en charge sont affichées dans la liste, l’administrateur doit installer l’application de langue appropriée sur l’abonné avant que les utilisateurs puissent passer à la nouvelle langue dans [!INCLUDE[prod_short](includes/prod_short.md)].  

## <a name="time-zone"></a>Fuseau horaire

Définit le fuseau horaire dans lequel vous vous trouvez. Lorsque vous vous connectez pour la première fois à [!INCLUDE [prod_short](includes/prod_short.md)], le fuseau horaire est défini en fonction de l'adresse de votre entreprise. Modifiez-le s'il ne correspond pas à votre emplacement physique.  

## <a name="notifications"></a>Notifications

Sélectionnez le lien *Modifier quand je reçois une notification* pour afficher ou modifier les notifications que vous recevez au sujet de certains événements ou modification de statut, lorsque vous êtes sur le point de facturer un client avec des écritures échues, ou lorsque le stock disponible est inférieur à la quantité que vous êtes sur le point de vendre. Pour plus d’informations, voir [Gérer les notifications](ui-smart-notifications.md).

## <a name="teaching-tips"></a>Conseils d’apprentissage

[!INCLUDE [ua-teachingtips](includes/ua-teachingtips.md)]

## <a name="see-related-training-at-microsoft-learn"></a>Voir la formation associée sur [Microsoft Learn](/learn/modules/personalize-ui-dynamics-365-business-central/index)

## <a name="see-also"></a>Voir aussi

[Création de sociétés](about-new-company.md)  
[Utilisation de [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Modifier les fonctionnalités affichées](ui-experiences.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
