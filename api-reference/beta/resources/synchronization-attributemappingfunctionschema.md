---
title: Ressourcentyp attributeMappingFunctionSchema
description: Beschreibt eine Funktion, die in eine Zuordnung Attribut verwendet werden kann, während der Synchronisierung Werte umgewandelt.
localization_priority: Normal
ms.openlocfilehash: 7273534d281d8ea5eaf3709b530776295cd9c767
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822162"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="55686-103">Ressourcentyp attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="55686-103">attributeMappingFunctionSchema resource type</span></span>

> <span data-ttu-id="55686-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="55686-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55686-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="55686-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55686-106">Beschreibt eine Funktion, die in eine [Zuordnung zwischen Attributen](synchronization-attributemapping.md) verwendet werden kann, während der Synchronisierung Werte umgewandelt.</span><span class="sxs-lookup"><span data-stu-id="55686-106">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="55686-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="55686-107">Methods</span></span>

| <span data-ttu-id="55686-108">Methode</span><span class="sxs-lookup"><span data-stu-id="55686-108">Method</span></span>           | <span data-ttu-id="55686-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="55686-109">Return Type</span></span>    |<span data-ttu-id="55686-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55686-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55686-111">List</span><span class="sxs-lookup"><span data-stu-id="55686-111">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="55686-112">[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="55686-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="55686-113">Liste unterstützt Attribut Zuordnungsfunktionen.</span><span class="sxs-lookup"><span data-stu-id="55686-113">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="55686-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="55686-114">Properties</span></span>

| <span data-ttu-id="55686-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="55686-115">Property</span></span>                   | <span data-ttu-id="55686-116">Typ</span><span class="sxs-lookup"><span data-stu-id="55686-116">Type</span></span>                      | <span data-ttu-id="55686-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55686-117">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="55686-118">name</span><span class="sxs-lookup"><span data-stu-id="55686-118">name</span></span>                        |<span data-ttu-id="55686-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55686-119">String</span></span>                    |<span data-ttu-id="55686-120">Name des Operators.</span><span class="sxs-lookup"><span data-stu-id="55686-120">Operator name.</span></span> |
|<span data-ttu-id="55686-121">parameters</span><span class="sxs-lookup"><span data-stu-id="55686-121">parameters</span></span>                  |<span data-ttu-id="55686-122">[AttributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="55686-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="55686-123">Auflistung von Funktionsparametern.</span><span class="sxs-lookup"><span data-stu-id="55686-123">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55686-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="55686-124">JSON representation</span></span>

<span data-ttu-id="55686-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="55686-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
