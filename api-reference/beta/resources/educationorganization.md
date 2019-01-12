---
title: Ressourcentyp educationOrganization
description: 'Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a1e3f82e2d777b1d32cc445f543e7beed570a8b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949521"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="e9891-103">Ressourcentyp educationOrganization</span><span class="sxs-lookup"><span data-stu-id="e9891-103">educationOrganization resource type</span></span>

> <span data-ttu-id="e9891-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e9891-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9891-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e9891-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9891-106">Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.</span><span class="sxs-lookup"><span data-stu-id="e9891-106">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="e9891-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e9891-107">Properties</span></span>
| <span data-ttu-id="e9891-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9891-108">Property</span></span>     | <span data-ttu-id="e9891-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e9891-109">Type</span></span>   |<span data-ttu-id="e9891-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9891-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9891-111">description</span><span class="sxs-lookup"><span data-stu-id="e9891-111">description</span></span>|<span data-ttu-id="e9891-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e9891-112">String</span></span>| <span data-ttu-id="e9891-113">Beschreibung der Organisation.</span><span class="sxs-lookup"><span data-stu-id="e9891-113">Organization description.</span></span>|
|<span data-ttu-id="e9891-114">displayName</span><span class="sxs-lookup"><span data-stu-id="e9891-114">displayName</span></span>|<span data-ttu-id="e9891-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e9891-115">String</span></span>| <span data-ttu-id="e9891-116">Anzeigename der Organisation.</span><span class="sxs-lookup"><span data-stu-id="e9891-116">Organization display name.</span></span>|
|<span data-ttu-id="e9891-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="e9891-117">externalSource</span></span>|<span data-ttu-id="e9891-118">string</span><span class="sxs-lookup"><span data-stu-id="e9891-118">string</span></span>| <span data-ttu-id="e9891-119">Quelle, wo diese Organisation erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="e9891-119">Source where this organization was created from.</span></span> <span data-ttu-id="e9891-120">Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e9891-120">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9891-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e9891-121">Relationships</span></span>
<span data-ttu-id="e9891-122">Keine.</span><span class="sxs-lookup"><span data-stu-id="e9891-122">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e9891-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e9891-123">JSON representation</span></span>

<span data-ttu-id="e9891-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e9891-124">The following is a JSON representation of the resource.</span></span>

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
