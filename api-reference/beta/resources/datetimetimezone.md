---
title: Ressourcentyp dateTimeTimeZone
description: Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.
ms.openlocfilehash: a95ebf35d6a47b8b39c34cab8d6d35b92eaae2c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060668"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="c9b98-103">Ressourcentyp dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c9b98-103">dateTimeTimeZone resource type</span></span>

> <span data-ttu-id="c9b98-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c9b98-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9b98-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9b98-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9b98-106">Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.</span><span class="sxs-lookup"><span data-stu-id="c9b98-106">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="c9b98-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9b98-107">Properties</span></span>
| <span data-ttu-id="c9b98-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9b98-108">Property</span></span>     | <span data-ttu-id="c9b98-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c9b98-109">Type</span></span>   |<span data-ttu-id="c9b98-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9b98-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9b98-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="c9b98-111">DateTime</span></span>|<span data-ttu-id="c9b98-112">String</span><span class="sxs-lookup"><span data-stu-id="c9b98-112">String</span></span>|<span data-ttu-id="c9b98-113">Ein bestimmter Zeitpunkt in einer kombinierten Datums- und Uhrzeitsdarstellung (`<date>T<time>`).</span><span class="sxs-lookup"><span data-stu-id="c9b98-113">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="c9b98-114">TimeZone</span><span class="sxs-lookup"><span data-stu-id="c9b98-114">TimeZone</span></span>|<span data-ttu-id="c9b98-115">String</span><span class="sxs-lookup"><span data-stu-id="c9b98-115">String</span></span>|<span data-ttu-id="c9b98-116">Einer der folgenden Zeitzonennamen.</span><span class="sxs-lookup"><span data-stu-id="c9b98-116">One of the following time zone names.</span></span>|

<span data-ttu-id="c9b98-117">Die Eigenschaft _TimeZone_ kann auf eine beliebige, von Windows unterstützte Zeitzone und auf einen der folgenden Zeitzonennamen eingestellt werden .</span><span class="sxs-lookup"><span data-stu-id="c9b98-117">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="c9b98-118">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="c9b98-118">Etc/GMT+12</span></span>

<span data-ttu-id="c9b98-119">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="c9b98-119">Etc/GMT+11</span></span>

<span data-ttu-id="c9b98-120">Pazifik/Honolulu</span><span class="sxs-lookup"><span data-stu-id="c9b98-120">Pacific/Honolulu</span></span>

<span data-ttu-id="c9b98-121">Amerika/Anchorage</span><span class="sxs-lookup"><span data-stu-id="c9b98-121">America/Anchorage</span></span>

<span data-ttu-id="c9b98-122">Amerika/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="c9b98-122">America/Santa_Isabel</span></span>

<span data-ttu-id="c9b98-123">Amerika/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="c9b98-123">America/Los_Angeles</span></span>

<span data-ttu-id="c9b98-124">Amerika/Phoenix</span><span class="sxs-lookup"><span data-stu-id="c9b98-124">America/Phoenix</span></span>

<span data-ttu-id="c9b98-125">Amerika/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="c9b98-125">America/Chihuahua</span></span>

<span data-ttu-id="c9b98-126">Amerika/Denver</span><span class="sxs-lookup"><span data-stu-id="c9b98-126">America/Denver</span></span>

<span data-ttu-id="c9b98-127">Amerika/Guatemala</span><span class="sxs-lookup"><span data-stu-id="c9b98-127">America/Guatemala</span></span>

<span data-ttu-id="c9b98-128">Amerika/Chicago</span><span class="sxs-lookup"><span data-stu-id="c9b98-128">America/Chicago</span></span>

<span data-ttu-id="c9b98-129">Amerika/Mexico_Stadt</span><span class="sxs-lookup"><span data-stu-id="c9b98-129">America/Mexico_City</span></span>

<span data-ttu-id="c9b98-130">Amerika/Regina</span><span class="sxs-lookup"><span data-stu-id="c9b98-130">America/Regina</span></span>

<span data-ttu-id="c9b98-131">Amerika/Bogota</span><span class="sxs-lookup"><span data-stu-id="c9b98-131">America/Bogota</span></span>

<span data-ttu-id="c9b98-132">Amerika/New_York</span><span class="sxs-lookup"><span data-stu-id="c9b98-132">America/New_York</span></span>

<span data-ttu-id="c9b98-133">Amerika/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="c9b98-133">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="c9b98-134">Amerika/Caracas</span><span class="sxs-lookup"><span data-stu-id="c9b98-134">America/Caracas</span></span>

