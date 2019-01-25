---
title: Ressourcentyp referencedObject
description: Beschreibt einen Verweis auf ein anderes Objekt in der gleichen Verzeichnis Definition definiert.
localization_priority: Normal
ms.openlocfilehash: dcec232335fdf3d447097ea1ae87fbc9ea676cfe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529320"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="c6e9b-103">Ressourcentyp referencedObject</span><span class="sxs-lookup"><span data-stu-id="c6e9b-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6e9b-104">Beschreibt einen Verweis auf ein anderes Objekt in der gleichen [Verzeichnis Definition](synchronization-directorydefinition.md)definiert.</span><span class="sxs-lookup"><span data-stu-id="c6e9b-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c6e9b-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c6e9b-105">Properties</span></span>

| <span data-ttu-id="c6e9b-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6e9b-106">Property</span></span>                   | <span data-ttu-id="c6e9b-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c6e9b-107">Type</span></span>                      | <span data-ttu-id="c6e9b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6e9b-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="c6e9b-109">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="c6e9b-109">referencedObjectName</span></span>        |<span data-ttu-id="c6e9b-110">String</span><span class="sxs-lookup"><span data-stu-id="c6e9b-110">String</span></span>                     |<span data-ttu-id="c6e9b-111">Name des Objekts verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="c6e9b-111">Name of the referenced object.</span></span> <span data-ttu-id="c6e9b-112">Muss eines der Objekte in der [Definition des Verzeichnisses](synchronization-directorydefinition.md)übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="c6e9b-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="c6e9b-113">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="c6e9b-113">referencedProperty</span></span>          |<span data-ttu-id="c6e9b-114">String</span><span class="sxs-lookup"><span data-stu-id="c6e9b-114">String</span></span>                     |<span data-ttu-id="c6e9b-115">**Derzeit nicht unterstützt**.</span><span class="sxs-lookup"><span data-stu-id="c6e9b-115">**Currently not supported**.</span></span> <span data-ttu-id="c6e9b-116">Der Name der Eigenschaft in das Objekt verwiesen wird, der, das Wert für die als Referenz verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="c6e9b-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6e9b-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c6e9b-117">JSON representation</span></span>

<span data-ttu-id="c6e9b-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c6e9b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-referencedobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
            
