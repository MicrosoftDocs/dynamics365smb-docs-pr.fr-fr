---
title: "Planification d'un état à exécuter à une date et une heure spécifiques | Microsoft Docs"
description: "En savoir plus sur l'entrée d'un état dans une file d'attente de projets et la planification de son traitement à une date et à une heure spécifiques."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: task, process, report
ms.date: 07/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: badcdee3dfa5bec3c2462149989cf9d4fb5af2a0
ms.contentlocale: fr-fr
ms.lasthandoff: 09/22/2017

---
# <a name="working-with-reports"></a><span data-ttu-id="6fafb-103">Utilisation des états</span><span class="sxs-lookup"><span data-stu-id="6fafb-103">Working with Reports</span></span>
<span data-ttu-id="6fafb-104">Un état regroupe des informations en fonction d'un ensemble de critères spécifié, et organise et présente les informations dans un format imprimable et facilement lisible.</span><span class="sxs-lookup"><span data-stu-id="6fafb-104">A report gathers information based on a specified set of criteria, and organizes and presents the information in an easy-to-read, printable format.</span></span> <span data-ttu-id="6fafb-105">Il existe de nombreux états accessibles tout au long de l'application.</span><span class="sxs-lookup"><span data-stu-id="6fafb-105">There are many reports that you can access throughout the application.</span></span> <span data-ttu-id="6fafb-106">Les états fournissent généralement des informations relatives au contexte de la page où vous vous trouvez.</span><span class="sxs-lookup"><span data-stu-id="6fafb-106">The reports typically provide information relative to the context of the page you are on.</span></span> <span data-ttu-id="6fafb-107">Par exemple, la page **Client** comprend des états pour les 10 principaux clients et les statistiques de vente, et plus encore.</span><span class="sxs-lookup"><span data-stu-id="6fafb-107">For example, the **Customer** page includes reports for the top 10 customers and the sales statistics, and more.</span></span>

<span data-ttu-id="6fafb-108">Vous pouvez rechercher des états dans l'onglet **États** des pages sélectionnées, ou vous pouvez utiliser la recherche pour rechercher des états par leur nom.</span><span class="sxs-lookup"><span data-stu-id="6fafb-108">You can find reports in the **Reports** tab on selected pages, or you can use search to find reports by name.</span></span> <span data-ttu-id="6fafb-109">Lorsque vous ouvrez un état, vous voyez d'abord une page qui vous permet de spécifier des informations (des options et des filtres) qui déterminent ce que vous souhaitez inclure dans l'état.</span><span class="sxs-lookup"><span data-stu-id="6fafb-109">When you open a report, you are presented with a page that let's you specify information (options and filters) that determines want to include in the report.</span></span> <span data-ttu-id="6fafb-110">Par exemple, selon l'état, vous pouvez spécifier une plage de dates, un enregistrement particulier tel qu'un client, ou effectuer un tri.</span><span class="sxs-lookup"><span data-stu-id="6fafb-110">For example, depending on the report, you can specify a date range, a specific record such as a customer, or sorting order.</span></span>

## <a name="previewing-a-report"></a><span data-ttu-id="6fafb-111">Affichage de l'aperçu d'un état</span><span class="sxs-lookup"><span data-stu-id="6fafb-111">Previewing a report</span></span>
<span data-ttu-id="6fafb-112">Sélectionnez **Aperçu** pour visualiser l'état dans le navigateur Internet.</span><span class="sxs-lookup"><span data-stu-id="6fafb-112">Choose **Preview** to see the report in the Internet browser.</span></span> <span data-ttu-id="6fafb-113">Pointez une zone de l'état pour afficher la barre de menu.</span><span class="sxs-lookup"><span data-stu-id="6fafb-113">Point to an area of the report to show the menu bar.</span></span>  

<span data-ttu-id="6fafb-114">![Barre d'outils Aperçu de l'état](media/report_viewer.png "Barre d'outils Aperçu de l'état").</span><span class="sxs-lookup"><span data-stu-id="6fafb-114">![Report preview toolbar](media/report_viewer.png "Report preview toolbar").</span></span>

<span data-ttu-id="6fafb-115">Utilisez la barre de menus pour :</span><span class="sxs-lookup"><span data-stu-id="6fafb-115">Use the menu bar to:</span></span>

