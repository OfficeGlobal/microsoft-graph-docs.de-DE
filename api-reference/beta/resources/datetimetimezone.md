---
title: Ressourcentyp dateTimeTimeZone
description: Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.
localization_priority: Normal
ms.openlocfilehash: 5090edce8d86ff12470cc1bb39f92ef13b42ba15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876069"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="9fb9f-103">Ressourcentyp dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9fb9f-103">dateTimeTimeZone resource type</span></span>

> <span data-ttu-id="9fb9f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9fb9f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fb9f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9fb9f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9fb9f-106">Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.</span><span class="sxs-lookup"><span data-stu-id="9fb9f-106">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="9fb9f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9fb9f-107">Properties</span></span>
| <span data-ttu-id="9fb9f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9fb9f-108">Property</span></span>     | <span data-ttu-id="9fb9f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9fb9f-109">Type</span></span>   |<span data-ttu-id="9fb9f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fb9f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fb9f-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="9fb9f-111">DateTime</span></span>|<span data-ttu-id="9fb9f-112">String</span><span class="sxs-lookup"><span data-stu-id="9fb9f-112">String</span></span>|<span data-ttu-id="9fb9f-113">Ein bestimmter Zeitpunkt in einer kombinierten Datums- und Uhrzeitsdarstellung (`<date>T<time>`).</span><span class="sxs-lookup"><span data-stu-id="9fb9f-113">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="9fb9f-114">TimeZone</span><span class="sxs-lookup"><span data-stu-id="9fb9f-114">TimeZone</span></span>|<span data-ttu-id="9fb9f-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9fb9f-115">String</span></span>|<span data-ttu-id="9fb9f-116">Einer der folgenden Zeitzonennamen.</span><span class="sxs-lookup"><span data-stu-id="9fb9f-116">One of the following time zone names.</span></span>|

<span data-ttu-id="9fb9f-117">Die Eigenschaft _TimeZone_ kann auf eine beliebige, von Windows unterstützte Zeitzone und auf einen der folgenden Zeitzonennamen eingestellt werden .</span><span class="sxs-lookup"><span data-stu-id="9fb9f-117">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="9fb9f-118">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="9fb9f-118">Etc/GMT+12</span></span>

<span data-ttu-id="9fb9f-119">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="9fb9f-119">Etc/GMT+11</span></span>

<span data-ttu-id="9fb9f-120">Pazifik/Honolulu</span><span class="sxs-lookup"><span data-stu-id="9fb9f-120">Pacific/Honolulu</span></span>

<span data-ttu-id="9fb9f-121">Amerika/Anchorage</span><span class="sxs-lookup"><span data-stu-id="9fb9f-121">America/Anchorage</span></span>

<span data-ttu-id="9fb9f-122">Amerika/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="9fb9f-122">America/Santa_Isabel</span></span>

<span data-ttu-id="9fb9f-123">Amerika/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="9fb9f-123">America/Los_Angeles</span></span>

<span data-ttu-id="9fb9f-124">Amerika/Phoenix</span><span class="sxs-lookup"><span data-stu-id="9fb9f-124">America/Phoenix</span></span>

<span data-ttu-id="9fb9f-125">Amerika/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="9fb9f-125">America/Chihuahua</span></span>

<span data-ttu-id="9fb9f-126">Amerika/Denver</span><span class="sxs-lookup"><span data-stu-id="9fb9f-126">America/Denver</span></span>

<span data-ttu-id="9fb9f-127">Amerika/Guatemala</span><span class="sxs-lookup"><span data-stu-id="9fb9f-127">America/Guatemala</span></span>

<span data-ttu-id="9fb9f-128">Amerika/Chicago</span><span class="sxs-lookup"><span data-stu-id="9fb9f-128">America/Chicago</span></span>

<span data-ttu-id="9fb9f-129">Amerika/Mexico_Stadt</span><span class="sxs-lookup"><span data-stu-id="9fb9f-129">America/Mexico_City</span></span>

<span data-ttu-id="9fb9f-130">Amerika/Regina</span><span class="sxs-lookup"><span data-stu-id="9fb9f-130">America/Regina</span></span>

<span data-ttu-id="9fb9f-131">Amerika/Bogota</span><span class="sxs-lookup"><span data-stu-id="9fb9f-131">America/Bogota</span></span>

<span data-ttu-id="9fb9f-132">Amerika/New_York</span><span class="sxs-lookup"><span data-stu-id="9fb9f-132">America/New_York</span></span>

