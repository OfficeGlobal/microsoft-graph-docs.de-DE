---
title: Ressourcentyp dateTimeTimeZone
description: Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.
localization_priority: Normal
ms.openlocfilehash: ee5359c0ababad2a4f785d17a02ac5bb618d2681
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057043"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="f1f73-103">Ressourcentyp dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f1f73-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1f73-104">Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.</span><span class="sxs-lookup"><span data-stu-id="f1f73-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="f1f73-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f1f73-105">Properties</span></span>
| <span data-ttu-id="f1f73-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1f73-106">Property</span></span>     | <span data-ttu-id="f1f73-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f1f73-107">Type</span></span>   |<span data-ttu-id="f1f73-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1f73-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1f73-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="f1f73-109">dateTime</span></span>|<span data-ttu-id="f1f73-110">String</span><span class="sxs-lookup"><span data-stu-id="f1f73-110">String</span></span>|<span data-ttu-id="f1f73-111">Ein bestimmter Zeitpunkt in einer kombinierten Datums- und Uhrzeitsdarstellung (`{date}T{time}`).</span><span class="sxs-lookup"><span data-stu-id="f1f73-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="f1f73-112">Beispielsweise "2019-04-16T09:00:00".</span><span class="sxs-lookup"><span data-stu-id="f1f73-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="f1f73-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="f1f73-113">timeZone</span></span>|<span data-ttu-id="f1f73-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1f73-114">String</span></span>|<span data-ttu-id="f1f73-115">Ein Zeitzonenname, wie unten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="f1f73-115">A time zone name as described below.</span></span>|

<span data-ttu-id="f1f73-116">Die **TimeZone** -Eigenschaft kann auf eine der von Windows unterstützten Zeitzonen sowie die folgenden Zeitzonen-Namen festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="f1f73-116">The **timeZone** property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="f1f73-117">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="f1f73-117">Etc/GMT+12</span></span>

<span data-ttu-id="f1f73-118">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="f1f73-118">Etc/GMT+11</span></span>

<span data-ttu-id="f1f73-119">Pazifik/Honolulu</span><span class="sxs-lookup"><span data-stu-id="f1f73-119">Pacific/Honolulu</span></span>

<span data-ttu-id="f1f73-120">Amerika/Anchorage</span><span class="sxs-lookup"><span data-stu-id="f1f73-120">America/Anchorage</span></span>

<span data-ttu-id="f1f73-121">Amerika/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="f1f73-121">America/Santa_Isabel</span></span>

<span data-ttu-id="f1f73-122">Amerika/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="f1f73-122">America/Los_Angeles</span></span>

<span data-ttu-id="f1f73-123">Amerika/Phoenix</span><span class="sxs-lookup"><span data-stu-id="f1f73-123">America/Phoenix</span></span>

<span data-ttu-id="f1f73-124">Amerika/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="f1f73-124">America/Chihuahua</span></span>

<span data-ttu-id="f1f73-125">Amerika/Denver</span><span class="sxs-lookup"><span data-stu-id="f1f73-125">America/Denver</span></span>

<span data-ttu-id="f1f73-126">Amerika/Guatemala</span><span class="sxs-lookup"><span data-stu-id="f1f73-126">America/Guatemala</span></span>

<span data-ttu-id="f1f73-127">Amerika/Chicago</span><span class="sxs-lookup"><span data-stu-id="f1f73-127">America/Chicago</span></span>

<span data-ttu-id="f1f73-128">Amerika/Mexico_Stadt</span><span class="sxs-lookup"><span data-stu-id="f1f73-128">America/Mexico_City</span></span>

<span data-ttu-id="f1f73-129">Amerika/Regina</span><span class="sxs-lookup"><span data-stu-id="f1f73-129">America/Regina</span></span>

<span data-ttu-id="f1f73-130">Amerika/Bogota</span><span class="sxs-lookup"><span data-stu-id="f1f73-130">America/Bogota</span></span>

<span data-ttu-id="f1f73-131">Amerika/New_York</span><span class="sxs-lookup"><span data-stu-id="f1f73-131">America/New_York</span></span>

<span data-ttu-id="f1f73-132">Amerika/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="f1f73-132">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="f1f73-133">Amerika/Caracas</span><span class="sxs-lookup"><span data-stu-id="f1f73-133">America/Caracas</span></span>

