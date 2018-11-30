---
title: Ressourcentyp attributeMappingFunctionSchema
description: Beschreibt eine Funktion, die in eine Zuordnung Attribut verwendet werden kann, während der Synchronisierung Werte umgewandelt.
ms.openlocfilehash: 9760669bb29700bfa79c1cd375857b4fd673879b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062042"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="4654e-103">Ressourcentyp attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="4654e-103">attributeMappingFunctionSchema resource type</span></span>

> <span data-ttu-id="4654e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4654e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4654e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4654e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4654e-106">Beschreibt eine Funktion, die in eine [Zuordnung zwischen Attributen](synchronization-attributemapping.md) verwendet werden kann, während der Synchronisierung Werte umgewandelt.</span><span class="sxs-lookup"><span data-stu-id="4654e-106">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="4654e-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="4654e-107">Methods</span></span>

| <span data-ttu-id="4654e-108">Methode</span><span class="sxs-lookup"><span data-stu-id="4654e-108">Method</span></span>           | <span data-ttu-id="4654e-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4654e-109">Return Type</span></span>    |<span data-ttu-id="4654e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4654e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4654e-111">List</span><span class="sxs-lookup"><span data-stu-id="4654e-111">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="4654e-112">[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4654e-112">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="4654e-113">Liste unterstützt Attribut Zuordnungsfunktionen.</span><span class="sxs-lookup"><span data-stu-id="4654e-113">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="4654e-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4654e-114">Properties</span></span>

| <span data-ttu-id="4654e-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4654e-115">Property</span></span>                   | <span data-ttu-id="4654e-116">Typ</span><span class="sxs-lookup"><span data-stu-id="4654e-116">Type</span></span>                      | <span data-ttu-id="4654e-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4654e-117">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="4654e-118">name</span><span class="sxs-lookup"><span data-stu-id="4654e-118">name</span></span>                        |<span data-ttu-id="4654e-119">String</span><span class="sxs-lookup"><span data-stu-id="4654e-119">String</span></span>                    |<span data-ttu-id="4654e-120">Name des Operators.</span><span class="sxs-lookup"><span data-stu-id="4654e-120">Operator name.</span></span> |
|<span data-ttu-id="4654e-121">parameters</span><span class="sxs-lookup"><span data-stu-id="4654e-121">parameters</span></span>                  |<span data-ttu-id="4654e-122">[AttributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4654e-122">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="4654e-123">Auflistung von Funktionsparametern.</span><span class="sxs-lookup"><span data-stu-id="4654e-123">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4654e-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4654e-124">JSON representation</span></span>

<span data-ttu-id="4654e-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4654e-125">The following is a JSON representation of the resource.</span></span>

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