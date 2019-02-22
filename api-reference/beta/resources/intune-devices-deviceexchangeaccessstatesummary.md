---
title: deviceExchangeAccessStateSummary-Ressourcentyp
description: Exchange-Zugriffsstatus für Geräte – Zusammenfassung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ad327dc26bc9268a5f248206893e3a11e6fb27c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154131"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="e6a5b-103">deviceExchangeAccessStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e6a5b-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="e6a5b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6a5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6a5b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e6a5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6a5b-106">Exchange-Zugriffsstatus für Geräte – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="e6a5b-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="e6a5b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e6a5b-107">Properties</span></span>
|<span data-ttu-id="e6a5b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e6a5b-108">Property</span></span>|<span data-ttu-id="e6a5b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e6a5b-109">Type</span></span>|<span data-ttu-id="e6a5b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6a5b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6a5b-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a5b-111">allowedDeviceCount</span></span>|<span data-ttu-id="e6a5b-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a5b-112">Int32</span></span>|<span data-ttu-id="e6a5b-113">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Zulässig.</span><span class="sxs-lookup"><span data-stu-id="e6a5b-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="e6a5b-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a5b-114">blockedDeviceCount</span></span>|<span data-ttu-id="e6a5b-115">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a5b-115">Int32</span></span>|<span data-ttu-id="e6a5b-116">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Blockiert.</span><span class="sxs-lookup"><span data-stu-id="e6a5b-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="e6a5b-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a5b-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="e6a5b-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a5b-118">Int32</span></span>|<span data-ttu-id="e6a5b-119">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: In Quarantäne.</span><span class="sxs-lookup"><span data-stu-id="e6a5b-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="e6a5b-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a5b-120">unknownDeviceCount</span></span>|<span data-ttu-id="e6a5b-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a5b-121">Int32</span></span>|<span data-ttu-id="e6a5b-122">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="e6a5b-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="e6a5b-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a5b-123">unavailableDeviceCount</span></span>|<span data-ttu-id="e6a5b-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a5b-124">Int32</span></span>|<span data-ttu-id="e6a5b-125">Gesamtanzahl von Geräten, für die kein Exchange-Zugriffsstatus gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="e6a5b-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6a5b-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e6a5b-126">Relationships</span></span>
<span data-ttu-id="e6a5b-127">Keine</span><span class="sxs-lookup"><span data-stu-id="e6a5b-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6a5b-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e6a5b-128">JSON Representation</span></span>
<span data-ttu-id="e6a5b-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e6a5b-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```




