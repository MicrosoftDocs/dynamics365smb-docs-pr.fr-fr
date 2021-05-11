---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7ead218d289668d893a659f730a4c64e31195f10
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788539"
---
<span data-ttu-id="456e5-101">Lorsque vous saisissez les dates/heures, qui sont une date et heure combinées en un champ, vous devez saisir un espace entre la date et l’heure.</span><span class="sxs-lookup"><span data-stu-id="456e5-101">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span></span> <span data-ttu-id="456e5-102">La partie de la date ne peut contenir des espaces sous forme de séparateur de date officiel de vos paramètres de région.</span><span class="sxs-lookup"><span data-stu-id="456e5-102">The date part can only contain spaces in the form of the official date separator of your region settings.</span></span> <span data-ttu-id="456e5-103">L’heure peut contenir des espaces autour de l’indicateur AM/PM dans les paramètres régionaux correspondants.</span><span class="sxs-lookup"><span data-stu-id="456e5-103">The time can contain spaces around the AM/PM indicator in relevant regional settings.</span></span>

<!--It is also possible to enter only a date in a datetime field, but it is not possible to enter only a time.-->

<span data-ttu-id="456e5-104">Le tableau suivant répertorie les différents formats de saisie possibles pour les dates/heures, ainsi que leur interprétation.</span><span class="sxs-lookup"><span data-stu-id="456e5-104">The following table lists the various ways in which you can enter datetimes and how they're interpreted.</span></span>  

