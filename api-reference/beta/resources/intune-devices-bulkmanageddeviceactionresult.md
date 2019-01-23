---
title: Ressourcentyp bulkManagedDeviceActionResult
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d1b23efdb5b8eed16c6c66d72a13efaef9e38d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425841"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="b615e-103">Ressourcentyp bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="b615e-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="b615e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b615e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b615e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b615e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b615e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b615e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b615e-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b615e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b615e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b615e-108">Properties</span></span>
|<span data-ttu-id="b615e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b615e-109">Property</span></span>|<span data-ttu-id="b615e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b615e-110">Type</span></span>|<span data-ttu-id="b615e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b615e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b615e-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="b615e-112">successfulDeviceIds</span></span>|<span data-ttu-id="b615e-113">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b615e-113">String collection</span></span>|<span data-ttu-id="b615e-114">Erfolgreiche Geräte</span><span class="sxs-lookup"><span data-stu-id="b615e-114">Successful devices</span></span>|
|<span data-ttu-id="b615e-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="b615e-115">failedDeviceIds</span></span>|<span data-ttu-id="b615e-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b615e-116">String collection</span></span>|<span data-ttu-id="b615e-117">Fehlerhafte Geräte</span><span class="sxs-lookup"><span data-stu-id="b615e-117">Failed devices</span></span>|
|<span data-ttu-id="b615e-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="b615e-118">notFoundDeviceIds</span></span>|<span data-ttu-id="b615e-119">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b615e-119">String collection</span></span>|<span data-ttu-id="b615e-120">Geräte nicht gefunden</span><span class="sxs-lookup"><span data-stu-id="b615e-120">Not found devices</span></span>|
|<span data-ttu-id="b615e-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="b615e-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="b615e-122">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b615e-122">String collection</span></span>|<span data-ttu-id="b615e-123">Nicht unterstützte Geräte</span><span class="sxs-lookup"><span data-stu-id="b615e-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="b615e-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b615e-124">Relationships</span></span>
<span data-ttu-id="b615e-125">Keine</span><span class="sxs-lookup"><span data-stu-id="b615e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b615e-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b615e-126">JSON Representation</span></span>
<span data-ttu-id="b615e-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b615e-127">Here is a JSON representation of the resource.</span></span>
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




