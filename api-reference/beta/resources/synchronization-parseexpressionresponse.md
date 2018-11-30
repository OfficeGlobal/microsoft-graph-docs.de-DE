---
title: Ressourcentyp parseExpressionResponse
description: 'Stellt die Antwort von der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion.'
ms.openlocfilehash: 625df0ca16135eaa35c5b679c79dea582c4012e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065190"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="63cb1-103">Ressourcentyp parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="63cb1-103">parseExpressionResponse resource type</span></span>

> <span data-ttu-id="63cb1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="63cb1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63cb1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="63cb1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63cb1-106">Stellt die Antwort von der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion.</span><span class="sxs-lookup"><span data-stu-id="63cb1-106">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="63cb1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="63cb1-107">Properties</span></span>
| <span data-ttu-id="63cb1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="63cb1-108">Property</span></span>     | <span data-ttu-id="63cb1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="63cb1-109">Type</span></span>   |<span data-ttu-id="63cb1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63cb1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63cb1-111">error</span><span class="sxs-lookup"><span data-stu-id="63cb1-111">error</span></span>|<span data-ttu-id="63cb1-112">OData.Error</span><span class="sxs-lookup"><span data-stu-id="63cb1-112">odata.error</span></span>|<span data-ttu-id="63cb1-113">Fehlerdetails, wenn die Auswertung von Ausdrücken ein Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="63cb1-113">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="63cb1-114">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="63cb1-114">evaluationResult</span></span>|<span data-ttu-id="63cb1-115">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="63cb1-115">String collection</span></span>|<span data-ttu-id="63cb1-116">Eine Auflistung von Werten, die mit der Auswertung des Ausdrucks.</span><span class="sxs-lookup"><span data-stu-id="63cb1-116">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="63cb1-117">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="63cb1-117">evaluationSucceeded</span></span>|<span data-ttu-id="63cb1-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="63cb1-118">Boolean</span></span>|<span data-ttu-id="63cb1-119">`true`Wenn die Auswertung erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="63cb1-119">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="63cb1-120">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="63cb1-120">parsedExpression</span></span>|[<span data-ttu-id="63cb1-121">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="63cb1-121">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="63cb1-122">Ein [AttributeMappingSource](synchronization-attributemappingsource.md) -Objekt, das den analysierten Ausdruck darstellt.</span><span class="sxs-lookup"><span data-stu-id="63cb1-122">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="63cb1-123">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="63cb1-123">parsingSucceeded</span></span>|<span data-ttu-id="63cb1-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="63cb1-124">Boolean</span></span>|<span data-ttu-id="63cb1-125">`true`Wenn der Ausdruck erfolgreich analysiert wurde.</span><span class="sxs-lookup"><span data-stu-id="63cb1-125">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63cb1-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="63cb1-126">JSON representation</span></span>

<span data-ttu-id="63cb1-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="63cb1-127">The following is a JSON representation of the resource.</span></span>

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