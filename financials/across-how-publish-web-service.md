---
title: Exposer des objets en tant que services Web | Microsoft Docs
description: "Lorsque vous publiez des objets [!INCLUDE[d365fin](includes/d365fin_md.md)] en tant que services Web, ils sont immédiatement disponibles sur le réseau."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 278515fc479a72957fb52dad71ce2f98d354ee32
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-publish-a-web-service"></a><span data-ttu-id="867b1-103">Procédure de publication d'un service Web</span><span class="sxs-lookup"><span data-stu-id="867b1-103">How to: Publish a Web Service</span></span>
<span data-ttu-id="867b1-104">Les services Web sont un moyen pratique de rendre une fonctionnalité d'application disponible à différents systèmes et utilisateurs externes.</span><span class="sxs-lookup"><span data-stu-id="867b1-104">Web services are a lightweight way to make application functionality available to a variety of external systems and users.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="867b1-105"> inclut plusieurs objets qui sont exposés par défaut en tant que services Web en raison de l'intégration à d'autres services Microsoft, mais vous pouvez également ajouter d'autres services Web.</span><span class="sxs-lookup"><span data-stu-id="867b1-105"> includes an number of objects that are exposed as web services by default due to integration with other Microsoft services, but you can also add other web services.</span></span>  

<span data-ttu-id="867b1-106">Vous pouvez configurer un service Web dans le client Windows ou le client Web.</span><span class="sxs-lookup"><span data-stu-id="867b1-106">You can set up a web service in the Windows client or in the Web client.</span></span> <span data-ttu-id="867b1-107">Vous devez ensuite publier le service Web pour le rendre disponible aux demandes de service sur le réseau.</span><span class="sxs-lookup"><span data-stu-id="867b1-107">You must then publish the web service so that it is available to service requests over the network.</span></span> <span data-ttu-id="867b1-108">Les utilisateurs peuvent découvrir les services Web en pointant un navigateur sur l'emplacement du serveur et en demandant la liste des services disponibles.</span><span class="sxs-lookup"><span data-stu-id="867b1-108">Users can discover web services by pointing a browser at the server location and requesting a list of available services.</span></span> <span data-ttu-id="867b1-109">Lorsque vous publiez un service Web, il est immédiatement disponible sur le réseau pour les utilisateurs authentifiés.</span><span class="sxs-lookup"><span data-stu-id="867b1-109">When you publish a web service, it is immediately available over the network for authenticated users.</span></span> <span data-ttu-id="867b1-110">Tous les utilisateurs autorisés peuvent accéder aux métadonnées des services Web, mais seuls les utilisateurs ayant les autorisations nécessaires peuvent accéder aux données réelles.</span><span class="sxs-lookup"><span data-stu-id="867b1-110">All authorized users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span></span>

## <a name="creating-and-publishing-a-web-service"></a><span data-ttu-id="867b1-111">Création et publication d'un service Web</span><span class="sxs-lookup"><span data-stu-id="867b1-111">Creating and Publishing a Web Service</span></span>  
 <span data-ttu-id="867b1-112">Les étapes suivantes expliquent la procédure de création et de publication d'un service Web.</span><span class="sxs-lookup"><span data-stu-id="867b1-112">The following steps explain how to create and publish a web service.</span></span>  

#### <a name="to-create-and-publish-a-web-service"></a><span data-ttu-id="867b1-113">Création et publication d'un service Web</span><span class="sxs-lookup"><span data-stu-id="867b1-113">To create and publish a web service</span></span>  

