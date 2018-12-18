---
title: Ressourcentyp educationOrganization
description: 'Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.  '
author: mmast-msft
ms.openlocfilehash: 54f281de29033418b6acb2f9821c5ebd1eaf4db0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349889"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="35a89-103">Ressourcentyp educationOrganization</span><span class="sxs-lookup"><span data-stu-id="35a89-103">educationOrganization resource type</span></span>

> <span data-ttu-id="35a89-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="35a89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35a89-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35a89-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35a89-106">Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.</span><span class="sxs-lookup"><span data-stu-id="35a89-106">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="35a89-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="35a89-107">Properties</span></span>
| <span data-ttu-id="35a89-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="35a89-108">Property</span></span>     | <span data-ttu-id="35a89-109">Typ</span><span class="sxs-lookup"><span data-stu-id="35a89-109">Type</span></span>   |<span data-ttu-id="35a89-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35a89-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35a89-111">description</span><span class="sxs-lookup"><span data-stu-id="35a89-111">description</span></span>|<span data-ttu-id="35a89-112">String</span><span class="sxs-lookup"><span data-stu-id="35a89-112">String</span></span>| <span data-ttu-id="35a89-113">Beschreibung der Organisation.</span><span class="sxs-lookup"><span data-stu-id="35a89-113">Organization description.</span></span>|
|<span data-ttu-id="35a89-114">displayName</span><span class="sxs-lookup"><span data-stu-id="35a89-114">displayName</span></span>|<span data-ttu-id="35a89-115">String</span><span class="sxs-lookup"><span data-stu-id="35a89-115">String</span></span>| <span data-ttu-id="35a89-116">Anzeigename der Organisation.</span><span class="sxs-lookup"><span data-stu-id="35a89-116">Organization display name.</span></span>|
|<span data-ttu-id="35a89-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="35a89-117">externalSource</span></span>|<span data-ttu-id="35a89-118">string</span><span class="sxs-lookup"><span data-stu-id="35a89-118">string</span></span>| <span data-ttu-id="35a89-119">Quelle, wo diese Organisation erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="35a89-119">Source where this organization was created from.</span></span> <span data-ttu-id="35a89-120">Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="35a89-120">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35a89-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="35a89-121">Relationships</span></span>
<span data-ttu-id="35a89-122">Keine.</span><span class="sxs-lookup"><span data-stu-id="35a89-122">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="35a89-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="35a89-123">JSON representation</span></span>

<span data-ttu-id="35a89-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="35a89-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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