---
title: Ressourcentyp educationOrganization
description: Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: b0b65978b3b415af407c886095c4b31c7aaffab9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831934"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="3c8a4-103">Ressourcentyp educationOrganization</span><span class="sxs-lookup"><span data-stu-id="3c8a4-103">educationOrganization resource type</span></span>

<span data-ttu-id="3c8a4-104">Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.</span><span class="sxs-lookup"><span data-stu-id="3c8a4-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="3c8a4-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c8a4-105">Properties</span></span>
| <span data-ttu-id="3c8a4-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c8a4-106">Property</span></span>     | <span data-ttu-id="3c8a4-107">Typ</span><span class="sxs-lookup"><span data-stu-id="3c8a4-107">Type</span></span>   |<span data-ttu-id="3c8a4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c8a4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c8a4-109">description</span><span class="sxs-lookup"><span data-stu-id="3c8a4-109">description</span></span>|<span data-ttu-id="3c8a4-110">String</span><span class="sxs-lookup"><span data-stu-id="3c8a4-110">String</span></span>| <span data-ttu-id="3c8a4-111">Beschreibung der Organisation.</span><span class="sxs-lookup"><span data-stu-id="3c8a4-111">Organization description.</span></span>|
|<span data-ttu-id="3c8a4-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3c8a4-112">displayName</span></span>|<span data-ttu-id="3c8a4-113">String</span><span class="sxs-lookup"><span data-stu-id="3c8a4-113">String</span></span>| <span data-ttu-id="3c8a4-114">Anzeigename der Organisation.</span><span class="sxs-lookup"><span data-stu-id="3c8a4-114">Organization display name.</span></span>|
|<span data-ttu-id="3c8a4-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="3c8a4-115">externalSource</span></span>|<span data-ttu-id="3c8a4-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="3c8a4-116">educationExternalSource</span></span>| <span data-ttu-id="3c8a4-117">Quelle, wo diese Organisation erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3c8a4-117">Source where this organization was created from.</span></span> <span data-ttu-id="3c8a4-118">Die möglichen Werte sind: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3c8a4-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c8a4-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3c8a4-119">Relationships</span></span>
<span data-ttu-id="3c8a4-120">Keine.</span><span class="sxs-lookup"><span data-stu-id="3c8a4-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3c8a4-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c8a4-121">JSON representation</span></span>

<span data-ttu-id="3c8a4-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c8a4-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