-   <span data-ttu-id="6fafb-116">Naviguer entre les pages</span><span class="sxs-lookup"><span data-stu-id="6fafb-116">Move through pages</span></span>
-   <span data-ttu-id="6fafb-117">Effectuer un zoom avant et arrière</span><span class="sxs-lookup"><span data-stu-id="6fafb-117">Zoom in and out</span></span>
-   <span data-ttu-id="6fafb-118">Redimensionner à la taille de la fenêtre</span><span class="sxs-lookup"><span data-stu-id="6fafb-118">Resize to fit the window</span></span>
-   <span data-ttu-id="6fafb-119">Sélectionner du texte</span><span class="sxs-lookup"><span data-stu-id="6fafb-119">Select text</span></span>

    <span data-ttu-id="6fafb-120">Vous pouvez copier le texte d'un état puis le coller ailleurs, comme dans une page de [!INCLUDE[d365fin](includes/d365fin_md.md)] ou Microsoft Word.</span><span class="sxs-lookup"><span data-stu-id="6fafb-120">You can copy text from a report, and then paste it somewhere else, like a page in [!INCLUDE[d365fin](includes/d365fin_md.md)] or Microsoft Word.</span></span>  <span data-ttu-id="6fafb-121">Avec la souris, par exemple, appuyez et maintenez la pression là où vous souhaitez démarrer, puis déplacez la souris pour sélectionner un ou plusieurs mots, phrases ou paragraphes.</span><span class="sxs-lookup"><span data-stu-id="6fafb-121">Using a mouse, for example, you press and hold where you want to start, and then move the mouse to select one or more words, sentences, or paragraphs.</span></span> <span data-ttu-id="6fafb-122">Vous pouvez ensuite appuyer sur le bouton droit de la souris et sélectionner **Copier**.</span><span class="sxs-lookup"><span data-stu-id="6fafb-122">You can then press the right mouse button, and select **Copy**.</span></span> <span data-ttu-id="6fafb-123">Vous pouvez coller le texte sélectionné partout où vous le souhaitez.</span><span class="sxs-lookup"><span data-stu-id="6fafb-123">You can the paste the selected text where ever you want it.</span></span>
-   <span data-ttu-id="6fafb-124">Faire défiler le document</span><span class="sxs-lookup"><span data-stu-id="6fafb-124">Pan the document</span></span>

    <span data-ttu-id="6fafb-125">Vous pouvez déplacer la zone visible de l'état dans n'importe quelle direction de manière voir d'autres zones ou l'état.</span><span class="sxs-lookup"><span data-stu-id="6fafb-125">You can move the visible area of the report in any direction so you can view other areas or the report.</span></span> <span data-ttu-id="6fafb-126">Ceci est utile si vous avez effectué un zoom pour observer les détails.</span><span class="sxs-lookup"><span data-stu-id="6fafb-126">This is helpful when you have zoomed in to see details.</span></span>  <span data-ttu-id="6fafb-127">Avec la souris, par exemple, appuyez et maintenez la pression n'importe où dans l'aperçu de l'état, puis déplacez la souris.</span><span class="sxs-lookup"><span data-stu-id="6fafb-127">Using your mouse, for example, press and hold the mouse button anywhere in the report preview, and then move your mouse.</span></span>

-   <span data-ttu-id="6fafb-128">Téléchargez un fichier PDF sur votre ordinateur ou votre réseau.</span><span class="sxs-lookup"><span data-stu-id="6fafb-128">Download to a PDF file on your computer or network.</span></span>


## <a name="saving-a-report"></a><span data-ttu-id="6fafb-129">Enregistrement d'un état</span><span class="sxs-lookup"><span data-stu-id="6fafb-129">Saving a Report</span></span>
<span data-ttu-id="6fafb-130">Vous pouvez enregistrer un état dans un document PDF, un document Microsoft Word ou un document Microsoft Excel en sélectionnant **Envoyer à**, puis en effectuant votre sélection.</span><span class="sxs-lookup"><span data-stu-id="6fafb-130">You can save a report to a PDF document, Microsoft Word document, or Microsoft Excel document by choosing **Send to**, and then making your selection.</span></span> 

