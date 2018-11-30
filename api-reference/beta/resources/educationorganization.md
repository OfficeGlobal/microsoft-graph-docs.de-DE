---
title: Ressourcentyp educationOrganization
description: 'Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.  '
ms.openlocfilehash: 86da4e19f9cc36de7a61ca2c76565a17ec3acac0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061005"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="ff032-103">Ressourcentyp educationOrganization</span><span class="sxs-lookup"><span data-stu-id="ff032-103">educationOrganization resource type</span></span>

> <span data-ttu-id="ff032-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff032-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff032-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff032-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff032-106">Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.</span><span class="sxs-lookup"><span data-stu-id="ff032-106">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="ff032-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ff032-107">Properties</span></span>
| <span data-ttu-id="ff032-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff032-108">Property</span></span>     | <span data-ttu-id="ff032-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ff032-109">Type</span></span>   |<span data-ttu-id="ff032-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff032-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff032-111">description</span><span class="sxs-lookup"><span data-stu-id="ff032-111">description</span></span>|<span data-ttu-id="ff032-112">String</span><span class="sxs-lookup"><span data-stu-id="ff032-112">String</span></span>| <span data-ttu-id="ff032-113">Beschreibung der Organisation.</span><span class="sxs-lookup"><span data-stu-id="ff032-113">Organization description.</span></span>|
|<span data-ttu-id="ff032-114">displayName</span><span class="sxs-lookup"><span data-stu-id="ff032-114">displayName</span></span>|<span data-ttu-id="ff032-115">String</span><span class="sxs-lookup"><span data-stu-id="ff032-115">String</span></span>| <span data-ttu-id="ff032-116">Anzeigename der Organisation.</span><span class="sxs-lookup"><span data-stu-id="ff032-116">Organization display name.</span></span>|
|<span data-ttu-id="ff032-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="ff032-117">externalSource</span></span>|<span data-ttu-id="ff032-118">string</span><span class="sxs-lookup"><span data-stu-id="ff032-118">string</span></span>| <span data-ttu-id="ff032-119">Quelle, wo diese Organisation erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="ff032-119">Source where this organization was created from.</span></span> <span data-ttu-id="ff032-120">Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ff032-120">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff032-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ff032-121">Relationships</span></span>
<span data-ttu-id="ff032-122">Keine.</span><span class="sxs-lookup"><span data-stu-id="ff032-122">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ff032-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ff032-123">JSON representation</span></span>

<span data-ttu-id="ff032-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ff032-124">The following is a JSON representation of the resource.</span></span>

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