<span data-ttu-id="9fb9f-133">Amerika/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="9fb9f-133">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="9fb9f-134">Amerika/Caracas</span><span class="sxs-lookup"><span data-stu-id="9fb9f-134">America/Caracas</span></span>

<span data-ttu-id="9fb9f-135">Amerika/Asuncion</span><span class="sxs-lookup"><span data-stu-id="9fb9f-135">America/Asuncion</span></span>

<span data-ttu-id="9fb9f-136">Amerika/Halifax</span><span class="sxs-lookup"><span data-stu-id="9fb9f-136">America/Halifax</span></span>

<span data-ttu-id="9fb9f-137">Amerika/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="9fb9f-137">America/Cuiaba</span></span>

<span data-ttu-id="9fb9f-138">Amerika/La_Paz</span><span class="sxs-lookup"><span data-stu-id="9fb9f-138">America/La_Paz</span></span>

<span data-ttu-id="9fb9f-139">Amerika/Santiago</span><span class="sxs-lookup"><span data-stu-id="9fb9f-139">America/Santiago</span></span>

<span data-ttu-id="9fb9f-140">Amerika/St_Johns</span><span class="sxs-lookup"><span data-stu-id="9fb9f-140">America/St_Johns</span></span>

<span data-ttu-id="9fb9f-141">Amerika/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="9fb9f-141">America/Sao_Paulo</span></span>

<span data-ttu-id="9fb9f-142">Amerika/Argentinien/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="9fb9f-142">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="9fb9f-143">Amerika/Cayenne</span><span class="sxs-lookup"><span data-stu-id="9fb9f-143">America/Cayenne</span></span>

<span data-ttu-id="9fb9f-144">Amerika/Godthab</span><span class="sxs-lookup"><span data-stu-id="9fb9f-144">America/Godthab</span></span>

<span data-ttu-id="9fb9f-145">Amerika/Montevideo</span><span class="sxs-lookup"><span data-stu-id="9fb9f-145">America/Montevideo</span></span>

<span data-ttu-id="9fb9f-146">Amerika/Bahia</span><span class="sxs-lookup"><span data-stu-id="9fb9f-146">America/Bahia</span></span>

<span data-ttu-id="9fb9f-147">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="9fb9f-147">Etc/GMT+2</span></span>

<span data-ttu-id="9fb9f-148">Atlantik/Azoren</span><span class="sxs-lookup"><span data-stu-id="9fb9f-148">Atlantic/Azores</span></span>

<span data-ttu-id="9fb9f-149">Atlantik/Kap_Verde</span><span class="sxs-lookup"><span data-stu-id="9fb9f-149">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="9fb9f-150">Afrika/Casablanca</span><span class="sxs-lookup"><span data-stu-id="9fb9f-150">Africa/Casablanca</span></span>

<span data-ttu-id="9fb9f-151">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="9fb9f-151">Etc/GMT</span></span>

<span data-ttu-id="9fb9f-152">Europa/London</span><span class="sxs-lookup"><span data-stu-id="9fb9f-152">Europe/London</span></span>

<span data-ttu-id="9fb9f-153">Atlantik/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="9fb9f-153">Atlantic/Reykjavik</span></span>

<span data-ttu-id="9fb9f-154">Europa/Berlin</span><span class="sxs-lookup"><span data-stu-id="9fb9f-154">Europe/Berlin</span></span>

<span data-ttu-id="9fb9f-155">Europa/Budapest</span><span class="sxs-lookup"><span data-stu-id="9fb9f-155">Europe/Budapest</span></span>

<span data-ttu-id="9fb9f-156">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="9fb9f-156">Europe/Paris</span></span>

<span data-ttu-id="9fb9f-157">Europa/Warschau</span><span class="sxs-lookup"><span data-stu-id="9fb9f-157">Europe/Warsaw</span></span>

<span data-ttu-id="9fb9f-158">Afrika/Lagos</span><span class="sxs-lookup"><span data-stu-id="9fb9f-158">Africa/Lagos</span></span>

<span data-ttu-id="9fb9f-159">Afrika/Windhoek</span><span class="sxs-lookup"><span data-stu-id="9fb9f-159">Africa/Windhoek</span></span>

<span data-ttu-id="9fb9f-160">Europa/Bukarest</span><span class="sxs-lookup"><span data-stu-id="9fb9f-160">Europe/Bucharest</span></span>

<span data-ttu-id="9fb9f-161">Asien/Beirut</span><span class="sxs-lookup"><span data-stu-id="9fb9f-161">Asia/Beirut</span></span>

<span data-ttu-id="9fb9f-162">Afrika/Kairo</span><span class="sxs-lookup"><span data-stu-id="9fb9f-162">Africa/Cairo</span></span>