## <span data-ttu-id="6fafb-131"><a name="ScheduleReport"></a> Planification d'un état à exécuter</span><span class="sxs-lookup"><span data-stu-id="6fafb-131"><a name="ScheduleReport"></a> Scheduling a Report to Run</span></span>
<span data-ttu-id="6fafb-132">Vous pouvez planifier un état à exécuter à une date et une heure spécifiques.</span><span class="sxs-lookup"><span data-stu-id="6fafb-132">You can schedule a report to run at a specific date and time.</span></span> <span data-ttu-id="6fafb-133">Les états prévus sont entrés dans la file projets et traités au moment prévu, comme les autres projets.</span><span class="sxs-lookup"><span data-stu-id="6fafb-133">Scheduled reports are entered in the job queue and processed at the scheduled time, similar to other jobs.</span></span> <span data-ttu-id="6fafb-134">Vous pouvez choisir de sauvegarder l'état traité dans un fichier, par exemple, Excel, Word ou PDF, de l'imprimer sur une imprimante sélectionnée ou de traiter l'état uniquement.</span><span class="sxs-lookup"><span data-stu-id="6fafb-134">You can choose to save the processed report to a file, such as an Excel, Word, or PDF, print it to a selected printer, or process the report only.</span></span> <span data-ttu-id="6fafb-135">Si vous choisissez d'enregistrer l'état dans un fichier, alors l'état traité est envoyé à la **Boîte de réception état** de votre page d'accueil, dans laquelle vous pouvez l'afficher.</span><span class="sxs-lookup"><span data-stu-id="6fafb-135">If you choose to save the report to a file, then the processed report is sent to the **Report Inbox** area on your Home page, where you can view it.</span></span>

<span data-ttu-id="6fafb-136">Vous pouvez planifier un état lorsque vous l'ouvrez.</span><span class="sxs-lookup"><span data-stu-id="6fafb-136">You can schedule a report when you open a report.</span></span> <span data-ttu-id="6fafb-137">Vous devez sélectionner **Planifier** et entrer des informations telles que l'imprimante, ainsi que la date et l'heure.</span><span class="sxs-lookup"><span data-stu-id="6fafb-137">You choose the **Schedule** action and then you enter information such as printer, and time and date.</span></span> <span data-ttu-id="6fafb-138">L'état est alors ajouté à la file d'attente des travaux et sera exécuté au moment spécifié.</span><span class="sxs-lookup"><span data-stu-id="6fafb-138">The report is then added to the job queue and will be run at the specified time.</span></span> <span data-ttu-id="6fafb-139">Lorsque l'état a été traité, l'article est supprimé de la file projets.</span><span class="sxs-lookup"><span data-stu-id="6fafb-139">When the report is processed, the item will be removed from the job queue.</span></span> <span data-ttu-id="6fafb-140">Si vous avez enregistré l'état traité dans un fichier, il est disponible dans la **Boîte de réception état**.</span><span class="sxs-lookup"><span data-stu-id="6fafb-140">If you saved the processed report to a file, it will be available in the **Report Inbox** area.</span></span>

## <span data-ttu-id="6fafb-141"><a name="PrintReport"></a>Impression d'un état</span><span class="sxs-lookup"><span data-stu-id="6fafb-141"><a name="PrintReport"></a>Printing a Report</span></span>
<span data-ttu-id="6fafb-142">Si vous souhaitez imprimer un état, vous devez d'abord le télécharger en tant document PDF, Word ou Excel en choisissant le bouton **Envoyer à**.</span><span class="sxs-lookup"><span data-stu-id="6fafb-142">When you want to print a report you have to download the report as a PDF, Word, or Excel document first by choosing **Send to**.</span></span> <span data-ttu-id="6fafb-143">À présent, vous pouvez soit ouvrir l'état directement et l'imprimer, ou l'enregistrer et l'imprimer plus tard.</span><span class="sxs-lookup"><span data-stu-id="6fafb-143">Now, you can either open the report document right-away and print it, or save it and print it later.</span></span>

