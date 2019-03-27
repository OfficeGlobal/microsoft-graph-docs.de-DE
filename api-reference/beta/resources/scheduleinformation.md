---
title: scheduleInformation-Ressourcentyp
description: 'Stellt die Verfügbarkeit eines Benutzers, einer Verteilerliste oder einer Ressource für einen bestimmten Zeitraum dar. '
localization_priority: Normal
ms.openlocfilehash: 6c809b9cf600d9b620164f253d2a37e57a0f5d4d
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869491"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="6ba00-103">scheduleInformation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6ba00-103">scheduleInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="6ba00-104">Stellt die Verfügbarkeit eines Benutzers, einer Verteilerliste oder einer Ressource (Raum oder Equipment) für einen bestimmten Zeitraum dar.</span><span class="sxs-lookup"><span data-stu-id="6ba00-104">Represents the availability of a user, distribution list, or resource (room or equipment) for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="6ba00-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ba00-105">Properties</span></span>
| <span data-ttu-id="6ba00-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ba00-106">Property</span></span>     | <span data-ttu-id="6ba00-107">Typ</span><span class="sxs-lookup"><span data-stu-id="6ba00-107">Type</span></span>   |<span data-ttu-id="6ba00-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ba00-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ba00-109">availabilityView</span><span class="sxs-lookup"><span data-stu-id="6ba00-109">availabilityView</span></span> |<span data-ttu-id="6ba00-110">String</span><span class="sxs-lookup"><span data-stu-id="6ba00-110">String</span></span> |<span data-ttu-id="6ba00-111">Stellt eine zusammengeführte Ansicht der Verfügbarkeit aller Elemente in `scheduleItems`dar.</span><span class="sxs-lookup"><span data-stu-id="6ba00-111">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="6ba00-112">Die Ansicht besteht aus Zeitschlitzen.</span><span class="sxs-lookup"><span data-stu-id="6ba00-112">The view consists of time slots.</span></span> <span data-ttu-id="6ba00-113">Die Verfügbarkeit in jedem Zeitschlitz wird mit `0`: = Free `1`, = zaghaft `2`, = busy `3`, = Abwesenheit, `4`= arbeiten an einem anderen Ort angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6ba00-113">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="6ba00-114">error</span><span class="sxs-lookup"><span data-stu-id="6ba00-114">error</span></span> |[<span data-ttu-id="6ba00-115">freeBusyError</span><span class="sxs-lookup"><span data-stu-id="6ba00-115">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="6ba00-116">Fehlerinformationen aus dem Versuch, die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource abzurufen.</span><span class="sxs-lookup"><span data-stu-id="6ba00-116">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="6ba00-117">scheduleId</span><span class="sxs-lookup"><span data-stu-id="6ba00-117">scheduleId</span></span> |<span data-ttu-id="6ba00-118">String</span><span class="sxs-lookup"><span data-stu-id="6ba00-118">String</span></span> |<span data-ttu-id="6ba00-119">Eine SMTP-Adresse des Benutzers, der Verteilerliste oder der Ressource, die eine Instanz von **scheduleInformation**identifiziert.</span><span class="sxs-lookup"><span data-stu-id="6ba00-119">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="6ba00-120">scheduleItems</span><span class="sxs-lookup"><span data-stu-id="6ba00-120">scheduleItems</span></span> |<span data-ttu-id="6ba00-121">[scheduleItem](scheduleitem.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ba00-121">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="6ba00-122">Enthält die Elemente, die die Verfügbarkeit des Benutzers oder der Ressource beschreiben.</span><span class="sxs-lookup"><span data-stu-id="6ba00-122">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="6ba00-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="6ba00-123">workingHours</span></span> |[<span data-ttu-id="6ba00-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="6ba00-124">workingHours</span></span>](workinghours.md) |<span data-ttu-id="6ba00-125">Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet.</span><span class="sxs-lookup"><span data-stu-id="6ba00-125">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="6ba00-126">Diese werden als Teil des [Mailbox Settings](mailboxsettings.md)des Benutzers festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6ba00-126">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6ba00-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ba00-127">JSON representation</span></span>

<span data-ttu-id="6ba00-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ba00-128">The following is a JSON representation of the resource.</span></span>

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
