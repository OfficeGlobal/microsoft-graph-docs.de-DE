---
title: Ressourcentyp scheduleInformation
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: e84505ee2f30a5b7b52e9d5b589b8bb24d9a4c95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521908"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="78291-104">Ressourcentyp scheduleInformation</span><span class="sxs-lookup"><span data-stu-id="78291-104">scheduleInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="78291-105">Stellt die Verfügbarkeit von einem Benutzer, eine Verteilerliste oder eine Ressource für einen angegebenen Zeitraum dar.</span><span class="sxs-lookup"><span data-stu-id="78291-105">Represents the availability of a user, distribution list, or resource for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="78291-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78291-106">Properties</span></span>
| <span data-ttu-id="78291-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78291-107">Property</span></span>     | <span data-ttu-id="78291-108">Typ</span><span class="sxs-lookup"><span data-stu-id="78291-108">Type</span></span>   |<span data-ttu-id="78291-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78291-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78291-110">availabilityView</span><span class="sxs-lookup"><span data-stu-id="78291-110">availabilityView</span></span> |<span data-ttu-id="78291-111">String</span><span class="sxs-lookup"><span data-stu-id="78291-111">String</span></span> |<span data-ttu-id="78291-112">Stellt eine Ansicht der Verfügbarkeit aller Elemente in zusammengeführte `scheduleItems`.</span><span class="sxs-lookup"><span data-stu-id="78291-112">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="78291-113">Die Ansicht Zeitfenster besteht aus.</span><span class="sxs-lookup"><span data-stu-id="78291-113">The view consists of time slots.</span></span> <span data-ttu-id="78291-114">Verfügbarkeit während jedes Zeitintervall wird mit angegeben: `0`= frei, `1`mit Vorbehalt = `2`= beschäftigt, `3`= abwesend, `4`= arbeiten an anderer Stelle.</span><span class="sxs-lookup"><span data-stu-id="78291-114">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="78291-115">error</span><span class="sxs-lookup"><span data-stu-id="78291-115">error</span></span> |[<span data-ttu-id="78291-116">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="78291-116">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="78291-117">Fehlerinformationen versucht, die die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="78291-117">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="78291-118">scheduleId</span><span class="sxs-lookup"><span data-stu-id="78291-118">scheduleId</span></span> |<span data-ttu-id="78291-119">String</span><span class="sxs-lookup"><span data-stu-id="78291-119">String</span></span> |<span data-ttu-id="78291-120">Eine SMTP-Adresse des Benutzers, der Verteilerliste oder der Ressource, die eine Instanz des **ScheduleInformation**identifiziert.</span><span class="sxs-lookup"><span data-stu-id="78291-120">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="78291-121">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="78291-121">scheduleItems</span></span> |<span data-ttu-id="78291-122">[von ScheduleItem](scheduleitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="78291-122">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="78291-123">Enthält die Elemente, die die Verfügbarkeit des Benutzers oder der Ressource zu beschreiben.</span><span class="sxs-lookup"><span data-stu-id="78291-123">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="78291-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="78291-124">workingHours</span></span> |[<span data-ttu-id="78291-125">workingHours</span><span class="sxs-lookup"><span data-stu-id="78291-125">workingHours</span></span>](workinghours.md) |<span data-ttu-id="78291-126">Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="78291-126">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="78291-127">Diese werden als Teil des Benutzers [MailboxSettings](mailboxsettings.md)festgelegt.</span><span class="sxs-lookup"><span data-stu-id="78291-127">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="78291-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="78291-128">JSON representation</span></span>

<span data-ttu-id="78291-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="78291-129">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
