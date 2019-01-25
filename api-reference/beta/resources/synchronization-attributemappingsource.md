---
title: Ressourcentyp attributeMappingSource
description: 'Definiert, wie ein Wert sein sollte extrahiert haben (oder transformiert), aus dem Quellobjekt. Beispielsweise kann ein einfaches Wert aus einem gegebenen Attribut für das Quellobjekt sein oder einen komplexeren Ausdruck Zeichenfolge Verkettung/Extraction/Ersatz von basierend auf verschiedene Attribute für Datenquellen sind möglich. '
localization_priority: Normal
ms.openlocfilehash: 1d15cd82c0a58ac8bdd3ac5805abc166322f27fe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510407"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="906e5-104">Ressourcentyp attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="906e5-104">attributeMappingSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="906e5-105">Definiert, wie ein Wert sein sollte extrahiert haben (oder transformiert), aus dem Quellobjekt.</span><span class="sxs-lookup"><span data-stu-id="906e5-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="906e5-106">Beispielsweise kann ein einfaches Wert aus einem gegebenen Attribut für das Quellobjekt sein oder einen komplexeren Ausdruck Zeichenfolge Verkettung/Extraction/Ersatz von basierend auf verschiedene Attribute für Datenquellen sind möglich.</span><span class="sxs-lookup"><span data-stu-id="906e5-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="906e5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="906e5-107">Properties</span></span>

| <span data-ttu-id="906e5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="906e5-108">Property</span></span>              | <span data-ttu-id="906e5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="906e5-109">Type</span></span>                      | <span data-ttu-id="906e5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="906e5-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="906e5-111">Ausdruck</span><span class="sxs-lookup"><span data-stu-id="906e5-111">expression</span></span>             |<span data-ttu-id="906e5-112">String</span><span class="sxs-lookup"><span data-stu-id="906e5-112">String</span></span>                     |<span data-ttu-id="906e5-113">Entsprechende Ausdruck Darstellung dieses **AttributeMappingSource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="906e5-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="906e5-114">name</span><span class="sxs-lookup"><span data-stu-id="906e5-114">name</span></span>                   |<span data-ttu-id="906e5-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="906e5-115">String</span></span>                     |<span data-ttu-id="906e5-116">Name-Parameter der Zuordnungsquelle.</span><span class="sxs-lookup"><span data-stu-id="906e5-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="906e5-117">Je nach der Wert der **Type** -Eigenschaft kann dies der Name der Funktion, die den Namen der Source-Attribut oder einen konstanten Wert geeignet sein.</span><span class="sxs-lookup"><span data-stu-id="906e5-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="906e5-118">parameters</span><span class="sxs-lookup"><span data-stu-id="906e5-118">parameters</span></span>             |<span data-ttu-id="906e5-119">[StringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="906e5-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="906e5-120">Wenn dieses Objekt eine Funktion darstellt, werden Funktionsparameter aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="906e5-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="906e5-121">Parameter bestehen aus **AttributeMappingSource** Objekte selbst komplexe Ausdrücke zulassen.</span><span class="sxs-lookup"><span data-stu-id="906e5-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="906e5-122">**Typ** ist nicht `Function`, wird diese Eigenschaft Array Null/leer sein.</span><span class="sxs-lookup"><span data-stu-id="906e5-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="906e5-123">type</span><span class="sxs-lookup"><span data-stu-id="906e5-123">type</span></span>                   | <span data-ttu-id="906e5-124">String</span><span class="sxs-lookup"><span data-stu-id="906e5-124">String</span></span>                    |<span data-ttu-id="906e5-125">Der Typ des in diesem Attribut Zuordnungsquelle.</span><span class="sxs-lookup"><span data-stu-id="906e5-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="906e5-126">Mögliche Werte sind: `Attribute`, `Constant` und `Function`.</span><span class="sxs-lookup"><span data-stu-id="906e5-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="906e5-127">Der Standardwert lautet `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="906e5-127">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="906e5-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="906e5-128">JSON representation</span></span>

<span data-ttu-id="906e5-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="906e5-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
  "expression": "String",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"}],
  "type": "String"
}
```

## <a name="json-examples"></a><span data-ttu-id="906e5-130">Beispiele für JSON</span><span class="sxs-lookup"><span data-stu-id="906e5-130">JSON Examples</span></span>

<span data-ttu-id="906e5-131">Einfache-Attribut zum Zuordnen</span><span class="sxs-lookup"><span data-stu-id="906e5-131">Simple attribute to attribute mapping</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
    "expression": "[mail]",
    "name": "mail",
    "type": "Attribute"
}
```

<span data-ttu-id="906e5-132">Extrahieren von ersten 8 Zeichen aus dem Ausdruck</span><span class="sxs-lookup"><span data-stu-id="906e5-132">Expression extracting first 8 characters from the source attribute</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
 {
    "expression": "Mid([userPrincipalName], 1, 8)",
    "name": "Mid",
    "parameters": [
        {
            "key": "source",
            "value": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            }
        },
        {
            "key": "start",
            "value": {
                "expression": "\"1\"",
                "name": "1",
                "parameters": [],
                "type": "Constant"
            }
        },
        {
            "key": "length",
            "value": {
                "expression": "\"8\"",
                "name": "8",
                "parameters": [],
                "type": "Constant"
            }
        }
    ],
    "type": "Function"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingsource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
