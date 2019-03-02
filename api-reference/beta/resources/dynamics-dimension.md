---
title: Dimensions-Ressourcentyp
description: Eine Dimension in Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 92ba48a7ad55b6a7dff28ccc1547769c149e378b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365570"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="11f0b-103">Dimensions-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="11f0b-103">Dimensions resource type</span></span>
<span data-ttu-id="11f0b-104">Stellt eine Dimension in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="11f0b-104">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="11f0b-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="11f0b-105">Methods</span></span>
| <span data-ttu-id="11f0b-106">Methode</span><span class="sxs-lookup"><span data-stu-id="11f0b-106">Method</span></span>       | <span data-ttu-id="11f0b-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="11f0b-107">Return Type</span></span>  |<span data-ttu-id="11f0b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11f0b-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="11f0b-109">Dimensionen abrufen</span><span class="sxs-lookup"><span data-stu-id="11f0b-109">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="11f0b-110">dimension</span><span class="sxs-lookup"><span data-stu-id="11f0b-110">dimension</span></span>|<span data-ttu-id="11f0b-111">Ruft eine Dimension ab.</span><span class="sxs-lookup"><span data-stu-id="11f0b-111">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="11f0b-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="11f0b-112">Properties</span></span>
| <span data-ttu-id="11f0b-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11f0b-113">Property</span></span>           | <span data-ttu-id="11f0b-114">Typ</span><span class="sxs-lookup"><span data-stu-id="11f0b-114">Type</span></span>                  |<span data-ttu-id="11f0b-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11f0b-115">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="11f0b-116">id</span><span class="sxs-lookup"><span data-stu-id="11f0b-116">id</span></span>                  |<span data-ttu-id="11f0b-117">GUID</span><span class="sxs-lookup"><span data-stu-id="11f0b-117">GUID</span></span>                   |<span data-ttu-id="11f0b-118">Die eindeutige ID des Elements.</span><span class="sxs-lookup"><span data-stu-id="11f0b-118">The unique ID of the item.</span></span>|
|<span data-ttu-id="11f0b-119">code</span><span class="sxs-lookup"><span data-stu-id="11f0b-119">code</span></span>                |<span data-ttu-id="11f0b-120">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="11f0b-120">string, maximum size 20</span></span>|<span data-ttu-id="11f0b-121">Der Dimensionscode.</span><span class="sxs-lookup"><span data-stu-id="11f0b-121">The dimension code.</span></span>       |
|<span data-ttu-id="11f0b-122">displayName</span><span class="sxs-lookup"><span data-stu-id="11f0b-122">displayName</span></span>         |<span data-ttu-id="11f0b-123">string</span><span class="sxs-lookup"><span data-stu-id="11f0b-123">string</span></span>                 |<span data-ttu-id="11f0b-124">Gibt den Namen der Dimension an.</span><span class="sxs-lookup"><span data-stu-id="11f0b-124">Specifies the dimension's name.</span></span> <span data-ttu-id="11f0b-125">Dieser Name wird angezeigt, wo die Dimension verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="11f0b-125">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="11f0b-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11f0b-126">lastModifiedDateTime</span></span>|<span data-ttu-id="11f0b-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="11f0b-127">datetime</span></span>               |<span data-ttu-id="11f0b-128">Die letzte DateTime, die die Dimension geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="11f0b-128">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="11f0b-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="11f0b-129">JSON representation</span></span>

<span data-ttu-id="11f0b-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="11f0b-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

