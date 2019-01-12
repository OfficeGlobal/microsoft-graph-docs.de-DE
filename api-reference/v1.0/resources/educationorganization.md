---
title: Ressourcentyp educationOrganization
description: Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99f3294f76a246e4e78f0f61b0fc1f62532c3a03
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977423"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="38a15-103">Ressourcentyp educationOrganization</span><span class="sxs-lookup"><span data-stu-id="38a15-103">educationOrganization resource type</span></span>

<span data-ttu-id="38a15-104">Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.</span><span class="sxs-lookup"><span data-stu-id="38a15-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="38a15-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="38a15-105">Properties</span></span>
| <span data-ttu-id="38a15-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38a15-106">Property</span></span>     | <span data-ttu-id="38a15-107">Typ</span><span class="sxs-lookup"><span data-stu-id="38a15-107">Type</span></span>   |<span data-ttu-id="38a15-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38a15-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38a15-109">description</span><span class="sxs-lookup"><span data-stu-id="38a15-109">description</span></span>|<span data-ttu-id="38a15-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38a15-110">String</span></span>| <span data-ttu-id="38a15-111">Beschreibung der Organisation.</span><span class="sxs-lookup"><span data-stu-id="38a15-111">Organization description.</span></span>|
|<span data-ttu-id="38a15-112">displayName</span><span class="sxs-lookup"><span data-stu-id="38a15-112">displayName</span></span>|<span data-ttu-id="38a15-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="38a15-113">String</span></span>| <span data-ttu-id="38a15-114">Anzeigename der Organisation.</span><span class="sxs-lookup"><span data-stu-id="38a15-114">Organization display name.</span></span>|
|<span data-ttu-id="38a15-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="38a15-115">externalSource</span></span>|<span data-ttu-id="38a15-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="38a15-116">educationExternalSource</span></span>| <span data-ttu-id="38a15-117">Quelle, wo diese Organisation erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="38a15-117">Source where this organization was created from.</span></span> <span data-ttu-id="38a15-118">Die möglichen Werte sind: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="38a15-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38a15-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="38a15-119">Relationships</span></span>
<span data-ttu-id="38a15-120">Keine.</span><span class="sxs-lookup"><span data-stu-id="38a15-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="38a15-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="38a15-121">JSON representation</span></span>

<span data-ttu-id="38a15-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="38a15-122">The following is a JSON representation of the resource.</span></span>

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
