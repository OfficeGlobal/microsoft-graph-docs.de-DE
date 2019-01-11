---
title: Ressourcentyp expressionInputObject
description: 'Stellt ein Objekt als Eingabe Testdaten verwendet werden bei der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion ausführt Ausdruck in Bezug auf.'
localization_priority: Normal
ms.openlocfilehash: acf0fa5125d863224de6df76d46109b9888f8ddf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820111"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="231f1-103">Ressourcentyp expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="231f1-103">expressionInputObject resource type</span></span>

> <span data-ttu-id="231f1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="231f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="231f1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="231f1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="231f1-106">Stellt ein Objekt als Eingabe Testdaten verwendet werden bei der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion ausführt Ausdruck in Bezug auf.</span><span class="sxs-lookup"><span data-stu-id="231f1-106">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="231f1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="231f1-107">Properties</span></span>
| <span data-ttu-id="231f1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="231f1-108">Property</span></span>     | <span data-ttu-id="231f1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="231f1-109">Type</span></span>   |<span data-ttu-id="231f1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="231f1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="231f1-111">definition</span><span class="sxs-lookup"><span data-stu-id="231f1-111">definition</span></span>|[<span data-ttu-id="231f1-112">Sind</span><span class="sxs-lookup"><span data-stu-id="231f1-112">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="231f1-113">Definition des Test-Objekts.</span><span class="sxs-lookup"><span data-stu-id="231f1-113">Definition of the test object.</span></span>|
|<span data-ttu-id="231f1-114">properties</span><span class="sxs-lookup"><span data-stu-id="231f1-114">properties</span></span>|<span data-ttu-id="231f1-115">[StringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="231f1-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="231f1-116">Eigenschaftswerte des Test-Objekts.</span><span class="sxs-lookup"><span data-stu-id="231f1-116">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="231f1-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="231f1-117">JSON representation</span></span>

<span data-ttu-id="231f1-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="231f1-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
