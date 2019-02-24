---
title: Ressourcentyp dateTimeTimeZone
description: Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.
localization_priority: Priority
ms.openlocfilehash: 9e031b053ebc185ee02fa11571019529a870cf04
ms.sourcegitcommit: 7412dd2f2d5ed66afa2b0759c861ad23b4c6ecdf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/23/2019
ms.locfileid: "30212361"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="215d8-103">dateTimeTimeZone-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="215d8-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="215d8-104">Beschreibt das Datum, die Uhrzeit und Zeitzone eines Zeitpunkts.</span><span class="sxs-lookup"><span data-stu-id="215d8-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="215d8-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="215d8-105">Properties</span></span>
| <span data-ttu-id="215d8-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="215d8-106">Property</span></span>     | <span data-ttu-id="215d8-107">Typ</span><span class="sxs-lookup"><span data-stu-id="215d8-107">Type</span></span>   |<span data-ttu-id="215d8-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="215d8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="215d8-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="215d8-109">dateTime</span></span>|<span data-ttu-id="215d8-110">String</span><span class="sxs-lookup"><span data-stu-id="215d8-110">String</span></span>|<span data-ttu-id="215d8-111">Ein bestimmter Zeitpunkt in einer kombinierten Datums- und Uhrzeitsdarstellung (`{date}T{time}`; zum Beispiel `2017-08-29T04:00:00.0000000`).</span><span class="sxs-lookup"><span data-stu-id="215d8-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span>|
|<span data-ttu-id="215d8-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="215d8-112">timeZone</span></span>|<span data-ttu-id="215d8-113">String</span><span class="sxs-lookup"><span data-stu-id="215d8-113">String</span></span>|<span data-ttu-id="215d8-114">Einer der folgenden Zeitzonennamen.</span><span class="sxs-lookup"><span data-stu-id="215d8-114">One of the following time zone names.</span></span>|

<span data-ttu-id="215d8-115">Die Eigenschaft _TimeZone_ kann auf eine beliebige, von Windows unterstützte Zeitzone und auf einen der folgenden Zeitzonennamen eingestellt werden .</span><span class="sxs-lookup"><span data-stu-id="215d8-115">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="215d8-116">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="215d8-116">Etc/GMT+12</span></span>

<span data-ttu-id="215d8-117">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="215d8-117">Etc/GMT+11</span></span>

<span data-ttu-id="215d8-118">Pazifik/Honolulu</span><span class="sxs-lookup"><span data-stu-id="215d8-118">Pacific/Honolulu</span></span>

<span data-ttu-id="215d8-119">Amerika/Anchorage</span><span class="sxs-lookup"><span data-stu-id="215d8-119">America/Anchorage</span></span>

<span data-ttu-id="215d8-120">Amerika/Santa_Isabel</span><span class="sxs-lookup"><span data-stu-id="215d8-120">America/Santa_Isabel</span></span>

<span data-ttu-id="215d8-121">Amerika/Los_Angeles</span><span class="sxs-lookup"><span data-stu-id="215d8-121">America/Los_Angeles</span></span>

<span data-ttu-id="215d8-122">Amerika/Phoenix</span><span class="sxs-lookup"><span data-stu-id="215d8-122">America/Phoenix</span></span>

<span data-ttu-id="215d8-123">Amerika/Chihuahua</span><span class="sxs-lookup"><span data-stu-id="215d8-123">America/Chihuahua</span></span>

<span data-ttu-id="215d8-124">Amerika/Denver</span><span class="sxs-lookup"><span data-stu-id="215d8-124">America/Denver</span></span>

<span data-ttu-id="215d8-125">Amerika/Guatemala</span><span class="sxs-lookup"><span data-stu-id="215d8-125">America/Guatemala</span></span>

<span data-ttu-id="215d8-126">Amerika/Chicago</span><span class="sxs-lookup"><span data-stu-id="215d8-126">America/Chicago</span></span>

<span data-ttu-id="215d8-127">Amerika/Mexico_Stadt</span><span class="sxs-lookup"><span data-stu-id="215d8-127">America/Mexico_City</span></span>

<span data-ttu-id="215d8-128">Amerika/Regina</span><span class="sxs-lookup"><span data-stu-id="215d8-128">America/Regina</span></span>

<span data-ttu-id="215d8-129">Amerika/Bogota</span><span class="sxs-lookup"><span data-stu-id="215d8-129">America/Bogota</span></span>

<span data-ttu-id="215d8-130">Amerika/New_York</span><span class="sxs-lookup"><span data-stu-id="215d8-130">America/New_York</span></span>

