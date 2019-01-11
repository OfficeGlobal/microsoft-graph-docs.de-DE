---
title: Ressourcentyp attributeMappingSource
description: 'Definiert, wie ein Wert sein sollte extrahiert haben (oder transformiert), aus dem Quellobjekt. Beispielsweise kann ein einfaches Wert aus einem gegebenen Attribut für das Quellobjekt sein oder einen komplexeren Ausdruck Zeichenfolge Verkettung/Extraction/Ersatz von basierend auf verschiedene Attribute für Datenquellen sind möglich. '
localization_priority: Normal
ms.openlocfilehash: a7c1493f27f34230d4305fe95b2d2f03a5ad25e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825011"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="f1da6-104">Ressourcentyp attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="f1da6-104">attributeMappingSource resource type</span></span>

> <span data-ttu-id="f1da6-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f1da6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1da6-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1da6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f1da6-107">Definiert, wie ein Wert sein sollte extrahiert haben (oder transformiert), aus dem Quellobjekt.</span><span class="sxs-lookup"><span data-stu-id="f1da6-107">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="f1da6-108">Beispielsweise kann ein einfaches Wert aus einem gegebenen Attribut für das Quellobjekt sein oder einen komplexeren Ausdruck Zeichenfolge Verkettung/Extraction/Ersatz von basierend auf verschiedene Attribute für Datenquellen sind möglich.</span><span class="sxs-lookup"><span data-stu-id="f1da6-108">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="f1da6-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f1da6-109">Properties</span></span>

| <span data-ttu-id="f1da6-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1da6-110">Property</span></span>              | <span data-ttu-id="f1da6-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f1da6-111">Type</span></span>                      | <span data-ttu-id="f1da6-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1da6-112">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="f1da6-113">Ausdruck</span><span class="sxs-lookup"><span data-stu-id="f1da6-113">expression</span></span>             |<span data-ttu-id="f1da6-114">String</span><span class="sxs-lookup"><span data-stu-id="f1da6-114">String</span></span>                     |<span data-ttu-id="f1da6-115">Entsprechende Ausdruck Darstellung dieses **AttributeMappingSource** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1da6-115">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="f1da6-116">name</span><span class="sxs-lookup"><span data-stu-id="f1da6-116">name</span></span>                   |<span data-ttu-id="f1da6-117">String</span><span class="sxs-lookup"><span data-stu-id="f1da6-117">String</span></span>                     |<span data-ttu-id="f1da6-118">Name-Parameter der Zuordnungsquelle.</span><span class="sxs-lookup"><span data-stu-id="f1da6-118">Name parameter of the mapping source.</span></span> <span data-ttu-id="f1da6-119">Je nach der Wert der **Type** -Eigenschaft kann dies der Name der Funktion, die den Namen der Source-Attribut oder einen konstanten Wert geeignet sein.</span><span class="sxs-lookup"><span data-stu-id="f1da6-119">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="f1da6-120">parameters</span><span class="sxs-lookup"><span data-stu-id="f1da6-120">parameters</span></span>             |<span data-ttu-id="f1da6-121">[StringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f1da6-121">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="f1da6-122">Wenn dieses Objekt eine Funktion darstellt, werden Funktionsparameter aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="f1da6-122">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="f1da6-123">Parameter bestehen aus **AttributeMappingSource** Objekte selbst komplexe Ausdrücke zulassen.</span><span class="sxs-lookup"><span data-stu-id="f1da6-123">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="f1da6-124">**Typ** ist nicht `Function`, wird diese Eigenschaft Array Null/leer sein.</span><span class="sxs-lookup"><span data-stu-id="f1da6-124">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="f1da6-125">type</span><span class="sxs-lookup"><span data-stu-id="f1da6-125">type</span></span>                   | <span data-ttu-id="f1da6-126">String</span><span class="sxs-lookup"><span data-stu-id="f1da6-126">String</span></span>                    |<span data-ttu-id="f1da6-127">Der Typ des in diesem Attribut Zuordnungsquelle.</span><span class="sxs-lookup"><span data-stu-id="f1da6-127">The type of this attribute mapping source.</span></span> <span data-ttu-id="f1da6-128">Mögliche Werte sind: `Attribute`, `Constant` und `Function`.</span><span class="sxs-lookup"><span data-stu-id="f1da6-128">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="f1da6-129">Der Standardwert lautet `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="f1da6-129">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="f1da6-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f1da6-130">JSON representation</span></span>

<span data-ttu-id="f1da6-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f1da6-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="f1da6-132">Beispiele für JSON</span><span class="sxs-lookup"><span data-stu-id="f1da6-132">JSON Examples</span></span>

<span data-ttu-id="f1da6-133">Einfache-Attribut zum Zuordnen</span><span class="sxs-lookup"><span data-stu-id="f1da6-133">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="f1da6-134">Extrahieren von ersten 8 Zeichen aus dem Ausdruck</span><span class="sxs-lookup"><span data-stu-id="f1da6-134">Expression extracting first 8 characters from the source attribute</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