|<span data-ttu-id="456e5-105">Écriture</span><span class="sxs-lookup"><span data-stu-id="456e5-105">Entry</span></span>|<span data-ttu-id="456e5-106">Interprétation</span><span class="sxs-lookup"><span data-stu-id="456e5-106">Interpretation</span></span>|
|---------------|------------------------|
|<span data-ttu-id="456e5-107">08-01-2022 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="456e5-107">08-01-2022 05:48:12 PM</span></span>|<span data-ttu-id="456e5-108">08\-01\-2022 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="456e5-108">08\-01\-2022 05:48:12 PM</span></span>|
|<span data-ttu-id="456e5-109">131222 132455</span><span class="sxs-lookup"><span data-stu-id="456e5-109">131222 132455</span></span>|<span data-ttu-id="456e5-110">13-12-22 13:24:55</span><span class="sxs-lookup"><span data-stu-id="456e5-110">13-12-22 13:24:55</span></span>|
|<span data-ttu-id="456e5-111">1-12-22 10</span><span class="sxs-lookup"><span data-stu-id="456e5-111">1-12-22 10</span></span>|<span data-ttu-id="456e5-112">01-12-22 10:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-112">01-12-22 10:00:00</span></span>|
|<span data-ttu-id="456e5-113">1.12.22 5</span><span class="sxs-lookup"><span data-stu-id="456e5-113">1.12.22 5</span></span>|<span data-ttu-id="456e5-114">01-12-22 05:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-114">01-12-22 05:00:00</span></span>|
|<span data-ttu-id="456e5-115">1.12.22</span><span class="sxs-lookup"><span data-stu-id="456e5-115">1.12.22</span></span>|<span data-ttu-id="456e5-116">01-12-22 00:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-116">01-12-22 00:00:00</span></span>|
|<span data-ttu-id="456e5-117">11 12</span><span class="sxs-lookup"><span data-stu-id="456e5-117">11 12</span></span>|<span data-ttu-id="456e5-118">11/mois en cours/année en cours 12:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-118">11-current month-current year 12:00:00</span></span>|
|<span data-ttu-id="456e5-119">1112 12</span><span class="sxs-lookup"><span data-stu-id="456e5-119">1112 12</span></span>|<span data-ttu-id="456e5-120">11/12/année en cours 12:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-120">11-12-current year 12:00:00</span></span>|
|<span data-ttu-id="456e5-121">a ou date du jour</span><span class="sxs-lookup"><span data-stu-id="456e5-121">t or today</span></span>|<span data-ttu-id="456e5-122">date du jour 00:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-122">today's date 00:00:00</span></span>|
|<span data-ttu-id="456e5-123">heure h</span><span class="sxs-lookup"><span data-stu-id="456e5-123">t time</span></span>|<span data-ttu-id="456e5-124">date du jour heure réelle</span><span class="sxs-lookup"><span data-stu-id="456e5-124">today's date actual time</span></span>|
|<span data-ttu-id="456e5-125">a 10:30</span><span class="sxs-lookup"><span data-stu-id="456e5-125">t 10:30</span></span>|<span data-ttu-id="456e5-126">date du jour 10:30:00</span><span class="sxs-lookup"><span data-stu-id="456e5-126">today's date 10:30:00</span></span>|
|<span data-ttu-id="456e5-127">a 3:3:3</span><span class="sxs-lookup"><span data-stu-id="456e5-127">t 3:3:3</span></span>|<span data-ttu-id="456e5-128">date du jour 03:03:03</span><span class="sxs-lookup"><span data-stu-id="456e5-128">today's date 03:03:03</span></span>|
|<span data-ttu-id="456e5-129">t ou date de travail</span><span class="sxs-lookup"><span data-stu-id="456e5-129">w or workdate</span></span>|<span data-ttu-id="456e5-130">date de travail 00:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-130">the working date 00:00:00</span></span>|
|<span data-ttu-id="456e5-131">lu ou lundi</span><span class="sxs-lookup"><span data-stu-id="456e5-131">m or Monday</span></span>|<span data-ttu-id="456e5-132">Lundi de la semaine en cours 00:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-132">Monday of the current week 00:00:00</span></span>|
|<span data-ttu-id="456e5-133">ma ou mardi</span><span class="sxs-lookup"><span data-stu-id="456e5-133">tu or Tuesday</span></span>|<span data-ttu-id="456e5-134">Mardi de la semaine en cours 00:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-134">Tuesday of the current week 00:00:00</span></span>|
|<span data-ttu-id="456e5-135">me ou mercredi</span><span class="sxs-lookup"><span data-stu-id="456e5-135">we or Wednesday</span></span>|<span data-ttu-id="456e5-136">Mercredi de la semaine en cours 00:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-136">Wednesday of the current week 00:00:00</span></span>|
|<span data-ttu-id="456e5-137">je ou jeudi</span><span class="sxs-lookup"><span data-stu-id="456e5-137">th or Thursday</span></span>|<span data-ttu-id="456e5-138">Jeudi de la semaine en cours 00:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-138">Thursday of the current week 00:00:00</span></span>|
|<span data-ttu-id="456e5-139">ve ou vendredi</span><span class="sxs-lookup"><span data-stu-id="456e5-139">f or Friday</span></span>|<span data-ttu-id="456e5-140">Vendredi de la semaine en cours 00:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-140">Friday of the current week 00:00:00</span></span>|
|<span data-ttu-id="456e5-141">sa ou samedi</span><span class="sxs-lookup"><span data-stu-id="456e5-141">s or Saturday</span></span>|<span data-ttu-id="456e5-142">Samedi de la semaine en cours 00:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-142">Saturday of the current week 00:00:00</span></span>|
|<span data-ttu-id="456e5-143">di ou dimanche</span><span class="sxs-lookup"><span data-stu-id="456e5-143">su or Sunday</span></span>|<span data-ttu-id="456e5-144">Dimanche de la semaine en cours 00:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-144">Sunday of the current week 00:00:00</span></span>|
|<span data-ttu-id="456e5-145">ma 10:30</span><span class="sxs-lookup"><span data-stu-id="456e5-145">tu 10:30</span></span>|<span data-ttu-id="456e5-146">Mardi de la semaine en cours 10:30:00</span><span class="sxs-lookup"><span data-stu-id="456e5-146">Tuesday of the current week 10:30:00</span></span>|
|<span data-ttu-id="456e5-147">ma 3:3:3</span><span class="sxs-lookup"><span data-stu-id="456e5-147">tu 3:3:3</span></span>|<span data-ttu-id="456e5-148">Mardi de la semaine en cours 03:03:03</span><span class="sxs-lookup"><span data-stu-id="456e5-148">Tuesday of the current week 03:03:03</span></span>|
|<span data-ttu-id="456e5-149">m23 a</span><span class="sxs-lookup"><span data-stu-id="456e5-149">t23 t</span></span>|<span data-ttu-id="456e5-150">Mardi de la semaine 23 de l’année de date de travail, heure actuelle</span><span class="sxs-lookup"><span data-stu-id="456e5-150">Tuesday of week 23 of the work date year, current time of day</span></span>|
|<span data-ttu-id="456e5-151">m23</span><span class="sxs-lookup"><span data-stu-id="456e5-151">t23</span></span>|<span data-ttu-id="456e5-152">Mardi de la semaine 23 de l’année de date de travail</span><span class="sxs-lookup"><span data-stu-id="456e5-152">Tuesday of week 23 of the work date year</span></span>|
|<span data-ttu-id="456e5-153">m 23</span><span class="sxs-lookup"><span data-stu-id="456e5-153">t 23</span></span>|<span data-ttu-id="456e5-154">Aujourd’hui 23:00:00</span><span class="sxs-lookup"><span data-stu-id="456e5-154">Today 23:00:00</span></span>|
|<span data-ttu-id="456e5-155">m-1</span><span class="sxs-lookup"><span data-stu-id="456e5-155">t-1</span></span>|<span data-ttu-id="456e5-156">Mardi de la semaine 1 de l’année de date de travail</span><span class="sxs-lookup"><span data-stu-id="456e5-156">Tuesday of week 1 of the work date year</span></span>|

