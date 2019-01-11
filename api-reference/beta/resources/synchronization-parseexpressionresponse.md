---
title: Ressourcentyp parseExpressionResponse
description: 'Stellt die Antwort von der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion.'
localization_priority: Normal
ms.openlocfilehash: 550a46b0c27c2ca8d2d4c01baa975d8a204546f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832949"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="ab440-103">Ressourcentyp parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="ab440-103">parseExpressionResponse resource type</span></span>

> <span data-ttu-id="ab440-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ab440-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab440-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ab440-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab440-106">Stellt die Antwort von der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion.</span><span class="sxs-lookup"><span data-stu-id="ab440-106">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="ab440-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ab440-107">Properties</span></span>
| <span data-ttu-id="ab440-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ab440-108">Property</span></span>     | <span data-ttu-id="ab440-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ab440-109">Type</span></span>   |<span data-ttu-id="ab440-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab440-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab440-111">error</span><span class="sxs-lookup"><span data-stu-id="ab440-111">error</span></span>|<span data-ttu-id="ab440-112">OData.Error</span><span class="sxs-lookup"><span data-stu-id="ab440-112">odata.error</span></span>|<span data-ttu-id="ab440-113">Fehlerdetails, wenn die Auswertung von Ausdrücken ein Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="ab440-113">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="ab440-114">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="ab440-114">evaluationResult</span></span>|<span data-ttu-id="ab440-115">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="ab440-115">String collection</span></span>|<span data-ttu-id="ab440-116">Eine Auflistung von Werten, die mit der Auswertung des Ausdrucks.</span><span class="sxs-lookup"><span data-stu-id="ab440-116">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="ab440-117">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="ab440-117">evaluationSucceeded</span></span>|<span data-ttu-id="ab440-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab440-118">Boolean</span></span>|<span data-ttu-id="ab440-119">`true`Wenn die Auswertung erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="ab440-119">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="ab440-120">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="ab440-120">parsedExpression</span></span>|[<span data-ttu-id="ab440-121">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="ab440-121">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="ab440-122">Ein [AttributeMappingSource](synchronization-attributemappingsource.md) -Objekt, das den analysierten Ausdruck darstellt.</span><span class="sxs-lookup"><span data-stu-id="ab440-122">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="ab440-123">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="ab440-123">parsingSucceeded</span></span>|<span data-ttu-id="ab440-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab440-124">Boolean</span></span>|<span data-ttu-id="ab440-125">`true`Wenn der Ausdruck erfolgreich analysiert wurde.</span><span class="sxs-lookup"><span data-stu-id="ab440-125">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab440-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ab440-126">JSON representation</span></span>

<span data-ttu-id="ab440-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ab440-127">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