<span data-ttu-id="9fb9f-163">Asien/Damaskus</span><span class="sxs-lookup"><span data-stu-id="9fb9f-163">Asia/Damascus</span></span>

<span data-ttu-id="9fb9f-164">Afrika/Johannesburg</span><span class="sxs-lookup"><span data-stu-id="9fb9f-164">Africa/Johannesburg</span></span>

<span data-ttu-id="9fb9f-165">Europa/Kiew</span><span class="sxs-lookup"><span data-stu-id="9fb9f-165">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="9fb9f-166">Europa/Istanbul</span><span class="sxs-lookup"><span data-stu-id="9fb9f-166">Europe/Istanbul</span></span>

<span data-ttu-id="9fb9f-167">Asien/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="9fb9f-167">Asia/Jerusalem</span></span>

<span data-ttu-id="9fb9f-168">Asien/Amman</span><span class="sxs-lookup"><span data-stu-id="9fb9f-168">Asia/Amman</span></span>

<span data-ttu-id="9fb9f-169">Asien/Bagdad</span><span class="sxs-lookup"><span data-stu-id="9fb9f-169">Asia/Baghdad</span></span>

<span data-ttu-id="9fb9f-170">Europa/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="9fb9f-170">Europe/Kaliningrad</span></span>

<span data-ttu-id="9fb9f-171">Asien/Riad</span><span class="sxs-lookup"><span data-stu-id="9fb9f-171">Asia/Riyadh</span></span>

<span data-ttu-id="9fb9f-172">Afrika/Nairobi</span><span class="sxs-lookup"><span data-stu-id="9fb9f-172">Africa/Nairobi</span></span>

<span data-ttu-id="9fb9f-173">Asien/Teheran</span><span class="sxs-lookup"><span data-stu-id="9fb9f-173">Asia/Tehran</span></span>

<span data-ttu-id="9fb9f-174">Asien/Dubai</span><span class="sxs-lookup"><span data-stu-id="9fb9f-174">Asia/Dubai</span></span>

<span data-ttu-id="9fb9f-175">Asien/Baku</span><span class="sxs-lookup"><span data-stu-id="9fb9f-175">Asia/Baku</span></span>

<span data-ttu-id="9fb9f-176">Europa/Moskau</span><span class="sxs-lookup"><span data-stu-id="9fb9f-176">Europe/Moscow</span></span>

<span data-ttu-id="9fb9f-177">Indisch/Mauritius</span><span class="sxs-lookup"><span data-stu-id="9fb9f-177">Indian/Mauritius</span></span>

<span data-ttu-id="9fb9f-178">Asien/Tiflis</span><span class="sxs-lookup"><span data-stu-id="9fb9f-178">Asia/Tbilisi</span></span>

<span data-ttu-id="9fb9f-179">Asien/Eriwan</span><span class="sxs-lookup"><span data-stu-id="9fb9f-179">Asia/Yerevan</span></span>

<span data-ttu-id="9fb9f-180">Asien/Kabul</span><span class="sxs-lookup"><span data-stu-id="9fb9f-180">Asia/Kabul</span></span>

<span data-ttu-id="9fb9f-181">Asien/Karatschi</span><span class="sxs-lookup"><span data-stu-id="9fb9f-181">Asia/Karachi</span></span>

<span data-ttu-id="9fb9f-182">Asien/Taschkent</span><span class="sxs-lookup"><span data-stu-id="9fb9f-182">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="9fb9f-183">Asien/Kolkata</span><span class="sxs-lookup"><span data-stu-id="9fb9f-183">Asia/Kolkata</span></span>

<span data-ttu-id="9fb9f-184">Asien/Colombo</span><span class="sxs-lookup"><span data-stu-id="9fb9f-184">Asia/Colombo</span></span>

<span data-ttu-id="9fb9f-185">Asien/Katmandu</span><span class="sxs-lookup"><span data-stu-id="9fb9f-185">Asia/Kathmandu</span></span>

<span data-ttu-id="9fb9f-186">Asien/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="9fb9f-186">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="9fb9f-187">Asien/Dhaka</span><span class="sxs-lookup"><span data-stu-id="9fb9f-187">Asia/Dhaka</span></span>

<span data-ttu-id="9fb9f-188">Asien/Jekaterinburg</span><span class="sxs-lookup"><span data-stu-id="9fb9f-188">Asia/Yekaterinburg</span></span>

