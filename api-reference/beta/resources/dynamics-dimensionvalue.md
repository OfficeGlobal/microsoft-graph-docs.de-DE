---
title: dimensionValues-Ressourcentyp
description: Ein Dimensionswert in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: da3935b8e784b05551af123c1832d5dc84a2c81c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365318"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="89f56-103">dimensionValues-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="89f56-103">dimensionValues resource type</span></span>
<span data-ttu-id="89f56-104">Stellt einen Dimensionswert in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="89f56-104">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="89f56-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="89f56-105">Methods</span></span>

| <span data-ttu-id="89f56-106">Methode</span><span class="sxs-lookup"><span data-stu-id="89f56-106">Method</span></span>       | <span data-ttu-id="89f56-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="89f56-107">Return Type</span></span>  |<span data-ttu-id="89f56-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89f56-108">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="89f56-109">DimensionValues abrufen</span><span class="sxs-lookup"><span data-stu-id="89f56-109">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="89f56-110">dimensionValues</span><span class="sxs-lookup"><span data-stu-id="89f56-110">dimensionValues</span></span>|<span data-ttu-id="89f56-111">Ruft ein Dimensionswert Objekt ab.</span><span class="sxs-lookup"><span data-stu-id="89f56-111">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="89f56-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="89f56-112">Properties</span></span>
| <span data-ttu-id="89f56-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="89f56-113">Property</span></span>           | <span data-ttu-id="89f56-114">Typ</span><span class="sxs-lookup"><span data-stu-id="89f56-114">Type</span></span>                  |<span data-ttu-id="89f56-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89f56-115">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="89f56-116">id</span><span class="sxs-lookup"><span data-stu-id="89f56-116">id</span></span>                  |<span data-ttu-id="89f56-117">GUID</span><span class="sxs-lookup"><span data-stu-id="89f56-117">GUID</span></span>                   |<span data-ttu-id="89f56-118">Die eindeutige ID des Elements.</span><span class="sxs-lookup"><span data-stu-id="89f56-118">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="89f56-119">code</span><span class="sxs-lookup"><span data-stu-id="89f56-119">code</span></span>                |<span data-ttu-id="89f56-120">Zeichenfolge, maximale Größe 20</span><span class="sxs-lookup"><span data-stu-id="89f56-120">string, maximum size 20</span></span>|<span data-ttu-id="89f56-121">Der Dimensionswertcode.</span><span class="sxs-lookup"><span data-stu-id="89f56-121">The dimension value code.</span></span>                          |
|<span data-ttu-id="89f56-122">displayName</span><span class="sxs-lookup"><span data-stu-id="89f56-122">displayName</span></span>         |<span data-ttu-id="89f56-123">string</span><span class="sxs-lookup"><span data-stu-id="89f56-123">string</span></span>                 |<span data-ttu-id="89f56-124">Gibt den Namen des Dimensionswerts an.</span><span class="sxs-lookup"><span data-stu-id="89f56-124">Specifies the dimension value's name.</span></span> <span data-ttu-id="89f56-125">Dieser Name wird angezeigt, wenn der Dimensionswert verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="89f56-125">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="89f56-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89f56-126">lastModifiedDateTime</span></span>|<span data-ttu-id="89f56-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="89f56-127">datetime</span></span>               |<span data-ttu-id="89f56-128">Die letzte DateTime, für die der Dimensionswert geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="89f56-128">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="89f56-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="89f56-129">JSON representation</span></span>

<span data-ttu-id="89f56-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="89f56-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


