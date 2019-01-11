---
title: timeZoneInformation-Ressourcentyp
description: Stellt eine Zeitzone dar. Unterstützte Format ist Windows und bei der Internet Assigned Numbers Authority (IANA) Zeit Zone (auch bekannt als Olson-Zeitzone)
localization_priority: Normal
ms.openlocfilehash: dc53cca34ef9c6a53a39394cbba8be4e1baca662
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839739"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="996e2-104">timeZoneInformation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="996e2-104">timeZoneInformation resource type</span></span>

> <span data-ttu-id="996e2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="996e2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="996e2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="996e2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="996e2-107">Stellt eine Zeitzone dar.</span><span class="sxs-lookup"><span data-stu-id="996e2-107">Represents a time zone.</span></span> <span data-ttu-id="996e2-108">Das unterstützte Format ist Windows und auch das Format der [IANA-Zeitzone (Internet Assigned Numbers Authority)](https://www.iana.org/time-zones) (auch bekannt als Olson-Zeitzone) wenn das derzeitige bekannte Problem behoben ist.</span><span class="sxs-lookup"><span data-stu-id="996e2-108">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="996e2-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="996e2-109">Properties</span></span>
| <span data-ttu-id="996e2-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="996e2-110">Property</span></span>     | <span data-ttu-id="996e2-111">Typ</span><span class="sxs-lookup"><span data-stu-id="996e2-111">Type</span></span>   |<span data-ttu-id="996e2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="996e2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="996e2-113">Alias</span><span class="sxs-lookup"><span data-stu-id="996e2-113">alias</span></span>|<span data-ttu-id="996e2-114">String</span><span class="sxs-lookup"><span data-stu-id="996e2-114">string</span></span>|<span data-ttu-id="996e2-115">Ein Bezeichner für die Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="996e2-115">An identifier for the time zone.</span></span>|
|<span data-ttu-id="996e2-116">displayName</span><span class="sxs-lookup"><span data-stu-id="996e2-116">displayName</span></span>|<span data-ttu-id="996e2-117">string</span><span class="sxs-lookup"><span data-stu-id="996e2-117">string</span></span>|<span data-ttu-id="996e2-118">Eine Anzeigezeichenfolge, die die Zeitzone darstellt.</span><span class="sxs-lookup"><span data-stu-id="996e2-118">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="996e2-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="996e2-119">JSON representation</span></span>

<span data-ttu-id="996e2-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="996e2-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
