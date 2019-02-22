---
title: bulkManagedDeviceActionResult-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 199fe08b4eaf339f17fdb67bb6dbcc0243fd90f9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168334"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="0ff5e-103">bulkManagedDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0ff5e-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="0ff5e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ff5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ff5e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0ff5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ff5e-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0ff5e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0ff5e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0ff5e-107">Properties</span></span>
|<span data-ttu-id="0ff5e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0ff5e-108">Property</span></span>|<span data-ttu-id="0ff5e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0ff5e-109">Type</span></span>|<span data-ttu-id="0ff5e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ff5e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ff5e-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="0ff5e-111">successfulDeviceIds</span></span>|<span data-ttu-id="0ff5e-112">String collection</span><span class="sxs-lookup"><span data-stu-id="0ff5e-112">String collection</span></span>|<span data-ttu-id="0ff5e-113">Erfolgreiche Geräte</span><span class="sxs-lookup"><span data-stu-id="0ff5e-113">Successful devices</span></span>|
|<span data-ttu-id="0ff5e-114">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="0ff5e-114">failedDeviceIds</span></span>|<span data-ttu-id="0ff5e-115">String collection</span><span class="sxs-lookup"><span data-stu-id="0ff5e-115">String collection</span></span>|<span data-ttu-id="0ff5e-116">FehlgeSchlagene Geräte</span><span class="sxs-lookup"><span data-stu-id="0ff5e-116">Failed devices</span></span>|
|<span data-ttu-id="0ff5e-117">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="0ff5e-117">notFoundDeviceIds</span></span>|<span data-ttu-id="0ff5e-118">String collection</span><span class="sxs-lookup"><span data-stu-id="0ff5e-118">String collection</span></span>|<span data-ttu-id="0ff5e-119">Nicht gefundene Geräte</span><span class="sxs-lookup"><span data-stu-id="0ff5e-119">Not found devices</span></span>|
|<span data-ttu-id="0ff5e-120">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="0ff5e-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="0ff5e-121">String collection</span><span class="sxs-lookup"><span data-stu-id="0ff5e-121">String collection</span></span>|<span data-ttu-id="0ff5e-122">Nicht unterstützte Geräte</span><span class="sxs-lookup"><span data-stu-id="0ff5e-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ff5e-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0ff5e-123">Relationships</span></span>
<span data-ttu-id="0ff5e-124">Keine</span><span class="sxs-lookup"><span data-stu-id="0ff5e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ff5e-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0ff5e-125">JSON Representation</span></span>
<span data-ttu-id="0ff5e-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0ff5e-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "successfulDeviceIds": [
    "String"
  ],
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ]
}
```