1.  <span data-ttu-id="867b1-114">Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Services Web**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="867b1-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Web Services**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="867b1-115">Dans la page **Services Web**, sélectionnez **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="867b1-115">In the **Web Services** page, choose **New**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    >  <span data-ttu-id="867b1-116">Les types valides pour les services Web SOAP sont **Codeunit** et **Page**.</span><span class="sxs-lookup"><span data-stu-id="867b1-116">**Codeunit** and **Page** are valid types for SOAP web services.</span></span> <span data-ttu-id="867b1-117">Les types valides pour les services Web OData sont **Page** et **Requête**.</span><span class="sxs-lookup"><span data-stu-id="867b1-117">**Page** and **Query** are valid types for OData web services.</span></span>  
    <span data-ttu-id="867b1-118">De même, si la base de données contient plusieurs sociétés, vous pouvez choisir un ID objet qui est spécifique à l'une des sociétés.</span><span class="sxs-lookup"><span data-stu-id="867b1-118">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span></span>  
    <span data-ttu-id="867b1-119">Enfin, le nom de service est visible par les clients de votre service Web et sert de base pour identifier et distinguer les services Web, il doit donc être explicite.</span><span class="sxs-lookup"><span data-stu-id="867b1-119">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span></span>

3.  <span data-ttu-id="867b1-120">Activez la case à cocher dans la colonne **Publié**.</span><span class="sxs-lookup"><span data-stu-id="867b1-120">Select the check box in the **Published** column.</span></span>  

     <span data-ttu-id="867b1-121">Lorsque vous publiez le service Web, dans les champs **URL OData** et **URL SOAP**, vous pouvez voir les URL générées pour le service Web.</span><span class="sxs-lookup"><span data-stu-id="867b1-121">When you publish the web service, in the **OData URL** and **SOAP URL** fields, you can see the URLs that are generated for the web service.</span></span> <span data-ttu-id="867b1-122">Vous pouvez tester le service Web immédiatement en choisissant les liens figurant dans les champs **URL OData** et **URL SOAP**.</span><span class="sxs-lookup"><span data-stu-id="867b1-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span></span> <span data-ttu-id="867b1-123">Éventuellement, vous pouvez copier la valeur du champ et pour l'enregistrer pour une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="867b1-123">Optionally, you can copy the value of the field and save it for later use.</span></span>  

<span data-ttu-id="867b1-124">Une fois le service Web publié, il est accessible aux parties externes.</span><span class="sxs-lookup"><span data-stu-id="867b1-124">After you publish a web service, it is available to external parties.</span></span> <span data-ttu-id="867b1-125">Vous pouvez vérifier la disponibilité de ce service Web à l'aide d'un navigateur, ou vous pouvez sélectionner le lien dans les champs **URL OData** et **URL SOAP** de la fenêtre **Services Web**.</span><span class="sxs-lookup"><span data-stu-id="867b1-125">You can verify the availability of that web service by using a browser, or you can choose the link in the **OData URL** and **SOAP URL** fields in the **Web Services** window.</span></span> <span data-ttu-id="867b1-126">La procédure suivante indique comment vous pouvez vérifier la disponibilité du service Web pour une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="867b1-126">The following procedure illustrates how you can verify the availability of the web service for later use.</span></span>  

#### <a name="to-verify-the-availability-of-a-web-service"></a><span data-ttu-id="867b1-127">Vérification de la disponibilité d'un service Web</span><span class="sxs-lookup"><span data-stu-id="867b1-127">To verify the availability of a web service</span></span>  

