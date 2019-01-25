---
title: timeZoneInformation-Ressourcentyp
description: Stellt eine Zeitzone dar. Unterstützte Format ist Windows und bei der Internet Assigned Numbers Authority (IANA) Zeit Zone (auch bekannt als Olson-Zeitzone)
localization_priority: Normal
ms.openlocfilehash: a63721de7ed4e8c3f3b74ce5954a88ee71a95414
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526774"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="2c37f-104">timeZoneInformation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2c37f-104">timeZoneInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c37f-105">Stellt eine Zeitzone dar.</span><span class="sxs-lookup"><span data-stu-id="2c37f-105">Represents a time zone.</span></span> <span data-ttu-id="2c37f-106">Das unterstützte Format ist Windows und auch das Format der [IANA-Zeitzone (Internet Assigned Numbers Authority)](https://www.iana.org/time-zones) (auch bekannt als Olson-Zeitzone) wenn das derzeitige bekannte Problem behoben ist.</span><span class="sxs-lookup"><span data-stu-id="2c37f-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="2c37f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2c37f-107">Properties</span></span>
| <span data-ttu-id="2c37f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c37f-108">Property</span></span>     | <span data-ttu-id="2c37f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2c37f-109">Type</span></span>   |<span data-ttu-id="2c37f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c37f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c37f-111">Alias</span><span class="sxs-lookup"><span data-stu-id="2c37f-111">alias</span></span>|<span data-ttu-id="2c37f-112">String</span><span class="sxs-lookup"><span data-stu-id="2c37f-112">string</span></span>|<span data-ttu-id="2c37f-113">Ein Bezeichner für die Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="2c37f-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="2c37f-114">displayName</span><span class="sxs-lookup"><span data-stu-id="2c37f-114">displayName</span></span>|<span data-ttu-id="2c37f-115">string</span><span class="sxs-lookup"><span data-stu-id="2c37f-115">string</span></span>|<span data-ttu-id="2c37f-116">Eine Anzeigezeichenfolge, die die Zeitzone darstellt.</span><span class="sxs-lookup"><span data-stu-id="2c37f-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c37f-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2c37f-117">JSON representation</span></span>

<span data-ttu-id="2c37f-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2c37f-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timezoneinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
