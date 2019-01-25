---
title: Ressourcentyp convertIdResult
description: Das Ergebnis einer ID formatkonvertierung, die von der Funktion TranslateExchangeIds durchgeführt.
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516525"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="cc184-103">Ressourcentyp convertIdResult</span><span class="sxs-lookup"><span data-stu-id="cc184-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc184-104">Das Ergebnis einer ID formatkonvertierung, die von der Funktion [TranslateExchangeIds](../api/user-translateexchangeids.md) durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="cc184-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="cc184-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cc184-105">Properties</span></span>

| <span data-ttu-id="cc184-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cc184-106">Property</span></span> | <span data-ttu-id="cc184-107">Typ</span><span class="sxs-lookup"><span data-stu-id="cc184-107">Type</span></span> | <span data-ttu-id="cc184-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc184-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="cc184-109">SourceId</span><span class="sxs-lookup"><span data-stu-id="cc184-109">sourceId</span></span> | <span data-ttu-id="cc184-110">String</span><span class="sxs-lookup"><span data-stu-id="cc184-110">String</span></span> | <span data-ttu-id="cc184-111">Der Bezeichner, der konvertiert wurde.</span><span class="sxs-lookup"><span data-stu-id="cc184-111">The identifier that was converted.</span></span> <span data-ttu-id="cc184-112">Dieser Wert ist der ursprüngliche, nicht konvertierten Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="cc184-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="cc184-113">targetId</span><span class="sxs-lookup"><span data-stu-id="cc184-113">targetId</span></span> | <span data-ttu-id="cc184-114">String</span><span class="sxs-lookup"><span data-stu-id="cc184-114">String</span></span> | <span data-ttu-id="cc184-115">Der Bezeichner konvertierte.</span><span class="sxs-lookup"><span data-stu-id="cc184-115">The converted identifier.</span></span> <span data-ttu-id="cc184-116">Dieser Wert ist nicht vorhanden, wenn die Konvertierung fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="cc184-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="cc184-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="cc184-117">errorDetails</span></span> | [<span data-ttu-id="cc184-118">Allgemeiner Fehler</span><span class="sxs-lookup"><span data-stu-id="cc184-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="cc184-119">Ein Error-Objekt zurück, der den Grund für die Konvertierungsfehler angibt.</span><span class="sxs-lookup"><span data-stu-id="cc184-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="cc184-120">Dieser Wert ist nicht vorhanden, wenn die Konvertierung erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="cc184-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cc184-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cc184-121">JSON representation</span></span>

<span data-ttu-id="cc184-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cc184-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/convertidresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