<span data-ttu-id="215d8-131">Amerika/Indiana/Indianapolis</span><span class="sxs-lookup"><span data-stu-id="215d8-131">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="215d8-132">Amerika/Caracas</span><span class="sxs-lookup"><span data-stu-id="215d8-132">America/Caracas</span></span>

<span data-ttu-id="215d8-133">Amerika/Asuncion</span><span class="sxs-lookup"><span data-stu-id="215d8-133">America/Asuncion</span></span>

<span data-ttu-id="215d8-134">Amerika/Halifax</span><span class="sxs-lookup"><span data-stu-id="215d8-134">America/Halifax</span></span>

<span data-ttu-id="215d8-135">Amerika/Cuiaba</span><span class="sxs-lookup"><span data-stu-id="215d8-135">America/Cuiaba</span></span>

<span data-ttu-id="215d8-136">Amerika/La_Paz</span><span class="sxs-lookup"><span data-stu-id="215d8-136">America/La_Paz</span></span>

<span data-ttu-id="215d8-137">Amerika/Santiago</span><span class="sxs-lookup"><span data-stu-id="215d8-137">America/Santiago</span></span>

<span data-ttu-id="215d8-138">Amerika/St_Johns</span><span class="sxs-lookup"><span data-stu-id="215d8-138">America/St_Johns</span></span>

<span data-ttu-id="215d8-139">Amerika/Sao_Paulo</span><span class="sxs-lookup"><span data-stu-id="215d8-139">America/Sao_Paulo</span></span>

<span data-ttu-id="215d8-140">Amerika/Argentinien/Buenos_Aires</span><span class="sxs-lookup"><span data-stu-id="215d8-140">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="215d8-141">Amerika/Cayenne</span><span class="sxs-lookup"><span data-stu-id="215d8-141">America/Cayenne</span></span>

<span data-ttu-id="215d8-142">Amerika/Godthab</span><span class="sxs-lookup"><span data-stu-id="215d8-142">America/Godthab</span></span>

<span data-ttu-id="215d8-143">Amerika/Montevideo</span><span class="sxs-lookup"><span data-stu-id="215d8-143">America/Montevideo</span></span>

<span data-ttu-id="215d8-144">Amerika/Bahia</span><span class="sxs-lookup"><span data-stu-id="215d8-144">America/Bahia</span></span>

<span data-ttu-id="215d8-145">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="215d8-145">Etc/GMT+2</span></span>

<span data-ttu-id="215d8-146">Atlantik/Azoren</span><span class="sxs-lookup"><span data-stu-id="215d8-146">Atlantic/Azores</span></span>

<span data-ttu-id="215d8-147">Atlantik/Kap_Verde</span><span class="sxs-lookup"><span data-stu-id="215d8-147">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="215d8-148">Afrika/Casablanca</span><span class="sxs-lookup"><span data-stu-id="215d8-148">Africa/Casablanca</span></span>

<span data-ttu-id="215d8-149">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="215d8-149">Etc/GMT</span></span>

<span data-ttu-id="215d8-150">Europa/London</span><span class="sxs-lookup"><span data-stu-id="215d8-150">Europe/London</span></span>

<span data-ttu-id="215d8-151">Atlantik/Reykjavik</span><span class="sxs-lookup"><span data-stu-id="215d8-151">Atlantic/Reykjavik</span></span>

<span data-ttu-id="215d8-152">Europa/Berlin</span><span class="sxs-lookup"><span data-stu-id="215d8-152">Europe/Berlin</span></span>

<span data-ttu-id="215d8-153">Europa/Budapest</span><span class="sxs-lookup"><span data-stu-id="215d8-153">Europe/Budapest</span></span>

<span data-ttu-id="215d8-154">Europa/Paris</span><span class="sxs-lookup"><span data-stu-id="215d8-154">Europe/Paris</span></span>

<span data-ttu-id="215d8-155">Europa/Warschau</span><span class="sxs-lookup"><span data-stu-id="215d8-155">Europe/Warsaw</span></span>

<span data-ttu-id="215d8-156">Afrika/Lagos</span><span class="sxs-lookup"><span data-stu-id="215d8-156">Africa/Lagos</span></span>

<span data-ttu-id="215d8-157">Afrika/Windhoek</span><span class="sxs-lookup"><span data-stu-id="215d8-157">Africa/Windhoek</span></span>

<span data-ttu-id="215d8-158">Europa/Bukarest</span><span class="sxs-lookup"><span data-stu-id="215d8-158">Europe/Bucharest</span></span>

<span data-ttu-id="215d8-159">Asien/Beirut</span><span class="sxs-lookup"><span data-stu-id="215d8-159">Asia/Beirut</span></span>

