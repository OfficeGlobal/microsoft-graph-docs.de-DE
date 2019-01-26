---
title: Ressourcentyp parseExpressionResponse
description: 'Stellt die Antwort von der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion.'
localization_priority: Normal
ms.openlocfilehash: fc37c963e9c9588241d84570edc73a933eec49fc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572878"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="2d04d-103">Ressourcentyp parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="2d04d-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d04d-104">Stellt die Antwort von der [SynchronizationSchema: ParseExpression](../api/synchronization-synchronizationschema-parseexpression.md) Aktion.</span><span class="sxs-lookup"><span data-stu-id="2d04d-104">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="2d04d-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2d04d-105">Properties</span></span>
| <span data-ttu-id="2d04d-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d04d-106">Property</span></span>     | <span data-ttu-id="2d04d-107">Typ</span><span class="sxs-lookup"><span data-stu-id="2d04d-107">Type</span></span>   |<span data-ttu-id="2d04d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d04d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d04d-109">error</span><span class="sxs-lookup"><span data-stu-id="2d04d-109">error</span></span>| <span data-ttu-id="2d04d-110">publicError</span><span class="sxs-lookup"><span data-stu-id="2d04d-110">publicError</span></span> |<span data-ttu-id="2d04d-111">Fehlerdetails, wenn die Auswertung von Ausdrücken ein Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="2d04d-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="2d04d-112">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="2d04d-112">evaluationResult</span></span>|<span data-ttu-id="2d04d-113">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="2d04d-113">String collection</span></span>|<span data-ttu-id="2d04d-114">Eine Auflistung von Werten, die mit der Auswertung des Ausdrucks.</span><span class="sxs-lookup"><span data-stu-id="2d04d-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="2d04d-115">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="2d04d-115">evaluationSucceeded</span></span>|<span data-ttu-id="2d04d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d04d-116">Boolean</span></span>|<span data-ttu-id="2d04d-117">`true`Wenn die Auswertung erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="2d04d-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="2d04d-118">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="2d04d-118">parsedExpression</span></span>|[<span data-ttu-id="2d04d-119">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="2d04d-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="2d04d-120">Ein [AttributeMappingSource](synchronization-attributemappingsource.md) -Objekt, das den analysierten Ausdruck darstellt.</span><span class="sxs-lookup"><span data-stu-id="2d04d-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="2d04d-121">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="2d04d-121">parsingSucceeded</span></span>|<span data-ttu-id="2d04d-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d04d-122">Boolean</span></span>|<span data-ttu-id="2d04d-123">`true`Wenn der Ausdruck erfolgreich analysiert wurde.</span><span class="sxs-lookup"><span data-stu-id="2d04d-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d04d-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2d04d-124">JSON representation</span></span>

<span data-ttu-id="2d04d-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2d04d-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-parseexpressionresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
