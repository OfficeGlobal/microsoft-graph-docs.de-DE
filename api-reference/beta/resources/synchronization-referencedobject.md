---
title: Ressourcentyp referencedObject
description: Beschreibt einen Verweis auf ein anderes Objekt in der gleichen Verzeichnis Definition definiert.
localization_priority: Normal
ms.openlocfilehash: 5a2aa2dcc358c856c18ea2ce9871ec634194ce54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821035"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="87008-103">Ressourcentyp referencedObject</span><span class="sxs-lookup"><span data-stu-id="87008-103">referencedObject resource type</span></span>

> <span data-ttu-id="87008-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87008-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87008-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87008-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87008-106">Beschreibt einen Verweis auf ein anderes Objekt in der gleichen [Verzeichnis Definition](synchronization-directorydefinition.md)definiert.</span><span class="sxs-lookup"><span data-stu-id="87008-106">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="87008-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="87008-107">Properties</span></span>

| <span data-ttu-id="87008-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87008-108">Property</span></span>                   | <span data-ttu-id="87008-109">Typ</span><span class="sxs-lookup"><span data-stu-id="87008-109">Type</span></span>                      | <span data-ttu-id="87008-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87008-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="87008-111">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="87008-111">referencedObjectName</span></span>        |<span data-ttu-id="87008-112">String</span><span class="sxs-lookup"><span data-stu-id="87008-112">String</span></span>                     |<span data-ttu-id="87008-113">Name des Objekts verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="87008-113">Name of the referenced object.</span></span> <span data-ttu-id="87008-114">Muss eines der Objekte in der [Definition des Verzeichnisses](synchronization-directorydefinition.md)übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="87008-114">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="87008-115">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="87008-115">referencedProperty</span></span>          |<span data-ttu-id="87008-116">String</span><span class="sxs-lookup"><span data-stu-id="87008-116">String</span></span>                     |<span data-ttu-id="87008-117">**Derzeit nicht unterstützt**.</span><span class="sxs-lookup"><span data-stu-id="87008-117">**Currently not supported**.</span></span> <span data-ttu-id="87008-118">Der Name der Eigenschaft in das Objekt verwiesen wird, der, das Wert für die als Referenz verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="87008-118">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87008-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="87008-119">JSON representation</span></span>

<span data-ttu-id="87008-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="87008-120">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
            
