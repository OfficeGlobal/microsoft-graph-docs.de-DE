---
title: Ressourcentyp freeBusyError
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: f1ff7717034798830a610b35dbbff5c987cf7371
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529845"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="c408d-104">Ressourcentyp freeBusyError</span><span class="sxs-lookup"><span data-stu-id="c408d-104">freeBusyError resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="c408d-105">Stellt Informationen zum Fehler versucht, die die Verfügbarkeit von einem Benutzer, eine Verteilerliste oder eine Ressource erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="c408d-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="c408d-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c408d-106">Properties</span></span>
| <span data-ttu-id="c408d-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c408d-107">Property</span></span>     | <span data-ttu-id="c408d-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c408d-108">Type</span></span>   |<span data-ttu-id="c408d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c408d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c408d-110">message</span><span class="sxs-lookup"><span data-stu-id="c408d-110">message</span></span> |<span data-ttu-id="c408d-111">String</span><span class="sxs-lookup"><span data-stu-id="c408d-111">String</span></span> |<span data-ttu-id="c408d-112">Beschreibt den Fehler.</span><span class="sxs-lookup"><span data-stu-id="c408d-112">Describes the error.</span></span> |
|<span data-ttu-id="c408d-113">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c408d-113">responseCode</span></span> |<span data-ttu-id="c408d-114">String</span><span class="sxs-lookup"><span data-stu-id="c408d-114">String</span></span> |<span data-ttu-id="c408d-115">Der Antwortcode von Abfragen für die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c408d-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c408d-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c408d-116">JSON representation</span></span>

<span data-ttu-id="c408d-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c408d-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/freebusyerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
