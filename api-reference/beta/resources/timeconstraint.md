---
title: Ressourcentyp „timeConstraint“
description: Schränkt Vorschläge für Besprechungstermine entsprechend der angegebenen Art der Aktivität und der offenen Zeitfenster auf bestimmte Stunden und Tage der Woche ein.
localization_priority: Normal
ms.openlocfilehash: 6e3cc56f1495eae60bb84c458caa25c79557e033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832907"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="85a3f-103">Ressourcentyp „timeConstraint“</span><span class="sxs-lookup"><span data-stu-id="85a3f-103">timeConstraint resource type</span></span>

> <span data-ttu-id="85a3f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="85a3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85a3f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85a3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85a3f-106">Schränkt Vorschläge für Besprechungstermine entsprechend der angegebenen Art der Aktivität und der offenen Zeitfenster auf bestimmte Stunden und Tage der Woche ein.</span><span class="sxs-lookup"><span data-stu-id="85a3f-106">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85a3f-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85a3f-107">JSON representation</span></span>

<span data-ttu-id="85a3f-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="85a3f-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="85a3f-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85a3f-109">Properties</span></span>
| <span data-ttu-id="85a3f-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85a3f-110">Property</span></span>     | <span data-ttu-id="85a3f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="85a3f-111">Type</span></span>   |<span data-ttu-id="85a3f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85a3f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85a3f-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="85a3f-113">activityDomain</span></span>|<span data-ttu-id="85a3f-114">String</span><span class="sxs-lookup"><span data-stu-id="85a3f-114">String</span></span>|<span data-ttu-id="85a3f-p102">Die Art der Aktivität. Diese Angabe ist optional. Mögliche Werte sind: `work`, `personal`, `unrestricted` oder `unknown`.</span><span class="sxs-lookup"><span data-stu-id="85a3f-p102">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="85a3f-117">timeslots</span><span class="sxs-lookup"><span data-stu-id="85a3f-117">timeslots</span></span>|<span data-ttu-id="85a3f-118">[timeSlot](timeslot.md) collection</span><span class="sxs-lookup"><span data-stu-id="85a3f-118">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="85a3f-119">Ein Array von Zeitfenstern</span><span class="sxs-lookup"><span data-stu-id="85a3f-119">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