1.  <span data-ttu-id="867b1-128">Dans votre navigateur, indiquez l'URL appropriée.</span><span class="sxs-lookup"><span data-stu-id="867b1-128">In your browser, enter the relevant URL.</span></span> <span data-ttu-id="867b1-129">Le tableau suivant présente les types d'URL champ que vous pouvez entrer.</span><span class="sxs-lookup"><span data-stu-id="867b1-129">The following table illustrates the types of URLs that you can enter.</span></span> <span data-ttu-id="867b1-130">Pour les services Web SOAP, utilisez le format suivant pour votre URI.</span><span class="sxs-lookup"><span data-stu-id="867b1-130">For SOAP web services, use the following format for your URI.</span></span>  

    <table>
    <tr>
    <th><span data-ttu-id="867b1-131">Type de service Web</span><span class="sxs-lookup"><span data-stu-id="867b1-131">Web service type</span></span></th>
    <th><span data-ttu-id="867b1-132">Syntaxe</span><span class="sxs-lookup"><span data-stu-id="867b1-132">Syntax</span></span></th>
    <th><span data-ttu-id="867b1-133">Exemple :</span><span class="sxs-lookup"><span data-stu-id="867b1-133">Example</span></span></th>
    </tr>
    <tr>
    <td><span data-ttu-id="867b1-134">SOAP</span><span class="sxs-lookup"><span data-stu-id="867b1-134">SOAP</span></span></td>
    <td><span data-ttu-id="867b1-135">https://*Server*:*SOAPWebServicePort*/*ServerInstance*/WS/*CompanyName*/salesDocuments/</span><span class="sxs-lookup"><span data-stu-id="867b1-135">https://*Server*:*SOAPWebServicePort*/*ServerInstance*/WS/*CompanyName*/salesDocuments/</span></span></td>
    <td><span data-ttu-id="867b1-136">https://mycompany.financials.dynamics.com:7047/MS/WS/MyCompany/Page/salesDocuments?tenant=mycompany.financials.dynamics.com</span><span class="sxs-lookup"><span data-stu-id="867b1-136">https://mycompany.financials.dynamics.com:7047/MS/WS/MyCompany/Page/salesDocuments?tenant=mycompany.financials.dynamics.com</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="867b1-137">OData</span><span class="sxs-lookup"><span data-stu-id="867b1-137">OData</span></span></td>
    <td><span data-ttu-id="867b1-138">https://*Server*:*ODataWebServicePort*/*ServerInstance*/OData/Company('*CompanyName*')</span><span class="sxs-lookup"><span data-stu-id="867b1-138">https://*Server*:*ODataWebServicePort*/*ServerInstance*/OData/Company('*CompanyName*')</span></span></td>
    <td><span data-ttu-id="867b1-139">https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com</span><span class="sxs-lookup"><span data-stu-id="867b1-139">https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com</span></span>

         The company name is case-sensitive.</td>
    </tr>
    </table>

2.  <span data-ttu-id="867b1-140">Examinez les informations affichées dans le navigateur.</span><span class="sxs-lookup"><span data-stu-id="867b1-140">Review the information that is displayed in the browser.</span></span> <span data-ttu-id="867b1-141">Vérifiez que vous pouvez visualiser le nom du service Web que vous avez créé.</span><span class="sxs-lookup"><span data-stu-id="867b1-141">Verify that you can see the name of the web service that you have created.</span></span>  

 <span data-ttu-id="867b1-142">Lorsque vous accédez à un service Web, et que vous souhaitez copier des données vers [!INCLUDE[d365fin](includes/d365fin_md.md)], vous devez spécifier le nom de la société.</span><span class="sxs-lookup"><span data-stu-id="867b1-142">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span></span> <span data-ttu-id="867b1-143">Vous pouvez spécifier la société en tant que membre de l'URI comme l'indiquent les exemples, ou vous pouvez spécifier la société comme partie des paramètres de requête.</span><span class="sxs-lookup"><span data-stu-id="867b1-143">You can specify the company as part of the URI as shown in the examples, or you can specify the company as part of the query parameters.</span></span> <span data-ttu-id="867b1-144">Par exemple, les URI suivants pointent vers le même service Web OData et qu'ils sont tous deux des URI valides.</span><span class="sxs-lookup"><span data-stu-id="867b1-144">For example, the following URIs point to the same OData web service and are both valid URIs.</span></span>  

```  
https://localhost:7048/server/OData/Company('CRONUS International Ltd.')/Customer  
```  

```  
https://localhost:7048/server/OData/Customer?company='CRONUS International Ltd.'  
```  

## <a name="see-also"></a><span data-ttu-id="867b1-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="867b1-145">See Also</span></span>  
[<span data-ttu-id="867b1-146">Configuration et administration dans Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="867b1-146">Setup and Administration in Dynamics 365 for Financials</span></span>](admin-setup-and-administration.md)  
