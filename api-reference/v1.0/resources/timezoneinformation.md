---
title: timeZoneInformation-Ressourcentyp
description: Stellt eine Zeitzone dar. Unterstützte Format ist Windows und bei der Internet Assigned Numbers Authority (IANA) Zeit Zone (auch bekannt als Olson-Zeitzone)
ms.openlocfilehash: de80ed293af834d299be5f9543c5c3bedde7a540
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016108"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="a5833-104">timeZoneInformation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a5833-104">timeZoneInformation resource type</span></span>


<span data-ttu-id="a5833-105">Stellt eine Zeitzone dar.</span><span class="sxs-lookup"><span data-stu-id="a5833-105">Represents a time zone.</span></span> <span data-ttu-id="a5833-106">Das unterstützte Format ist Windows und auch das Format der [IANA-Zeitzone (Internet Assigned Numbers Authority)](https://www.iana.org/time-zones) (auch bekannt als Olson-Zeitzone) wenn das derzeitige bekannte Problem behoben ist.</span><span class="sxs-lookup"><span data-stu-id="a5833-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="a5833-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a5833-107">Properties</span></span>
| <span data-ttu-id="a5833-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5833-108">Property</span></span>     | <span data-ttu-id="a5833-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a5833-109">Type</span></span>   |<span data-ttu-id="a5833-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5833-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5833-111">Alias</span><span class="sxs-lookup"><span data-stu-id="a5833-111">alias</span></span>|<span data-ttu-id="a5833-112">String</span><span class="sxs-lookup"><span data-stu-id="a5833-112">string</span></span>|<span data-ttu-id="a5833-113">Ein Bezeichner für die Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="a5833-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="a5833-114">displayName</span><span class="sxs-lookup"><span data-stu-id="a5833-114">displayName</span></span>|<span data-ttu-id="a5833-115">string</span><span class="sxs-lookup"><span data-stu-id="a5833-115">string</span></span>|<span data-ttu-id="a5833-116">Eine Anzeigezeichenfolge, die die Zeitzone darstellt.</span><span class="sxs-lookup"><span data-stu-id="a5833-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5833-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a5833-117">JSON representation</span></span>

<span data-ttu-id="a5833-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a5833-118">Here is a JSON representation of the resource.</span></span>

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