<span data-ttu-id="c9b98-135">Amerika/Asuncion</span><span class="sxs-lookup"><span data-stu-id="c9b98-135">America/Asuncion</span></span>

<span data-ttu-id="c9b98-136">Amerika/Halifax</span><span class="sxs-lookup"><span data-stu-id="c9b98-136">America/Halifax</span></span>

<span data-ttu-id="c9b98-137">Amerika/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="c9b98-137">America/Cuiaba</span></span>

<span data-ttu-id="c9b98-138">Amerika/La_Paz</span><span class="sxs-lookup"><span data-stu-id="c9b98-138">America/La_Paz</span></span>

<span data-ttu-id="c9b98-139">Amerika/Santiago</span><span class="sxs-lookup"><span data-stu-id="c9b98-139">America/Santiago</span></span>

<span data-ttu-id="c9b98-140">Amerika/St_Johns</span><span class="sxs-lookup"><span data-stu-id="c9b98-140">America/St_Johns</span></span>

<span data-ttu-id="c9b98-141">Amerika/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="c9b98-141">America/Sao_Paulo</span></span>

<span data-ttu-id="c9b98-142">Amerika/Argentinien/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="c9b98-142">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="c9b98-143">Amerika/Cayenne</span><span class="sxs-lookup"><span data-stu-id="c9b98-143">America/Cayenne</span></span>

<span data-ttu-id="c9b98-144">Amerika/Godthab</span><span class="sxs-lookup"><span data-stu-id="c9b98-144">America/Godthab</span></span>

<span data-ttu-id="c9b98-145">Amerika/Montevideo</span><span class="sxs-lookup"><span data-stu-id="c9b98-145">America/Montevideo</span></span>

<span data-ttu-id="c9b98-146">Amerika/Bahia</span><span class="sxs-lookup"><span data-stu-id="c9b98-146">America/Bahia</span></span>

<span data-ttu-id="c9b98-147">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="c9b98-147">Etc/GMT+2</span></span>

<span data-ttu-id="c9b98-148">Atlantik/Azoren</span><span class="sxs-lookup"><span data-stu-id="c9b98-148">Atlantic/Azores</span></span>

<span data-ttu-id="c9b98-149">Atlantik/Kap_Verde</span><span class="sxs-lookup"><span data-stu-id="c9b98-149">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="c9b98-150">Afrika/Casablanca</span><span class="sxs-lookup"><span data-stu-id="c9b98-150">Africa/Casablanca</span></span>

<span data-ttu-id="c9b98-151">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="c9b98-151">Etc/GMT</span></span>

<span data-ttu-id="c9b98-152">Europa/London</span><span class="sxs-lookup"><span data-stu-id="c9b98-152">Europe/London</span></span>

<span data-ttu-id="c9b98-153">Atlantik/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="c9b98-153">Atlantic/Reykjavik</span></span>

<span data-ttu-id="c9b98-154">Europa/Berlin</span><span class="sxs-lookup"><span data-stu-id="c9b98-154">Europe/Berlin</span></span>

<span data-ttu-id="c9b98-155">Europa/Budapest</span><span class="sxs-lookup"><span data-stu-id="c9b98-155">Europe/Budapest</span></span>

<span data-ttu-id="c9b98-156">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="c9b98-156">Europe/Paris</span></span>

<span data-ttu-id="c9b98-157">Europa/Warschau</span><span class="sxs-lookup"><span data-stu-id="c9b98-157">Europe/Warsaw</span></span>

<span data-ttu-id="c9b98-158">Afrika/Lagos</span><span class="sxs-lookup"><span data-stu-id="c9b98-158">Africa/Lagos</span></span>

<span data-ttu-id="c9b98-159">Afrika/Windhoek</span><span class="sxs-lookup"><span data-stu-id="c9b98-159">Africa/Windhoek</span></span>

<span data-ttu-id="c9b98-160">Europa/Bukarest</span><span class="sxs-lookup"><span data-stu-id="c9b98-160">Europe/Bucharest</span></span>

<span data-ttu-id="c9b98-161">Asien/Beirut</span><span class="sxs-lookup"><span data-stu-id="c9b98-161">Asia/Beirut</span></span>

<span data-ttu-id="c9b98-162">Afrika/Kairo</span><span class="sxs-lookup"><span data-stu-id="c9b98-162">Africa/Cairo</span></span>

