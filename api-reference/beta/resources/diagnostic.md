---
title: Diagnose Ressourcentyp
description: Informationen zu einer Fehlermeldung oder einer Warnung für eine OneNote-Operation.
localization_priority: Normal
ms.openlocfilehash: ef495374f84e0df887198b38a5c8488987a59343
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509504"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="af4f2-103">Diagnose Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="af4f2-103">diagnostic resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af4f2-104">Informationen zu einer Fehlermeldung oder einer Warnung für eine OneNote-Operation.</span><span class="sxs-lookup"><span data-stu-id="af4f2-104">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af4f2-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="af4f2-105">JSON representation</span></span>

<span data-ttu-id="af4f2-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="af4f2-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="af4f2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="af4f2-107">Properties</span></span>
| <span data-ttu-id="af4f2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af4f2-108">Property</span></span>     | <span data-ttu-id="af4f2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="af4f2-109">Type</span></span>   |<span data-ttu-id="af4f2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af4f2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af4f2-111">message</span><span class="sxs-lookup"><span data-stu-id="af4f2-111">message</span></span>|<span data-ttu-id="af4f2-112">String</span><span class="sxs-lookup"><span data-stu-id="af4f2-112">String</span></span>|<span data-ttu-id="af4f2-113">Die Nachricht, beschreibt die Bedingung, die den Fehler oder eine Warnung ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="af4f2-113">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="af4f2-114">url</span><span class="sxs-lookup"><span data-stu-id="af4f2-114">url</span></span>|<span data-ttu-id="af4f2-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af4f2-115">String</span></span>|<span data-ttu-id="af4f2-116">Die Verknüpfung mit der Dokumentation für dieses Problem.</span><span class="sxs-lookup"><span data-stu-id="af4f2-116">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/diagnostic.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
