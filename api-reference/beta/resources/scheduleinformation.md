---
title: Ressourcentyp scheduleInformation
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: e535f5c2b47e810fc767cb29d0b24f28ed3c7bf0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828707"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="32797-104">Ressourcentyp scheduleInformation</span><span class="sxs-lookup"><span data-stu-id="32797-104">scheduleInformation resource type</span></span>

 > <span data-ttu-id="32797-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="32797-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32797-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="32797-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="32797-107">Stellt die Verfügbarkeit von einem Benutzer, eine Verteilerliste oder eine Ressource für einen angegebenen Zeitraum dar.</span><span class="sxs-lookup"><span data-stu-id="32797-107">Represents the availability of a user, distribution list, or resource for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="32797-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="32797-108">Properties</span></span>
| <span data-ttu-id="32797-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32797-109">Property</span></span>     | <span data-ttu-id="32797-110">Typ</span><span class="sxs-lookup"><span data-stu-id="32797-110">Type</span></span>   |<span data-ttu-id="32797-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32797-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32797-112">availabilityView</span><span class="sxs-lookup"><span data-stu-id="32797-112">availabilityView</span></span> |<span data-ttu-id="32797-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32797-113">String</span></span> |<span data-ttu-id="32797-114">Stellt eine Ansicht der Verfügbarkeit aller Elemente in zusammengeführte `scheduleItems`.</span><span class="sxs-lookup"><span data-stu-id="32797-114">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="32797-115">Die Ansicht Zeitfenster besteht aus.</span><span class="sxs-lookup"><span data-stu-id="32797-115">The view consists of time slots.</span></span> <span data-ttu-id="32797-116">Verfügbarkeit während jedes Zeitintervall wird mit angegeben: `0`= frei, `1`mit Vorbehalt = `2`= beschäftigt, `3`= abwesend, `4`= arbeiten an anderer Stelle.</span><span class="sxs-lookup"><span data-stu-id="32797-116">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="32797-117">error</span><span class="sxs-lookup"><span data-stu-id="32797-117">error</span></span> |[<span data-ttu-id="32797-118">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="32797-118">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="32797-119">Fehlerinformationen versucht, die die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="32797-119">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="32797-120">scheduleId</span><span class="sxs-lookup"><span data-stu-id="32797-120">scheduleId</span></span> |<span data-ttu-id="32797-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32797-121">String</span></span> |<span data-ttu-id="32797-122">Eine SMTP-Adresse des Benutzers, der Verteilerliste oder der Ressource, die eine Instanz des **ScheduleInformation**identifiziert.</span><span class="sxs-lookup"><span data-stu-id="32797-122">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="32797-123">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="32797-123">scheduleItems</span></span> |<span data-ttu-id="32797-124">[von ScheduleItem](scheduleitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="32797-124">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="32797-125">Enthält die Elemente, die die Verfügbarkeit des Benutzers oder der Ressource zu beschreiben.</span><span class="sxs-lookup"><span data-stu-id="32797-125">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="32797-126">workingHours</span><span class="sxs-lookup"><span data-stu-id="32797-126">workingHours</span></span> |[<span data-ttu-id="32797-127">workingHours</span><span class="sxs-lookup"><span data-stu-id="32797-127">workingHours</span></span>](workinghours.md) |<span data-ttu-id="32797-128">Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="32797-128">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="32797-129">Diese werden als Teil des Benutzers [MailboxSettings](mailboxsettings.md)festgelegt.</span><span class="sxs-lookup"><span data-stu-id="32797-129">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="32797-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="32797-130">JSON representation</span></span>

<span data-ttu-id="32797-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="32797-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
