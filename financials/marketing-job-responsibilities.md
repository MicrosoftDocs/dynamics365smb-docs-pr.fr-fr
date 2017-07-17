---
title: "Configuration des responsabilités pour des contacts | Microsoft Docs"
description: "Décrit les responsabilités pour les contacts dans Financials"
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, to-do, relationship, prospect
ms.date: 03/28/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: 610ae314502e60b959f0e2ff705a48b936d79d68
ms.contentlocale: fr-fr
ms.lasthandoff: 05/04/2017


---
# <a name="setting-up-job-responsibilities-for-contact-persons"></a>Configuration des responsabilités pour les personnes contact
Vous pouvez ajouter des informations relatives aux responsabilités des personnes contact afin d'indiquer les tâches dont une personne contact est responsable au sein de sa société, par exemple, l'informatique, la gestion ou la production. Vous pouvez utiliser ces informations lors de la saisie de données sur vos contacts.

L'utilisation des responsabilités sur les contacts est un processus en deux étapes. Tout d'abord, vous définissez le code responsabilité. Vous ne devez effectuer cette étape qu'une seule fois pour chaque responsabilité. Une fois que vous disposez d'un code responsabilité, vous pouvez commencer à affecter ce code aux personnes contact.

## <a name="tp-define-a-job-responsibility-code"></a>Définir un code de responsabilité
Le code responsabilité définit le type ou la catégorie du projet, par exemple MARKETING ou ACHAT. Vous pouvez disposer de plusieurs codes responsabilité. La fenêtre **Responsabilités** vous permet de définir la responsabilité.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche** ![Page ou état pour la recherche](media/ui-search/search_small.png "Icône Page ou état pour la recherche"), entrez **Responsabilités**, puis sélectionnez le lien associé.
2. Sélectionnez l'action **Nouveau**, et entrez un code et une désignation. Vous pouvez saisir pour le code un maximum de 11 caractères, et toute combinaison de chiffres et des lettres.

## <a name="to-assign-job-responsibilities-to-a-contact-person"></a>pour affecter des responsabilités à vos contacts
Vous ne pouvez pas affecter de responsabilités aux sociétés contact.

1. Ouvrez la fiche de la personne contact.
2. Sélectionnez l'action **Personne**, puis sélectionnez l'action **Responsabilités**. La fenêtre **Responsabilités contact** s'affiche.
3. Dans le champ **Code responsabilité**, sélectionnez la responsabilité que vous souhaitez affecter.

Répétez ces étapes pour chaque responsabilité à affecter. Vous pouvez également affecter des responsabilités à partir de la liste des contacts en suivant la même procédure.

Le nombre de responsabilités affectées au contact s'affiche dans le champ **Nbre responsabilités** de la section **Segmentation** de la fenêtre **Contact**.

Une fois que vous avez affecté des responsabilités à vos contacts, vous pouvez utiliser ces informations pour sélectionner des contacts pour vos segments. Pour plus d'informations, reportez-vous à [Procédure : ajouter des contacts à des segments](marketing-add-contact-segment.md).

## <a name="see-also"></a>Voir aussi
[Création de personnes contact](marketing-create-contact-persons.md)  
[Création de sociétés contact](marketing-create-contact-companies.md)  
[Utilisation de Financials](ui-work-product.md)
