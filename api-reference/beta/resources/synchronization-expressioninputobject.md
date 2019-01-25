---
title: Ressourcentyp expressionInputObject
description: 'Stellt ein Objekt als Eingabe Testdaten verwendet werden bei der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion ausführt Ausdruck in Bezug auf.'
localization_priority: Normal
ms.openlocfilehash: 3e631102505408b955404c4badb33b98f314236f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510778"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="60377-103">Ressourcentyp expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="60377-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60377-104">Stellt ein Objekt als Eingabe Testdaten verwendet werden bei der [SynchronizationSchema: ParseExpression](../api/synchronization_synchronizationschema_parseexpression.md) Aktion ausführt Ausdruck in Bezug auf.</span><span class="sxs-lookup"><span data-stu-id="60377-104">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="60377-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="60377-105">Properties</span></span>
| <span data-ttu-id="60377-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60377-106">Property</span></span>     | <span data-ttu-id="60377-107">Typ</span><span class="sxs-lookup"><span data-stu-id="60377-107">Type</span></span>   |<span data-ttu-id="60377-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60377-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60377-109">definition</span><span class="sxs-lookup"><span data-stu-id="60377-109">definition</span></span>|[<span data-ttu-id="60377-110">Sind</span><span class="sxs-lookup"><span data-stu-id="60377-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="60377-111">Definition des Test-Objekts.</span><span class="sxs-lookup"><span data-stu-id="60377-111">Definition of the test object.</span></span>|
|<span data-ttu-id="60377-112">properties</span><span class="sxs-lookup"><span data-stu-id="60377-112">properties</span></span>|<span data-ttu-id="60377-113">[StringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="60377-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="60377-114">Eigenschaftswerte des Test-Objekts.</span><span class="sxs-lookup"><span data-stu-id="60377-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60377-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="60377-115">JSON representation</span></span>

<span data-ttu-id="60377-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="60377-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-expressioninputobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
