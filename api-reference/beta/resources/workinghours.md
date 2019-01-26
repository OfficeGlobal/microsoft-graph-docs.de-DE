---
title: workingHours-Ressourcentyp
description: Stellt die Wochentage und Zeiten in einer bestimmten Zeitzone dar, an bzw. zu denen der Benutzer arbeitet.
localization_priority: Normal
ms.openlocfilehash: 8d0c0c96838af63cd0e1c665d23e54938b4ea34d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573823"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="2ba3b-103">workingHours-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2ba3b-103">workingHours resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ba3b-104">Stellt die Wochentage und Zeiten in einer bestimmten Zeitzone dar, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-104">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="2ba3b-105">Zugriff auf die Arbeitszeiten eines Benutzers ist bei der Aktivitäts- oder Ressourcenplanung hilfreich.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-105">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="2ba3b-106">Sie können die Arbeitszeiten eines Benutzers als Teil der [Postfacheinstellungen](mailboxsettings.md) des Benutzers [abrufen](../api/user-get-mailboxsettings.md#request-3) und [festlegen](../api/user-update-mailboxsettings.md#request-2) .</span><span class="sxs-lookup"><span data-stu-id="2ba3b-106">You can [get](../api/user-get-mailboxsettings.md#request-3) and [set](../api/user-update-mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="2ba3b-107">Sie können für die Arbeitszeiten auch eine andere Zeitzone als die für Ihren Outlook-Client festgelegte Zeitzone festlegen.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-107">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="2ba3b-108">Dies kann zum Beispiel hilfreich sein, wenn Sie in eine andere Zeitzone reisen.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-108">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="2ba3b-109">Sie können den Outlook-Client auf</span><span class="sxs-lookup"><span data-stu-id="2ba3b-109">You can set the Outlook client</span></span>  
<span data-ttu-id="2ba3b-110">die Zielzeitzone festlegen, sodass die Outlook-Zeitwerte in der lokalen Zeit angezeigt werden, solange Sie sich in dieser Zeitzone befinden.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-110">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="2ba3b-111">Wenn andere Personen Arbeitsbesprechungen mit Ihnen an Ihrem üblichen Arbeitsplatz anfordern, können sie sich an Ihre Arbeitszeiten in der jeweiligen Zeitzone halten.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-111">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="2ba3b-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2ba3b-112">Properties</span></span>
| <span data-ttu-id="2ba3b-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ba3b-113">Property</span></span>     | <span data-ttu-id="2ba3b-114">Typ</span><span class="sxs-lookup"><span data-stu-id="2ba3b-114">Type</span></span>   |<span data-ttu-id="2ba3b-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ba3b-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2ba3b-116">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="2ba3b-116">daysOfWeek</span></span> | <span data-ttu-id="2ba3b-117">DayOfWeek-Auflistung</span><span class="sxs-lookup"><span data-stu-id="2ba3b-117">dayOfWeek collection</span></span> | <span data-ttu-id="2ba3b-118">Die Wochentage, an denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-118">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="2ba3b-119">startTime</span><span class="sxs-lookup"><span data-stu-id="2ba3b-119">startTime</span></span> | <span data-ttu-id="2ba3b-120">Zeichenfolge (TimeOfDay)</span><span class="sxs-lookup"><span data-stu-id="2ba3b-120">String (TimeOfDay)</span></span> | <span data-ttu-id="2ba3b-121">Die Tageszeit, zu der der Benutzer zu arbeiten beginnt.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-121">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="2ba3b-122">endTime</span><span class="sxs-lookup"><span data-stu-id="2ba3b-122">endTime</span></span> | <span data-ttu-id="2ba3b-123">Zeichenfolge (TimeOfDay)</span><span class="sxs-lookup"><span data-stu-id="2ba3b-123">String (TimeOfDay)</span></span> | <span data-ttu-id="2ba3b-124">Die Tageszeit, zu der der Benutzer zu arbeiten aufhört.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-124">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="2ba3b-125">timeZone</span><span class="sxs-lookup"><span data-stu-id="2ba3b-125">timeZone</span></span> | [<span data-ttu-id="2ba3b-126">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="2ba3b-126">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="2ba3b-127">Die Zeitzone, für die die Arbeitszeiten gelten.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-127">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="2ba3b-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2ba3b-128">JSON representation</span></span>

<span data-ttu-id="2ba3b-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2ba3b-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["dayOfWeek"],
  "startTime": "String (TimeOfDay)",
  "endTime": "String (TimeOfDay)",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/workinghours.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
