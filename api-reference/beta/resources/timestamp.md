---
title: Zeitstempel Ressourcentyp
description: Datum und Uhrzeit Informationen für einen Punkt in der Zeit.
ms.openlocfilehash: 24326f0c104dd4ee2be80016ce798cc843288975
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061681"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="b52d8-103">Zeitstempel Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b52d8-103">timeStamp resource type</span></span>

> <span data-ttu-id="b52d8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b52d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b52d8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b52d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b52d8-106">Datum und Uhrzeit Informationen für einen Punkt in der Zeit.</span><span class="sxs-lookup"><span data-stu-id="b52d8-106">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b52d8-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b52d8-107">JSON representation</span></span>

<span data-ttu-id="b52d8-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b52d8-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b52d8-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b52d8-109">Properties</span></span>
| <span data-ttu-id="b52d8-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b52d8-110">Property</span></span>     | <span data-ttu-id="b52d8-111">Typ</span><span class="sxs-lookup"><span data-stu-id="b52d8-111">Type</span></span>   |<span data-ttu-id="b52d8-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b52d8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b52d8-113">date</span><span class="sxs-lookup"><span data-stu-id="b52d8-113">date</span></span>|<span data-ttu-id="b52d8-114">Datum</span><span class="sxs-lookup"><span data-stu-id="b52d8-114">Date</span></span>|<span data-ttu-id="b52d8-115">Das der Zeitstempel Datumsteil.</span><span class="sxs-lookup"><span data-stu-id="b52d8-115">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="b52d8-116">time</span><span class="sxs-lookup"><span data-stu-id="b52d8-116">time</span></span>|<span data-ttu-id="b52d8-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b52d8-117">TimeOfDay</span></span>|<span data-ttu-id="b52d8-118">Den Zeitbereich des der Zeitstempel.</span><span class="sxs-lookup"><span data-stu-id="b52d8-118">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="b52d8-119">timeZone</span><span class="sxs-lookup"><span data-stu-id="b52d8-119">timeZone</span></span>|<span data-ttu-id="b52d8-120">String</span><span class="sxs-lookup"><span data-stu-id="b52d8-120">String</span></span>|<span data-ttu-id="b52d8-121">Der Timezone-Teil der Zeitstempel, der einem der 24 Länge Bereiche in der ganzen Welt ist.</span><span class="sxs-lookup"><span data-stu-id="b52d8-121">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->