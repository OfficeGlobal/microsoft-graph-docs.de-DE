---
title: Ressourcentyp modifiedProperty
description: Gibt an, die geänderten Eigenschaften mit vorherigen und neuen Wert für eine Ressource in Azure AD, die geändert wird.
ms.openlocfilehash: c504969ee12798969aa39490e79cb5b60bdb5435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060769"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="333c8-103">Ressourcentyp modifiedProperty</span><span class="sxs-lookup"><span data-stu-id="333c8-103">modifiedProperty resource type</span></span>
<span data-ttu-id="333c8-104">Gibt an, die geänderten Eigenschaften mit vorherigen und neuen Wert für eine Ressource in Azure AD, die geändert wird.</span><span class="sxs-lookup"><span data-stu-id="333c8-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="333c8-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="333c8-105">Properties</span></span>
| <span data-ttu-id="333c8-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="333c8-106">Property</span></span>     | <span data-ttu-id="333c8-107">Typ</span><span class="sxs-lookup"><span data-stu-id="333c8-107">Type</span></span>   |<span data-ttu-id="333c8-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="333c8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="333c8-109">displayName</span><span class="sxs-lookup"><span data-stu-id="333c8-109">displayName</span></span>|<span data-ttu-id="333c8-110">String</span><span class="sxs-lookup"><span data-stu-id="333c8-110">String</span></span>|<span data-ttu-id="333c8-111">Gibt den Eigenschaftennamen des Zielattributs, die geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="333c8-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="333c8-112">newValue</span><span class="sxs-lookup"><span data-stu-id="333c8-112">newValue</span></span>|<span data-ttu-id="333c8-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="333c8-113">String</span></span>|<span data-ttu-id="333c8-114">Gibt den aktualisierten Wert für die Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="333c8-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="333c8-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="333c8-115">oldValue</span></span>|<span data-ttu-id="333c8-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="333c8-116">String</span></span>|<span data-ttu-id="333c8-117">Gibt den vorherigen Wert (vor der Aktualisierung) für die Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="333c8-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="333c8-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="333c8-118">JSON representation</span></span>

<span data-ttu-id="333c8-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="333c8-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->