<span data-ttu-id="215d8-160">Afrika/Kairo</span><span class="sxs-lookup"><span data-stu-id="215d8-160">Africa/Cairo</span></span>

<span data-ttu-id="215d8-161">Asien/Damaskus</span><span class="sxs-lookup"><span data-stu-id="215d8-161">Asia/Damascus</span></span>

<span data-ttu-id="215d8-162">Afrika/Johannesburg</span><span class="sxs-lookup"><span data-stu-id="215d8-162">Africa/Johannesburg</span></span>

<span data-ttu-id="215d8-163">Europa/Kiew</span><span class="sxs-lookup"><span data-stu-id="215d8-163">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="215d8-164">Europa/Istanbul</span><span class="sxs-lookup"><span data-stu-id="215d8-164">Europe/Istanbul</span></span>

<span data-ttu-id="215d8-165">Asien/Jerusalem</span><span class="sxs-lookup"><span data-stu-id="215d8-165">Asia/Jerusalem</span></span>

<span data-ttu-id="215d8-166">Asien/Amman</span><span class="sxs-lookup"><span data-stu-id="215d8-166">Asia/Amman</span></span>

<span data-ttu-id="215d8-167">Asien/Bagdad</span><span class="sxs-lookup"><span data-stu-id="215d8-167">Asia/Baghdad</span></span>

<span data-ttu-id="215d8-168">Europa/Kaliningrad</span><span class="sxs-lookup"><span data-stu-id="215d8-168">Europe/Kaliningrad</span></span>

<span data-ttu-id="215d8-169">Asien/Riad</span><span class="sxs-lookup"><span data-stu-id="215d8-169">Asia/Riyadh</span></span>

<span data-ttu-id="215d8-170">Afrika/Nairobi</span><span class="sxs-lookup"><span data-stu-id="215d8-170">Africa/Nairobi</span></span>

<span data-ttu-id="215d8-171">Asien/Teheran</span><span class="sxs-lookup"><span data-stu-id="215d8-171">Asia/Tehran</span></span>

<span data-ttu-id="215d8-172">Asien/Dubai</span><span class="sxs-lookup"><span data-stu-id="215d8-172">Asia/Dubai</span></span>

<span data-ttu-id="215d8-173">Asien/Baku</span><span class="sxs-lookup"><span data-stu-id="215d8-173">Asia/Baku</span></span>

<span data-ttu-id="215d8-174">Europa/Moskau</span><span class="sxs-lookup"><span data-stu-id="215d8-174">Europe/Moscow</span></span>

<span data-ttu-id="215d8-175">Indisch/Mauritius</span><span class="sxs-lookup"><span data-stu-id="215d8-175">Indian/Mauritius</span></span>

<span data-ttu-id="215d8-176">Asien/Tiflis</span><span class="sxs-lookup"><span data-stu-id="215d8-176">Asia/Tbilisi</span></span>

<span data-ttu-id="215d8-177">Asien/Eriwan</span><span class="sxs-lookup"><span data-stu-id="215d8-177">Asia/Yerevan</span></span>

<span data-ttu-id="215d8-178">Asien/Kabul</span><span class="sxs-lookup"><span data-stu-id="215d8-178">Asia/Kabul</span></span>

<span data-ttu-id="215d8-179">Asien/Karatschi</span><span class="sxs-lookup"><span data-stu-id="215d8-179">Asia/Karachi</span></span>

<span data-ttu-id="215d8-180">Asien/Taschkent</span><span class="sxs-lookup"><span data-stu-id="215d8-180">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="215d8-181">Asien/Kolkata</span><span class="sxs-lookup"><span data-stu-id="215d8-181">Asia/Kolkata</span></span>

<span data-ttu-id="215d8-182">Asien/Colombo</span><span class="sxs-lookup"><span data-stu-id="215d8-182">Asia/Colombo</span></span>

<span data-ttu-id="215d8-183">Asien/Katmandu</span><span class="sxs-lookup"><span data-stu-id="215d8-183">Asia/Kathmandu</span></span>

<span data-ttu-id="215d8-184">Asien/Astana (Almaty)</span><span class="sxs-lookup"><span data-stu-id="215d8-184">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="215d8-185">Asien/Dhaka</span><span class="sxs-lookup"><span data-stu-id="215d8-185">Asia/Dhaka</span></span>

<span data-ttu-id="215d8-186">Asien/Jekaterinburg</span><span class="sxs-lookup"><span data-stu-id="215d8-186">Asia/Yekaterinburg</span></span>

<span data-ttu-id="215d8-187">Asien/Yangon (Rangun)</span><span class="sxs-lookup"><span data-stu-id="215d8-187">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="215d8-188">Asien/Bangkok</span><span class="sxs-lookup"><span data-stu-id="215d8-188">Asia/Bangkok</span></span>

