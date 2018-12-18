---
title: Ressourcentyp resourceReference
description: Komplexer Typ mit Eigenschaften des Insights.
author: simonhult
ms.openlocfilehash: 2f1a44412eebbb7a74895c12db9a07696d6ee409
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363620"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="d3bd7-103">Ressourcentyp resourceReference</span><span class="sxs-lookup"><span data-stu-id="d3bd7-103">resourceReference resource type</span></span>

> <span data-ttu-id="d3bd7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d3bd7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3bd7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d3bd7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3bd7-106">Komplexer Typ mit Eigenschaften des [Insights](insights.md).</span><span class="sxs-lookup"><span data-stu-id="d3bd7-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3bd7-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d3bd7-107">JSON representation</span></span>

<span data-ttu-id="d3bd7-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d3bd7-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="d3bd7-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d3bd7-109">Properties</span></span>

| <span data-ttu-id="d3bd7-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3bd7-110">Property</span></span>      | <span data-ttu-id="d3bd7-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d3bd7-111">Type</span></span>      | <span data-ttu-id="d3bd7-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3bd7-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="d3bd7-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="d3bd7-113">webUrl</span></span>        | <span data-ttu-id="d3bd7-114">String</span><span class="sxs-lookup"><span data-stu-id="d3bd7-114">String</span></span>    | <span data-ttu-id="d3bd7-115">Eine URL, die auf das verwiesene Element führende.</span><span class="sxs-lookup"><span data-stu-id="d3bd7-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="d3bd7-116">id</span><span class="sxs-lookup"><span data-stu-id="d3bd7-116">id</span></span>            | <span data-ttu-id="d3bd7-117">String</span><span class="sxs-lookup"><span data-stu-id="d3bd7-117">String</span></span>    | <span data-ttu-id="d3bd7-118">Eindeutiger Bezeichner des Elements.</span><span class="sxs-lookup"><span data-stu-id="d3bd7-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="d3bd7-119">type</span><span class="sxs-lookup"><span data-stu-id="d3bd7-119">type</span></span>          | <span data-ttu-id="d3bd7-120">String</span><span class="sxs-lookup"><span data-stu-id="d3bd7-120">String</span></span>    | <span data-ttu-id="d3bd7-121">Ein String-Wert, der verwendet werden kann, um das Element, wie beispielsweise "microsoft.graph.driveItem" klassifizieren</span><span class="sxs-lookup"><span data-stu-id="d3bd7-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |