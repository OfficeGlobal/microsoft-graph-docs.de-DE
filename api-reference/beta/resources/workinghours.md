---
title: workingHours-Ressourcentyp
description: Stellt die Wochentage und Zeiten in einer bestimmten Zeitzone dar, an bzw. zu denen der Benutzer arbeitet.
localization_priority: Normal
ms.openlocfilehash: d34da38ad1a007f6c63154cb496006585df95c13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885739"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="46f51-103">workingHours-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="46f51-103">workingHours resource type</span></span>

> <span data-ttu-id="46f51-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="46f51-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46f51-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46f51-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46f51-106">Stellt die Wochentage und Zeiten in einer bestimmten Zeitzone dar, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="46f51-106">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="46f51-107">Zugriff auf die Arbeitszeiten eines Benutzers ist bei der Aktivitäts- oder Ressourcenplanung hilfreich.</span><span class="sxs-lookup"><span data-stu-id="46f51-107">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="46f51-108">Sie können die Arbeitszeiten eines Benutzers als Teil der [Postfacheinstellungen](mailboxsettings.md) des Benutzers [abrufen](../api/user-get-mailboxsettings.md#request-3) und [festlegen](../api/user-update-mailboxsettings.md#request-2) .</span><span class="sxs-lookup"><span data-stu-id="46f51-108">You can [get](../api/user-get-mailboxsettings.md#request-3) and [set](../api/user-update-mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="46f51-109">Sie können für die Arbeitszeiten auch eine andere Zeitzone als die für Ihren Outlook-Client festgelegte Zeitzone festlegen.</span><span class="sxs-lookup"><span data-stu-id="46f51-109">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="46f51-110">Dies kann zum Beispiel hilfreich sein, wenn Sie in eine andere Zeitzone reisen.</span><span class="sxs-lookup"><span data-stu-id="46f51-110">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="46f51-111">Sie können den Outlook-Client auf</span><span class="sxs-lookup"><span data-stu-id="46f51-111">You can set the Outlook client</span></span>  
<span data-ttu-id="46f51-112">die Zielzeitzone festlegen, sodass die Outlook-Zeitwerte in der lokalen Zeit angezeigt werden, solange Sie sich in dieser Zeitzone befinden.</span><span class="sxs-lookup"><span data-stu-id="46f51-112">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="46f51-113">Wenn andere Personen Arbeitsbesprechungen mit Ihnen an Ihrem üblichen Arbeitsplatz anfordern, können sie sich an Ihre Arbeitszeiten in der jeweiligen Zeitzone halten.</span><span class="sxs-lookup"><span data-stu-id="46f51-113">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="46f51-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46f51-114">Properties</span></span>
| <span data-ttu-id="46f51-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46f51-115">Property</span></span>     | <span data-ttu-id="46f51-116">Typ</span><span class="sxs-lookup"><span data-stu-id="46f51-116">Type</span></span>   |<span data-ttu-id="46f51-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46f51-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46f51-118">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="46f51-118">daysOfWeek</span></span> | <span data-ttu-id="46f51-119">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="46f51-119">String collection</span></span> | <span data-ttu-id="46f51-120">Die Wochentage, an denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="46f51-120">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="46f51-121">startTime</span><span class="sxs-lookup"><span data-stu-id="46f51-121">startTime</span></span> | <span data-ttu-id="46f51-122">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="46f51-122">Edm.TimeOfDay</span></span> | <span data-ttu-id="46f51-123">Die Tageszeit, zu der der Benutzer zu arbeiten beginnt.</span><span class="sxs-lookup"><span data-stu-id="46f51-123">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="46f51-124">endTime</span><span class="sxs-lookup"><span data-stu-id="46f51-124">endTime</span></span> | <span data-ttu-id="46f51-125">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="46f51-125">Edm.TimeOfDay</span></span> | <span data-ttu-id="46f51-126">Die Tageszeit, zu der der Benutzer zu arbeiten aufhört.</span><span class="sxs-lookup"><span data-stu-id="46f51-126">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="46f51-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="46f51-127">timeZone</span></span> | [<span data-ttu-id="46f51-128">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="46f51-128">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="46f51-129">Die Zeitzone, für die die Arbeitszeiten gelten.</span><span class="sxs-lookup"><span data-stu-id="46f51-129">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="46f51-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46f51-130">JSON representation</span></span>

<span data-ttu-id="46f51-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="46f51-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