<span data-ttu-id="f1f73-134">Amerika/Asuncion</span><span class="sxs-lookup"><span data-stu-id="f1f73-134">America/Asuncion</span></span>

<span data-ttu-id="f1f73-135">Amerika/Halifax</span><span class="sxs-lookup"><span data-stu-id="f1f73-135">America/Halifax</span></span>

<span data-ttu-id="f1f73-136">Amerika/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="f1f73-136">America/Cuiaba</span></span>

<span data-ttu-id="f1f73-137">Amerika/La_Paz</span><span class="sxs-lookup"><span data-stu-id="f1f73-137">America/La_Paz</span></span>

<span data-ttu-id="f1f73-138">Amerika/Santiago</span><span class="sxs-lookup"><span data-stu-id="f1f73-138">America/Santiago</span></span>

<span data-ttu-id="f1f73-139">Amerika/St_Johns</span><span class="sxs-lookup"><span data-stu-id="f1f73-139">America/St_Johns</span></span>

<span data-ttu-id="f1f73-140">Amerika/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="f1f73-140">America/Sao_Paulo</span></span>

<span data-ttu-id="f1f73-141">Amerika/Argentinien/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="f1f73-141">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="f1f73-142">Amerika/Cayenne</span><span class="sxs-lookup"><span data-stu-id="f1f73-142">America/Cayenne</span></span>

<span data-ttu-id="f1f73-143">Amerika/Godthab</span><span class="sxs-lookup"><span data-stu-id="f1f73-143">America/Godthab</span></span>

<span data-ttu-id="f1f73-144">Amerika/Montevideo</span><span class="sxs-lookup"><span data-stu-id="f1f73-144">America/Montevideo</span></span>

<span data-ttu-id="f1f73-145">Amerika/Bahia</span><span class="sxs-lookup"><span data-stu-id="f1f73-145">America/Bahia</span></span>

<span data-ttu-id="f1f73-146">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="f1f73-146">Etc/GMT+2</span></span>

<span data-ttu-id="f1f73-147">Atlantik/Azoren</span><span class="sxs-lookup"><span data-stu-id="f1f73-147">Atlantic/Azores</span></span>

<span data-ttu-id="f1f73-148">Atlantik/Kap_Verde</span><span class="sxs-lookup"><span data-stu-id="f1f73-148">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="f1f73-149">Afrika/Casablanca</span><span class="sxs-lookup"><span data-stu-id="f1f73-149">Africa/Casablanca</span></span>

<span data-ttu-id="f1f73-150">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="f1f73-150">Etc/GMT</span></span>

<span data-ttu-id="f1f73-151">Europa/London</span><span class="sxs-lookup"><span data-stu-id="f1f73-151">Europe/London</span></span>

<span data-ttu-id="f1f73-152">Atlantik/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="f1f73-152">Atlantic/Reykjavik</span></span>

<span data-ttu-id="f1f73-153">Europa/Berlin</span><span class="sxs-lookup"><span data-stu-id="f1f73-153">Europe/Berlin</span></span>

<span data-ttu-id="f1f73-154">Europa/Budapest</span><span class="sxs-lookup"><span data-stu-id="f1f73-154">Europe/Budapest</span></span>

<span data-ttu-id="f1f73-155">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="f1f73-155">Europe/Paris</span></span>

<span data-ttu-id="f1f73-156">Europa/Warschau</span><span class="sxs-lookup"><span data-stu-id="f1f73-156">Europe/Warsaw</span></span>

<span data-ttu-id="f1f73-157">Afrika/Lagos</span><span class="sxs-lookup"><span data-stu-id="f1f73-157">Africa/Lagos</span></span>

<span data-ttu-id="f1f73-158">Afrika/Windhoek</span><span class="sxs-lookup"><span data-stu-id="f1f73-158">Africa/Windhoek</span></span>

<span data-ttu-id="f1f73-159">Europa/Bukarest</span><span class="sxs-lookup"><span data-stu-id="f1f73-159">Europe/Bucharest</span></span>

<span data-ttu-id="f1f73-160">Asien/Beirut</span><span class="sxs-lookup"><span data-stu-id="f1f73-160">Asia/Beirut</span></span>

<span data-ttu-id="f1f73-161">Afrika/Kairo</span><span class="sxs-lookup"><span data-stu-id="f1f73-161">Africa/Cairo</span></span>

<span data-ttu-id="f1f73-162">Asien/Damaskus</span><span class="sxs-lookup"><span data-stu-id="f1f73-162">Asia/Damascus</span></span>

<span data-ttu-id="f1f73-163">Afrika/Johannesburg</span><span class="sxs-lookup"><span data-stu-id="f1f73-163">Africa/Johannesburg</span></span>

<span data-ttu-id="f1f73-164">Europa/Kiew</span><span class="sxs-lookup"><span data-stu-id="f1f73-164">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="f1f73-165">Europa/Istanbul</span><span class="sxs-lookup"><span data-stu-id="f1f73-165">Europe/Istanbul</span></span>

<span data-ttu-id="f1f73-166">Asien/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="f1f73-166">Asia/Jerusalem</span></span>

<span data-ttu-id="f1f73-167">Asien/Amman</span><span class="sxs-lookup"><span data-stu-id="f1f73-167">Asia/Amman</span></span>

<span data-ttu-id="f1f73-168">Asien/Bagdad</span><span class="sxs-lookup"><span data-stu-id="f1f73-168">Asia/Baghdad</span></span>

<span data-ttu-id="f1f73-169">Europa/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="f1f73-169">Europe/Kaliningrad</span></span>

<span data-ttu-id="f1f73-170">Asien/Riad</span><span class="sxs-lookup"><span data-stu-id="f1f73-170">Asia/Riyadh</span></span>

<span data-ttu-id="f1f73-171">Afrika/Nairobi</span><span class="sxs-lookup"><span data-stu-id="f1f73-171">Africa/Nairobi</span></span>

<span data-ttu-id="f1f73-172">Asien/Teheran</span><span class="sxs-lookup"><span data-stu-id="f1f73-172">Asia/Tehran</span></span>

<span data-ttu-id="f1f73-173">Asien/Dubai</span><span class="sxs-lookup"><span data-stu-id="f1f73-173">Asia/Dubai</span></span>

<span data-ttu-id="f1f73-174">Asien/Baku</span><span class="sxs-lookup"><span data-stu-id="f1f73-174">Asia/Baku</span></span>

<span data-ttu-id="f1f73-175">Europa/Moskau</span><span class="sxs-lookup"><span data-stu-id="f1f73-175">Europe/Moscow</span></span>

<span data-ttu-id="f1f73-176">Indisch/Mauritius</span><span class="sxs-lookup"><span data-stu-id="f1f73-176">Indian/Mauritius</span></span>

<span data-ttu-id="f1f73-177">Asien/Tiflis</span><span class="sxs-lookup"><span data-stu-id="f1f73-177">Asia/Tbilisi</span></span>

<span data-ttu-id="f1f73-178">Asien/Eriwan</span><span class="sxs-lookup"><span data-stu-id="f1f73-178">Asia/Yerevan</span></span>

<span data-ttu-id="f1f73-179">Asien/Kabul</span><span class="sxs-lookup"><span data-stu-id="f1f73-179">Asia/Kabul</span></span>

<span data-ttu-id="f1f73-180">Asien/Karatschi</span><span class="sxs-lookup"><span data-stu-id="f1f73-180">Asia/Karachi</span></span>

<span data-ttu-id="f1f73-181">Asien/Taschkent</span><span class="sxs-lookup"><span data-stu-id="f1f73-181">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="f1f73-182">Asien/Kolkata</span><span class="sxs-lookup"><span data-stu-id="f1f73-182">Asia/Kolkata</span></span>

<span data-ttu-id="f1f73-183">Asien/Colombo</span><span class="sxs-lookup"><span data-stu-id="f1f73-183">Asia/Colombo</span></span>

<span data-ttu-id="f1f73-184">Asien/Katmandu</span><span class="sxs-lookup"><span data-stu-id="f1f73-184">Asia/Kathmandu</span></span>

<span data-ttu-id="f1f73-185">Asien/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="f1f73-185">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="f1f73-186">Asien/Dhaka</span><span class="sxs-lookup"><span data-stu-id="f1f73-186">Asia/Dhaka</span></span>

<span data-ttu-id="f1f73-187">Asien/Jekaterinburg</span><span class="sxs-lookup"><span data-stu-id="f1f73-187">Asia/Yekaterinburg</span></span>

<span data-ttu-id="f1f73-188">Asien/Yangon (Rangun)</span><span class="sxs-lookup"><span data-stu-id="f1f73-188">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="f1f73-189">Asien/Bangkok</span><span class="sxs-lookup"><span data-stu-id="f1f73-189">Asia/Bangkok</span></span>