## <a name="using-saved-settings"></a><span data-ttu-id="6fafb-144">Utilisation des paramètres enregistrés</span><span class="sxs-lookup"><span data-stu-id="6fafb-144">Using Saved Settings</span></span>
<span data-ttu-id="6fafb-145">Un état peut inclure une ou plusieurs écritures dans la zone **Paramètres enregistrés**.</span><span class="sxs-lookup"><span data-stu-id="6fafb-145">A report can include one or more entries in the **Saved Settings** box.</span></span> <span data-ttu-id="6fafb-146">Les *Paramètres enregistrés* sont fondamentalement un groupe d'options et de filtres prédéfini que vous pouvez appliquer à l'état avant d'en afficher un aperçu ou de l'envoyer vers un fichier.</span><span class="sxs-lookup"><span data-stu-id="6fafb-146">*Saved settings* are basically a predefined group of options and filters that you can apply to the report before previewing or sending the report to a file.</span></span> <span data-ttu-id="6fafb-147">Le fait d'utiliser les paramètres enregistrés est une façon rapide et fiable de générer de façon cohérente des états qui contiennent les données adéquates.</span><span class="sxs-lookup"><span data-stu-id="6fafb-147">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span></span>

<span data-ttu-id="6fafb-148">L'écriture de paramètres enregistrés appelée **Options et filtres récemment utilisés** est toujours disponible.</span><span class="sxs-lookup"><span data-stu-id="6fafb-148">The saved settings entry called **Last used options and filters** is always available.</span></span> <span data-ttu-id="6fafb-149">Cette écriture permet de faire en sorte que l'état utilise les options et les filtres qui ont été utilisés la dernière fois que vous l'avez regardé.</span><span class="sxs-lookup"><span data-stu-id="6fafb-149">This entry sets the report to use options and filters that were used the last time you looked at the report.</span></span>

>[!NOTE]
><span data-ttu-id="6fafb-150">En tant qu'administrateur, vous pouvez créer et gérer les paramètres enregistrés pour les états pour tous les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="6fafb-150">As an administrator, you can create and manage the saved settings for reports for all users.</span></span> <span data-ttu-id="6fafb-151">Pour plus d'informations, voir [Gestion des paramètres enregistrés dans les états](reports-saving-reusing-settings.md).</span><span class="sxs-lookup"><span data-stu-id="6fafb-151">For more information, see [Managing Saved Settings on Reports](reports-saving-reusing-settings.md).</span></span>

## <a name="changing-the-layout-and-look-of-a-report"></a><span data-ttu-id="6fafb-152">Modification de la présentation et de l'apparence d'un état</span><span class="sxs-lookup"><span data-stu-id="6fafb-152">Changing the layout and look of a report</span></span>
<span data-ttu-id="6fafb-153">Une présentation d'état contrôle les éléments affichés sur un état, leur agencement et leur mise en forme.</span><span class="sxs-lookup"><span data-stu-id="6fafb-153">A report layout controls what is shown on a report, how it is arranged, and how it is styled.</span></span> <span data-ttu-id="6fafb-154">Si vous souhaitez changer de présentation, voir [Procédure : modification de la présentation actuellement utilisée sur un rapport](ui-how-change-layout-currently-used-report.md).</span><span class="sxs-lookup"><span data-stu-id="6fafb-154">If you want to switch to a different layout, see [How to: Change Which Layout is Currently Used on a Report](ui-how-change-layout-currently-used-report.md).</span></span> <span data-ttu-id="6fafb-155">Ou, si vous souhaitez personnaliser votre propre présentation d'état, voir [Procédure : créer et modifier une présentation de rapport personnalisée](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="6fafb-155">Or, if you want to customize your own report layout, see [How to: Create and Modify a Custom Report Layout](ui-how-create-custom-report-layout.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="6fafb-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6fafb-156">See Also</span></span>
[<span data-ttu-id="6fafb-157">Spécifier la sélection de l'imprimante pour les états</span><span class="sxs-lookup"><span data-stu-id="6fafb-157">Specify Printer Selection for Reports</span></span>](ui-specify-printer-selection-reports.md)  
[<span data-ttu-id="6fafb-158">Gestion des présentations de rapport et de document</span><span class="sxs-lookup"><span data-stu-id="6fafb-158">Managing Report and Document Layouts</span></span>](ui-manage-report-layouts.md)  
<span data-ttu-id="6fafb-159">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6fafb-159">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