<span data-ttu-id="c9b98-163">Asien/Damaskus</span><span class="sxs-lookup"><span data-stu-id="c9b98-163">Asia/Damascus</span></span>

<span data-ttu-id="c9b98-164">Afrika/Johannesburg</span><span class="sxs-lookup"><span data-stu-id="c9b98-164">Africa/Johannesburg</span></span>

<span data-ttu-id="c9b98-165">Europa/Kiew</span><span class="sxs-lookup"><span data-stu-id="c9b98-165">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="c9b98-166">Europa/Istanbul</span><span class="sxs-lookup"><span data-stu-id="c9b98-166">Europe/Istanbul</span></span>

<span data-ttu-id="c9b98-167">Asien/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="c9b98-167">Asia/Jerusalem</span></span>

<span data-ttu-id="c9b98-168">Asien/Amman</span><span class="sxs-lookup"><span data-stu-id="c9b98-168">Asia/Amman</span></span>

<span data-ttu-id="c9b98-169">Asien/Bagdad</span><span class="sxs-lookup"><span data-stu-id="c9b98-169">Asia/Baghdad</span></span>

<span data-ttu-id="c9b98-170">Europa/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="c9b98-170">Europe/Kaliningrad</span></span>

<span data-ttu-id="c9b98-171">Asien/Riad</span><span class="sxs-lookup"><span data-stu-id="c9b98-171">Asia/Riyadh</span></span>

<span data-ttu-id="c9b98-172">Afrika/Nairobi</span><span class="sxs-lookup"><span data-stu-id="c9b98-172">Africa/Nairobi</span></span>

<span data-ttu-id="c9b98-173">Asien/Teheran</span><span class="sxs-lookup"><span data-stu-id="c9b98-173">Asia/Tehran</span></span>

<span data-ttu-id="c9b98-174">Asien/Dubai</span><span class="sxs-lookup"><span data-stu-id="c9b98-174">Asia/Dubai</span></span>

<span data-ttu-id="c9b98-175">Asien/Baku</span><span class="sxs-lookup"><span data-stu-id="c9b98-175">Asia/Baku</span></span>

<span data-ttu-id="c9b98-176">Europa/Moskau</span><span class="sxs-lookup"><span data-stu-id="c9b98-176">Europe/Moscow</span></span>

<span data-ttu-id="c9b98-177">Indisch/Mauritius</span><span class="sxs-lookup"><span data-stu-id="c9b98-177">Indian/Mauritius</span></span>

<span data-ttu-id="c9b98-178">Asien/Tiflis</span><span class="sxs-lookup"><span data-stu-id="c9b98-178">Asia/Tbilisi</span></span>

<span data-ttu-id="c9b98-179">Asien/Eriwan</span><span class="sxs-lookup"><span data-stu-id="c9b98-179">Asia/Yerevan</span></span>

<span data-ttu-id="c9b98-180">Asien/Kabul</span><span class="sxs-lookup"><span data-stu-id="c9b98-180">Asia/Kabul</span></span>

<span data-ttu-id="c9b98-181">Asien/Karatschi</span><span class="sxs-lookup"><span data-stu-id="c9b98-181">Asia/Karachi</span></span>

<span data-ttu-id="c9b98-182">Asien/Taschkent</span><span class="sxs-lookup"><span data-stu-id="c9b98-182">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="c9b98-183">Asien/Kolkata</span><span class="sxs-lookup"><span data-stu-id="c9b98-183">Asia/Kolkata</span></span>

<span data-ttu-id="c9b98-184">Asien/Colombo</span><span class="sxs-lookup"><span data-stu-id="c9b98-184">Asia/Colombo</span></span>

<span data-ttu-id="c9b98-185">Asien/Katmandu</span><span class="sxs-lookup"><span data-stu-id="c9b98-185">Asia/Kathmandu</span></span>

<span data-ttu-id="c9b98-186">Asien/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="c9b98-186">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="c9b98-187">Asien/Dhaka</span><span class="sxs-lookup"><span data-stu-id="c9b98-187">Asia/Dhaka</span></span>

<span data-ttu-id="c9b98-188">Asien/Jekaterinburg</span><span class="sxs-lookup"><span data-stu-id="c9b98-188">Asia/Yekaterinburg</span></span>

<span data-ttu-id="c9b98-189">Asien/Yangon (Rangun)</span><span class="sxs-lookup"><span data-stu-id="c9b98-189">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="c9b98-190">Asien/Bangkok</span><span class="sxs-lookup"><span data-stu-id="c9b98-190">Asia/Bangkok</span></span>