<span data-ttu-id="f1f73-190">Asien/Nowosibirsk</span><span class="sxs-lookup"><span data-stu-id="f1f73-190">Asia/Novosibirsk</span></span>

<span data-ttu-id="f1f73-191">Asien/Shanghai</span><span class="sxs-lookup"><span data-stu-id="f1f73-191">Asia/Shanghai</span></span>

<span data-ttu-id="f1f73-192">Asien/Krasnojarsk</span><span class="sxs-lookup"><span data-stu-id="f1f73-192">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="f1f73-193">Asien/Singapur</span><span class="sxs-lookup"><span data-stu-id="f1f73-193">Asia/Singapore</span></span>

<span data-ttu-id="f1f73-194">Australien/Perth</span><span class="sxs-lookup"><span data-stu-id="f1f73-194">Australia/Perth</span></span>

<span data-ttu-id="f1f73-195">Asien/Taipeh</span><span class="sxs-lookup"><span data-stu-id="f1f73-195">Asia/Taipei</span></span>

<span data-ttu-id="f1f73-196">Asien/Ulan-Bator</span><span class="sxs-lookup"><span data-stu-id="f1f73-196">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="f1f73-197">Asien/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="f1f73-197">Asia/Irkutsk</span></span>

<span data-ttu-id="f1f73-198">Asien/Tokio</span><span class="sxs-lookup"><span data-stu-id="f1f73-198">Asia/Tokyo</span></span>

<span data-ttu-id="f1f73-199">Asien/Seoul</span><span class="sxs-lookup"><span data-stu-id="f1f73-199">Asia/Seoul</span></span>

<span data-ttu-id="f1f73-200">Australien/Adelaide</span><span class="sxs-lookup"><span data-stu-id="f1f73-200">Australia/Adelaide</span></span>

<span data-ttu-id="f1f73-201">Australien/Darwin</span><span class="sxs-lookup"><span data-stu-id="f1f73-201">Australia/Darwin</span></span>

<span data-ttu-id="f1f73-202">Australien/Brisbane</span><span class="sxs-lookup"><span data-stu-id="f1f73-202">Australia/Brisbane</span></span>

<span data-ttu-id="f1f73-203">Australien/Sydney</span><span class="sxs-lookup"><span data-stu-id="f1f73-203">Australia/Sydney</span></span>

<span data-ttu-id="f1f73-204">Pazifik/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="f1f73-204">Pacific/Port_Moresby</span></span>

<span data-ttu-id="f1f73-205">Australien/Hobart</span><span class="sxs-lookup"><span data-stu-id="f1f73-205">Australia/Hobart</span></span>

<span data-ttu-id="f1f73-206">Asien/Jakutsk</span><span class="sxs-lookup"><span data-stu-id="f1f73-206">Asia/Yakutsk</span></span>

<span data-ttu-id="f1f73-207">Pazifik/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="f1f73-207">Pacific/Guadalcanal</span></span>

<span data-ttu-id="f1f73-208">Asien/Wladiwostok</span><span class="sxs-lookup"><span data-stu-id="f1f73-208">Asia/Vladivostok</span></span>

<span data-ttu-id="f1f73-209">Pazifik/Auckland</span><span class="sxs-lookup"><span data-stu-id="f1f73-209">Pacific/Auckland</span></span>

<span data-ttu-id="f1f73-210">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="f1f73-210">Etc/GMT-12</span></span>

<span data-ttu-id="f1f73-211">Pazifik/Fidschi</span><span class="sxs-lookup"><span data-stu-id="f1f73-211">Pacific/Fiji</span></span>

<span data-ttu-id="f1f73-212">Asien/Magadan</span><span class="sxs-lookup"><span data-stu-id="f1f73-212">Asia/Magadan</span></span>

<span data-ttu-id="f1f73-213">Pazifik/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="f1f73-213">Pacific/Tongatapu</span></span>

<span data-ttu-id="f1f73-214">Pazifik/Apia</span><span class="sxs-lookup"><span data-stu-id="f1f73-214">Pacific/Apia</span></span>

<span data-ttu-id="f1f73-215">Pazifik/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="f1f73-215">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1f73-216">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f1f73-216">JSON representation</span></span>

<span data-ttu-id="f1f73-217">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f1f73-217">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dateTimeTimeZone"
}-->

```json
{
  "dateTime": "string",
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimetimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
