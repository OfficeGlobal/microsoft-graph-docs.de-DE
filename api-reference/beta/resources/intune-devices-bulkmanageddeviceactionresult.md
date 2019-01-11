---
title: Ressourcentyp bulkManagedDeviceActionResult
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c7aa0d49182908a960130e202fd4cf096c2c16c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872247"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="fddd7-103">Ressourcentyp bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="fddd7-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="fddd7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fddd7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fddd7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fddd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fddd7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fddd7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fddd7-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fddd7-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="fddd7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fddd7-108">Properties</span></span>
|<span data-ttu-id="fddd7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fddd7-109">Property</span></span>|<span data-ttu-id="fddd7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fddd7-110">Type</span></span>|<span data-ttu-id="fddd7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fddd7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fddd7-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="fddd7-112">successfulDeviceIds</span></span>|<span data-ttu-id="fddd7-113">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="fddd7-113">String collection</span></span>|<span data-ttu-id="fddd7-114">Erfolgreiche Geräte</span><span class="sxs-lookup"><span data-stu-id="fddd7-114">Successful devices</span></span>|
|<span data-ttu-id="fddd7-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="fddd7-115">failedDeviceIds</span></span>|<span data-ttu-id="fddd7-116">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="fddd7-116">String collection</span></span>|<span data-ttu-id="fddd7-117">Fehlerhafte Geräte</span><span class="sxs-lookup"><span data-stu-id="fddd7-117">Failed devices</span></span>|
|<span data-ttu-id="fddd7-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="fddd7-118">notFoundDeviceIds</span></span>|<span data-ttu-id="fddd7-119">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="fddd7-119">String collection</span></span>|<span data-ttu-id="fddd7-120">Geräte nicht gefunden</span><span class="sxs-lookup"><span data-stu-id="fddd7-120">Not found devices</span></span>|
|<span data-ttu-id="fddd7-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="fddd7-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="fddd7-122">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="fddd7-122">String collection</span></span>|<span data-ttu-id="fddd7-123">Nicht unterstützte Geräte</span><span class="sxs-lookup"><span data-stu-id="fddd7-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="fddd7-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fddd7-124">Relationships</span></span>
<span data-ttu-id="fddd7-125">Keine</span><span class="sxs-lookup"><span data-stu-id="fddd7-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fddd7-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fddd7-126">JSON Representation</span></span>
<span data-ttu-id="fddd7-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fddd7-127">Here is a JSON representation of the resource.</span></span>
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