<span data-ttu-id="c9b98-191">Asien/Nowosibirsk</span><span class="sxs-lookup"><span data-stu-id="c9b98-191">Asia/Novosibirsk</span></span>

<span data-ttu-id="c9b98-192">Asien/Shanghai</span><span class="sxs-lookup"><span data-stu-id="c9b98-192">Asia/Shanghai</span></span>

<span data-ttu-id="c9b98-193">Asien/Krasnojarsk</span><span class="sxs-lookup"><span data-stu-id="c9b98-193">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="c9b98-194">Asien/Singapur</span><span class="sxs-lookup"><span data-stu-id="c9b98-194">Asia/Singapore</span></span>

<span data-ttu-id="c9b98-195">Australien/Perth</span><span class="sxs-lookup"><span data-stu-id="c9b98-195">Australia/Perth</span></span>

<span data-ttu-id="c9b98-196">Asien/Taipeh</span><span class="sxs-lookup"><span data-stu-id="c9b98-196">Asia/Taipei</span></span>

<span data-ttu-id="c9b98-197">Asien/Ulan-Bator</span><span class="sxs-lookup"><span data-stu-id="c9b98-197">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="c9b98-198">Asien/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="c9b98-198">Asia/Irkutsk</span></span>

<span data-ttu-id="c9b98-199">Asien/Tokio</span><span class="sxs-lookup"><span data-stu-id="c9b98-199">Asia/Tokyo</span></span>

<span data-ttu-id="c9b98-200">Asien/Seoul</span><span class="sxs-lookup"><span data-stu-id="c9b98-200">Asia/Seoul</span></span>

<span data-ttu-id="c9b98-201">Australien/Adelaide</span><span class="sxs-lookup"><span data-stu-id="c9b98-201">Australia/Adelaide</span></span>

<span data-ttu-id="c9b98-202">Australien/Darwin</span><span class="sxs-lookup"><span data-stu-id="c9b98-202">Australia/Darwin</span></span>

<span data-ttu-id="c9b98-203">Australien/Brisbane</span><span class="sxs-lookup"><span data-stu-id="c9b98-203">Australia/Brisbane</span></span>

<span data-ttu-id="c9b98-204">Australien/Sydney</span><span class="sxs-lookup"><span data-stu-id="c9b98-204">Australia/Sydney</span></span>

<span data-ttu-id="c9b98-205">Pazifik/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="c9b98-205">Pacific/Port_Moresby</span></span>

<span data-ttu-id="c9b98-206">Australien/Hobart</span><span class="sxs-lookup"><span data-stu-id="c9b98-206">Australia/Hobart</span></span>

<span data-ttu-id="c9b98-207">Asien/Jakutsk</span><span class="sxs-lookup"><span data-stu-id="c9b98-207">Asia/Yakutsk</span></span>

<span data-ttu-id="c9b98-208">Pazifik/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="c9b98-208">Pacific/Guadalcanal</span></span>

<span data-ttu-id="c9b98-209">Asien/Wladiwostok</span><span class="sxs-lookup"><span data-stu-id="c9b98-209">Asia/Vladivostok</span></span>

<span data-ttu-id="c9b98-210">Pazifik/Auckland</span><span class="sxs-lookup"><span data-stu-id="c9b98-210">Pacific/Auckland</span></span>

<span data-ttu-id="c9b98-211">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="c9b98-211">Etc/GMT-12</span></span>

<span data-ttu-id="c9b98-212">Pazifik/Fidschi</span><span class="sxs-lookup"><span data-stu-id="c9b98-212">Pacific/Fiji</span></span>

<span data-ttu-id="c9b98-213">Asien/Magadan</span><span class="sxs-lookup"><span data-stu-id="c9b98-213">Asia/Magadan</span></span>

<span data-ttu-id="c9b98-214">Pazifik/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="c9b98-214">Pacific/Tongatapu</span></span>

<span data-ttu-id="c9b98-215">Pazifik/Apia</span><span class="sxs-lookup"><span data-stu-id="c9b98-215">Pacific/Apia</span></span>

<span data-ttu-id="c9b98-216">Pazifik/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="c9b98-216">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9b98-217">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9b98-217">JSON representation</span></span>

<span data-ttu-id="c9b98-218">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c9b98-218">Here is a JSON representation of the resource</span></span>

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