<span data-ttu-id="215d8-189">Asien/Nowosibirsk</span><span class="sxs-lookup"><span data-stu-id="215d8-189">Asia/Novosibirsk</span></span>

<span data-ttu-id="215d8-190">Asien/Shanghai</span><span class="sxs-lookup"><span data-stu-id="215d8-190">Asia/Shanghai</span></span>

<span data-ttu-id="215d8-191">Asien/Krasnojarsk</span><span class="sxs-lookup"><span data-stu-id="215d8-191">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="215d8-192">Asien/Singapur</span><span class="sxs-lookup"><span data-stu-id="215d8-192">Asia/Singapore</span></span>

<span data-ttu-id="215d8-193">Australien/Perth</span><span class="sxs-lookup"><span data-stu-id="215d8-193">Australia/Perth</span></span>

<span data-ttu-id="215d8-194">Asien/Taipeh</span><span class="sxs-lookup"><span data-stu-id="215d8-194">Asia/Taipei</span></span>

<span data-ttu-id="215d8-195">Asien/Ulan-Bator</span><span class="sxs-lookup"><span data-stu-id="215d8-195">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="215d8-196">Asien/Irkutsk</span><span class="sxs-lookup"><span data-stu-id="215d8-196">Asia/Irkutsk</span></span>

<span data-ttu-id="215d8-197">Asien/Tokio</span><span class="sxs-lookup"><span data-stu-id="215d8-197">Asia/Tokyo</span></span>

<span data-ttu-id="215d8-198">Asien/Seoul</span><span class="sxs-lookup"><span data-stu-id="215d8-198">Asia/Seoul</span></span>

<span data-ttu-id="215d8-199">Australien/Adelaide</span><span class="sxs-lookup"><span data-stu-id="215d8-199">Australia/Adelaide</span></span>

<span data-ttu-id="215d8-200">Australien/Darwin</span><span class="sxs-lookup"><span data-stu-id="215d8-200">Australia/Darwin</span></span>

<span data-ttu-id="215d8-201">Australien/Brisbane</span><span class="sxs-lookup"><span data-stu-id="215d8-201">Australia/Brisbane</span></span>

<span data-ttu-id="215d8-202">Australien/Sydney</span><span class="sxs-lookup"><span data-stu-id="215d8-202">Australia/Sydney</span></span>

<span data-ttu-id="215d8-203">Pazifik/Port_Moresby</span><span class="sxs-lookup"><span data-stu-id="215d8-203">Pacific/Port_Moresby</span></span>

<span data-ttu-id="215d8-204">Australien/Hobart</span><span class="sxs-lookup"><span data-stu-id="215d8-204">Australia/Hobart</span></span>

<span data-ttu-id="215d8-205">Asien/Jakutsk</span><span class="sxs-lookup"><span data-stu-id="215d8-205">Asia/Yakutsk</span></span>

<span data-ttu-id="215d8-206">Pazifik/Guadalcanal</span><span class="sxs-lookup"><span data-stu-id="215d8-206">Pacific/Guadalcanal</span></span>

<span data-ttu-id="215d8-207">Asien/Wladiwostok</span><span class="sxs-lookup"><span data-stu-id="215d8-207">Asia/Vladivostok</span></span>

<span data-ttu-id="215d8-208">Pazifik/Auckland</span><span class="sxs-lookup"><span data-stu-id="215d8-208">Pacific/Auckland</span></span>

<span data-ttu-id="215d8-209">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="215d8-209">Etc/GMT-12</span></span>

<span data-ttu-id="215d8-210">Pazifik/Fidschi</span><span class="sxs-lookup"><span data-stu-id="215d8-210">Pacific/Fiji</span></span>

<span data-ttu-id="215d8-211">Asien/Magadan</span><span class="sxs-lookup"><span data-stu-id="215d8-211">Asia/Magadan</span></span>

<span data-ttu-id="215d8-212">Pazifik/Tongatapu</span><span class="sxs-lookup"><span data-stu-id="215d8-212">Pacific/Tongatapu</span></span>

<span data-ttu-id="215d8-213">Pazifik/Apia</span><span class="sxs-lookup"><span data-stu-id="215d8-213">Pacific/Apia</span></span>

<span data-ttu-id="215d8-214">Pazifik/Kiritimati</span><span class="sxs-lookup"><span data-stu-id="215d8-214">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="215d8-215">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="215d8-215">JSON representation</span></span>

<span data-ttu-id="215d8-216">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="215d8-216">Here is a JSON representation of the resource</span></span>

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
