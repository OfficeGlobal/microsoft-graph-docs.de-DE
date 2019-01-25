---
title: Ressourcentyp attributeMappingFunctionSchema
description: Beschreibt eine Funktion, die in eine Zuordnung Attribut verwendet werden kann, während der Synchronisierung Werte umgewandelt.
localization_priority: Normal
ms.openlocfilehash: e2c0139f7c797c3f519cc638561b09f611018b28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511982"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="449fa-103">Ressourcentyp attributeMappingFunctionSchema</span><span class="sxs-lookup"><span data-stu-id="449fa-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="449fa-104">Beschreibt eine Funktion, die in eine [Zuordnung zwischen Attributen](synchronization-attributemapping.md) verwendet werden kann, während der Synchronisierung Werte umgewandelt.</span><span class="sxs-lookup"><span data-stu-id="449fa-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="449fa-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="449fa-105">Methods</span></span>

| <span data-ttu-id="449fa-106">Methode</span><span class="sxs-lookup"><span data-stu-id="449fa-106">Method</span></span>           | <span data-ttu-id="449fa-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="449fa-107">Return Type</span></span>    |<span data-ttu-id="449fa-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="449fa-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="449fa-109">List</span><span class="sxs-lookup"><span data-stu-id="449fa-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="449fa-110">[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="449fa-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="449fa-111">Liste unterstützt Attribut Zuordnungsfunktionen.</span><span class="sxs-lookup"><span data-stu-id="449fa-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="449fa-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="449fa-112">Properties</span></span>

| <span data-ttu-id="449fa-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="449fa-113">Property</span></span>                   | <span data-ttu-id="449fa-114">Typ</span><span class="sxs-lookup"><span data-stu-id="449fa-114">Type</span></span>                      | <span data-ttu-id="449fa-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="449fa-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="449fa-116">name</span><span class="sxs-lookup"><span data-stu-id="449fa-116">name</span></span>                        |<span data-ttu-id="449fa-117">String</span><span class="sxs-lookup"><span data-stu-id="449fa-117">String</span></span>                    |<span data-ttu-id="449fa-118">Name des Operators.</span><span class="sxs-lookup"><span data-stu-id="449fa-118">Operator name.</span></span> |
|<span data-ttu-id="449fa-119">parameters</span><span class="sxs-lookup"><span data-stu-id="449fa-119">parameters</span></span>                  |<span data-ttu-id="449fa-120">[AttributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="449fa-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="449fa-121">Auflistung von Funktionsparametern.</span><span class="sxs-lookup"><span data-stu-id="449fa-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="449fa-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="449fa-122">JSON representation</span></span>

<span data-ttu-id="449fa-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="449fa-123">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingfunctionschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
