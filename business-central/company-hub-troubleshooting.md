---
title: Dépannage de votre Hub Entreprise
description: Découvrez comment contourner les problèmes lorsque vous dépannez votre Hub Entreprise dans Dynamics 365 Business Central pour gérer le travail dans plusieurs entreprises.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, troubleshoot
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 94bd2c0270263a1382094e559b4e70753f9bb91f
ms.sourcegitcommit: 311e86d6abb9b59a5483324d8bb4cd1be7949248
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2021
ms.locfileid: "5013581"
---
# <a name="troubleshooting-your-company-hub"></a><span data-ttu-id="03515-103">Dépannage de votre Hub Entreprise</span><span class="sxs-lookup"><span data-stu-id="03515-103">Troubleshooting Your Company Hub</span></span>

<span data-ttu-id="03515-104">L’ajout de sociétés au tableau de bord Hub Entreprise est assez facile, mais cet article traite des problèmes que vous pouvez rencontrer en route.</span><span class="sxs-lookup"><span data-stu-id="03515-104">Adding companies to the company hub dashboard is easy enough, but this article addresses issues that you may have on the way.</span></span>  

## <a name="check-errors"></a><span data-ttu-id="03515-105">Vérifier les erreurs</span><span class="sxs-lookup"><span data-stu-id="03515-105">Check errors</span></span>

<span data-ttu-id="03515-106">Utilisez l’action **Vérifier les erreurs** pour afficher une liste des erreurs récentes.</span><span class="sxs-lookup"><span data-stu-id="03515-106">Use the **Check Errors** action to view a list of recent errors.</span></span> <span data-ttu-id="03515-107">Vous pouvez voir des détails supplémentaires pour chaque erreur et vous pouvez nettoyer le journal en supprimant les anciennes entrées.</span><span class="sxs-lookup"><span data-stu-id="03515-107">You can see additional details for each error, and you can clean up the log by deleting older entries.</span></span>  

## <a name="connection-failed"></a><span data-ttu-id="03515-108">Échec de la connexion</span><span class="sxs-lookup"><span data-stu-id="03515-108">Connection failed</span></span>

<span data-ttu-id="03515-109">Il peut y avoir plusieurs raisons pour lesquelles vous ne pouvez pas vous connecter à une entreprise, notamment les suivantes :</span><span class="sxs-lookup"><span data-stu-id="03515-109">There can be a couple of reasons why you cannot connect to a company, including the following:</span></span>

- <span data-ttu-id="03515-110">L’URL dans le champ **Lien d’environnement** n’est pas valide</span><span class="sxs-lookup"><span data-stu-id="03515-110">The URL in the **Environment Link** field is not valid</span></span>  

  <span data-ttu-id="03515-111">Aller à la page **Liens d’environnements**, ouvrez l’environnement auquel vous ne pouvez pas vous connecter, puis choisissez l’action **Tester la connexion**.</span><span class="sxs-lookup"><span data-stu-id="03515-111">Go to the **Environment Links** page, open the environment that you cannot connect to, and then choose the **Test the connection** action.</span></span>  
- <span data-ttu-id="03515-112">La société du client est actuellement hors connexion, par exemple si elle est en cours de mise à niveau</span><span class="sxs-lookup"><span data-stu-id="03515-112">The client's company is currently offline, for example if it being upgraded</span></span>

  <span data-ttu-id="03515-113">Dans votre tableau de bord, choisissez l’élément de menu **Outils**, puis **Vérifier les erreurs**.</span><span class="sxs-lookup"><span data-stu-id="03515-113">In your dashboard, choose the **Tools** menu item, and then choose **Check Errors**.</span></span> <span data-ttu-id="03515-114">Cela ouvre une liste avec des informations techniques vous permettant de contacter votre administrateur si vous voyez des erreurs.</span><span class="sxs-lookup"><span data-stu-id="03515-114">This opens a list with technical details, so you might want to contact your administrator if you're seeing errors.</span></span> <span data-ttu-id="03515-115">Par exemple, le message d’erreur « *Le serveur a rejeté les informations d’identification du client* » suggère que vous n’avez pas accès.</span><span class="sxs-lookup"><span data-stu-id="03515-115">For example, the error message "*The server has rejected the client credentials*" suggests that you do not have access.</span></span>  
- <span data-ttu-id="03515-116">Vous n’avez pas accès à toutes les entreprises de l’environnement auquel vous essayez de vous connecter</span><span class="sxs-lookup"><span data-stu-id="03515-116">You do not have access to all companies in the environment that you are trying to connect to</span></span>

  <span data-ttu-id="03515-117">Dans [!INCLUDE [prod_short](includes/prod_short.md)], une organisation peut avoir plusieurs centres de profit appelés entreprises et vous n’aurez peut-être pas accès à toutes les entreprises.</span><span class="sxs-lookup"><span data-stu-id="03515-117">In [!INCLUDE [prod_short](includes/prod_short.md)], an organization can have multiple business units called companies, and you might not have access to all companies.</span></span> <span data-ttu-id="03515-118">Communiquez avec votre administrateur ou client pour vous assurer que vous avez accès aux sociétés dans lesquelles vous devez travailler.</span><span class="sxs-lookup"><span data-stu-id="03515-118">Work with your administrator or client to make sure that you have access to the companies that you have to work in.</span></span>  

## <a name="data-does-not-refresh"></a><span data-ttu-id="03515-119">Les données ne s’actualisent pas</span><span class="sxs-lookup"><span data-stu-id="03515-119">Data does not refresh</span></span>

<span data-ttu-id="03515-120">Lorsque vous ajoutez une société ou que vous demandez une actualisation des données, [!INCLUDE [prod_short](includes/prod_short.md)] récupère les données.</span><span class="sxs-lookup"><span data-stu-id="03515-120">When you add a company or request a refresh of the data, [!INCLUDE [prod_short](includes/prod_short.md)] fetches the data.</span></span> <span data-ttu-id="03515-121">Mais vous devez actualiser la page vous-même, par exemple en choisissant l’action **Afficher à nouveau toutes les sociétés**, actualisez la page du navigateur, quittez le tableau de bord puis retournez-y, ou similaire.</span><span class="sxs-lookup"><span data-stu-id="03515-121">But you must refresh the page yourself, such as choosing the **Reload all companies** action, refresh the browser page, navigate away from the dashboard and then back again, or similar.</span></span>  

<span data-ttu-id="03515-122">Si vous avez ajouté une entreprise, mais qu’elle ne s’affiche pas dans la liste, vous pouvez également utiliser l’action **Recharger toutes les entreprises** pour mettre à jour la liste.</span><span class="sxs-lookup"><span data-stu-id="03515-122">If you've added a company but it is not displaying in the list, you can also use the **Reload all companies** action to update the list.</span></span>

## <a name="see-also"></a><span data-ttu-id="03515-123">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="03515-123">See also</span></span>

[<span data-ttu-id="03515-124">Gérer le travail entre plusieurs entreprises dans le Hub Entreprise</span><span class="sxs-lookup"><span data-stu-id="03515-124">Manage Work across Multiple Companies in the Company Hub</span></span>](company-hub.md)  
[<span data-ttu-id="03515-125">Ajouter des entreprises à votre Hub Entreprise</span><span class="sxs-lookup"><span data-stu-id="03515-125">Add companies to your company hub</span></span>](company-hub-add-company.md)  
[<span data-ttu-id="03515-126">Expériences de comptables dans Business Central</span><span class="sxs-lookup"><span data-stu-id="03515-126">Accountant Experiences in Business Central</span></span>](finance-accounting.md)  