<span data-ttu-id="9fb9f-189">Asien/Yangon (Rangun)</span><span class="sxs-lookup"><span data-stu-id="9fb9f-189">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="9fb9f-190">Asien/Bangkok</span><span class="sxs-lookup"><span data-stu-id="9fb9f-190">Asia/Bangkok</span></span>

<span data-ttu-id="9fb9f-191">Asien/Nowosibirsk</span><span class="sxs-lookup"><span data-stu-id="9fb9f-191">Asia/Novosibirsk</span></span>

<span data-ttu-id="9fb9f-192">Asien/Shanghai</span><span class="sxs-lookup"><span data-stu-id="9fb9f-192">Asia/Shanghai</span></span>

<span data-ttu-id="9fb9f-193">Asien/Krasnojarsk</span><span class="sxs-lookup"><span data-stu-id="9fb9f-193">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="9fb9f-194">Asien/Singapur</span><span class="sxs-lookup"><span data-stu-id="9fb9f-194">Asia/Singapore</span></span>

<span data-ttu-id="9fb9f-195">Australien/Perth</span><span class="sxs-lookup"><span data-stu-id="9fb9f-195">Australia/Perth</span></span>

<span data-ttu-id="9fb9f-196">Asien/Taipeh</span><span class="sxs-lookup"><span data-stu-id="9fb9f-196">Asia/Taipei</span></span>

<span data-ttu-id="9fb9f-197">Asien/Ulan-Bator</span><span class="sxs-lookup"><span data-stu-id="9fb9f-197">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="9fb9f-198">Asien/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="9fb9f-198">Asia/Irkutsk</span></span>

<span data-ttu-id="9fb9f-199">Asien/Tokio</span><span class="sxs-lookup"><span data-stu-id="9fb9f-199">Asia/Tokyo</span></span>

<span data-ttu-id="9fb9f-200">Asien/Seoul</span><span class="sxs-lookup"><span data-stu-id="9fb9f-200">Asia/Seoul</span></span>

<span data-ttu-id="9fb9f-201">Australien/Adelaide</span><span class="sxs-lookup"><span data-stu-id="9fb9f-201">Australia/Adelaide</span></span>

<span data-ttu-id="9fb9f-202">Australien/Darwin</span><span class="sxs-lookup"><span data-stu-id="9fb9f-202">Australia/Darwin</span></span>

<span data-ttu-id="9fb9f-203">Australien/Brisbane</span><span class="sxs-lookup"><span data-stu-id="9fb9f-203">Australia/Brisbane</span></span>

<span data-ttu-id="9fb9f-204">Australien/Sydney</span><span class="sxs-lookup"><span data-stu-id="9fb9f-204">Australia/Sydney</span></span>

<span data-ttu-id="9fb9f-205">Pazifik/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="9fb9f-205">Pacific/Port_Moresby</span></span>

<span data-ttu-id="9fb9f-206">Australien/Hobart</span><span class="sxs-lookup"><span data-stu-id="9fb9f-206">Australia/Hobart</span></span>

<span data-ttu-id="9fb9f-207">Asien/Jakutsk</span><span class="sxs-lookup"><span data-stu-id="9fb9f-207">Asia/Yakutsk</span></span>

<span data-ttu-id="9fb9f-208">Pazifik/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="9fb9f-208">Pacific/Guadalcanal</span></span>

<span data-ttu-id="9fb9f-209">Asien/Wladiwostok</span><span class="sxs-lookup"><span data-stu-id="9fb9f-209">Asia/Vladivostok</span></span>

<span data-ttu-id="9fb9f-210">Pazifik/Auckland</span><span class="sxs-lookup"><span data-stu-id="9fb9f-210">Pacific/Auckland</span></span>

<span data-ttu-id="9fb9f-211">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="9fb9f-211">Etc/GMT-12</span></span>

<span data-ttu-id="9fb9f-212">Pazifik/Fidschi</span><span class="sxs-lookup"><span data-stu-id="9fb9f-212">Pacific/Fiji</span></span>

<span data-ttu-id="9fb9f-213">Asien/Magadan</span><span class="sxs-lookup"><span data-stu-id="9fb9f-213">Asia/Magadan</span></span>

<span data-ttu-id="9fb9f-214">Pazifik/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="9fb9f-214">Pacific/Tongatapu</span></span>

<span data-ttu-id="9fb9f-215">Pazifik/Apia</span><span class="sxs-lookup"><span data-stu-id="9fb9f-215">Pacific/Apia</span></span>

<span data-ttu-id="9fb9f-216">Pazifik/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="9fb9f-216">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fb9f-217">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9fb9f-217">JSON representation</span></span>

<span data-ttu-id="9fb9f-218">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9fb9f-218">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
