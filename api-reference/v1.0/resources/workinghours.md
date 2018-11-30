---
title: workingHours-Ressourcentyp
description: Stellt die Wochentage und Zeiten in einer bestimmten Zeitzone dar, an bzw. zu denen der Benutzer arbeitet.
ms.openlocfilehash: 23b24536ffc86feb261a17c0847e5c15ffc25922
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019507"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="6c576-103">workingHours-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6c576-103">workingHours resource type</span></span>

<span data-ttu-id="6c576-104">Stellt die Wochentage und Zeiten in einer bestimmten Zeitzone dar, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="6c576-104">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="6c576-105">Zugriff auf die Arbeitszeiten eines Benutzers ist bei der Aktivitäts- oder Ressourcenplanung hilfreich.</span><span class="sxs-lookup"><span data-stu-id="6c576-105">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="6c576-106">Sie können die Arbeitszeiten eines Benutzers als Teil der [Postfacheinstellungen](mailboxsettings.md) des Benutzers [abrufen](../api/user-get-mailboxsettings.md#request-3) und [festlegen](../api/user-update-mailboxsettings.md#request-2) .</span><span class="sxs-lookup"><span data-stu-id="6c576-106">You can [get](../api/user-get-mailboxsettings.md#request-3) and [set](../api/user-update-mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="6c576-107">Sie können für die Arbeitszeiten auch eine andere Zeitzone als die für Ihren Outlook-Client festgelegte Zeitzone festlegen.</span><span class="sxs-lookup"><span data-stu-id="6c576-107">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="6c576-108">Dies kann zum Beispiel hilfreich sein, wenn Sie in eine andere Zeitzone reisen.</span><span class="sxs-lookup"><span data-stu-id="6c576-108">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="6c576-109">Sie können den Outlook-Client auf</span><span class="sxs-lookup"><span data-stu-id="6c576-109">You can set the Outlook client</span></span>  
<span data-ttu-id="6c576-110">die Zielzeitzone festlegen, sodass die Outlook-Zeitwerte in der lokalen Zeit angezeigt werden, solange Sie sich in dieser Zeitzone befinden.</span><span class="sxs-lookup"><span data-stu-id="6c576-110">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="6c576-111">Wenn andere Personen Arbeitsbesprechungen mit Ihnen an Ihrem üblichen Arbeitsplatz anfordern, können sie sich an Ihre Arbeitszeiten in der jeweiligen Zeitzone halten.</span><span class="sxs-lookup"><span data-stu-id="6c576-111">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="6c576-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6c576-112">Properties</span></span>
| <span data-ttu-id="6c576-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c576-113">Property</span></span>     | <span data-ttu-id="6c576-114">Typ</span><span class="sxs-lookup"><span data-stu-id="6c576-114">Type</span></span>   |<span data-ttu-id="6c576-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c576-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6c576-116">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="6c576-116">daysOfWeek</span></span> | <span data-ttu-id="6c576-117">DayOfWeek-Auflistung</span><span class="sxs-lookup"><span data-stu-id="6c576-117">dayOfWeek collection</span></span> | <span data-ttu-id="6c576-118">Die Wochentage, an denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="6c576-118">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="6c576-119">startTime</span><span class="sxs-lookup"><span data-stu-id="6c576-119">startTime</span></span> | <span data-ttu-id="6c576-120">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6c576-120">Edm.TimeOfDay</span></span> | <span data-ttu-id="6c576-121">Die Tageszeit, zu der der Benutzer zu arbeiten beginnt.</span><span class="sxs-lookup"><span data-stu-id="6c576-121">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="6c576-122">endTime</span><span class="sxs-lookup"><span data-stu-id="6c576-122">endTime</span></span> | <span data-ttu-id="6c576-123">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6c576-123">Edm.TimeOfDay</span></span> | <span data-ttu-id="6c576-124">Die Tageszeit, zu der der Benutzer zu arbeiten aufhört.</span><span class="sxs-lookup"><span data-stu-id="6c576-124">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="6c576-125">timeZone</span><span class="sxs-lookup"><span data-stu-id="6c576-125">timeZone</span></span> | [<span data-ttu-id="6c576-126">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="6c576-126">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="6c576-127">Die Zeitzone, für die die Arbeitszeiten gelten.</span><span class="sxs-lookup"><span data-stu-id="6c576-127">The time zone to which the working hours apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6c576-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6c576-128">JSON representation</span></span>

<span data-ttu-id="6c576-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6c576-129">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/workinghours.md/microsoft.graph.workingHours/daysOfWeek:
      Inconsistent types between parameter (String) and table (Object)"
  ],
  "tocPath": ""
}-->