---
title: deviceExchangeAccessStateSummary-Ressourcentyp
description: Exchange-Zugriffsstatus für Geräte – Zusammenfassung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c336ee6d4b23983f01a4c4756325960c709194f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260515"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="e1b99-103">deviceExchangeAccessStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e1b99-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="e1b99-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e1b99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1b99-105">Exchange-Zugriffsstatus für Geräte – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="e1b99-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="e1b99-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e1b99-106">Properties</span></span>
|<span data-ttu-id="e1b99-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1b99-107">Property</span></span>|<span data-ttu-id="e1b99-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e1b99-108">Type</span></span>|<span data-ttu-id="e1b99-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1b99-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b99-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1b99-110">allowedDeviceCount</span></span>|<span data-ttu-id="e1b99-111">Int32</span><span class="sxs-lookup"><span data-stu-id="e1b99-111">Int32</span></span>|<span data-ttu-id="e1b99-112">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Zulässig.</span><span class="sxs-lookup"><span data-stu-id="e1b99-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="e1b99-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1b99-113">blockedDeviceCount</span></span>|<span data-ttu-id="e1b99-114">Int32</span><span class="sxs-lookup"><span data-stu-id="e1b99-114">Int32</span></span>|<span data-ttu-id="e1b99-115">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Blockiert.</span><span class="sxs-lookup"><span data-stu-id="e1b99-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="e1b99-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1b99-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="e1b99-117">Int32</span><span class="sxs-lookup"><span data-stu-id="e1b99-117">Int32</span></span>|<span data-ttu-id="e1b99-118">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: In Quarantäne.</span><span class="sxs-lookup"><span data-stu-id="e1b99-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="e1b99-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1b99-119">unknownDeviceCount</span></span>|<span data-ttu-id="e1b99-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e1b99-120">Int32</span></span>|<span data-ttu-id="e1b99-121">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="e1b99-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="e1b99-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e1b99-122">unavailableDeviceCount</span></span>|<span data-ttu-id="e1b99-123">Int32</span><span class="sxs-lookup"><span data-stu-id="e1b99-123">Int32</span></span>|<span data-ttu-id="e1b99-124">Gesamtanzahl von Geräten, für die kein Exchange-Zugriffsstatus gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="e1b99-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1b99-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e1b99-125">Relationships</span></span>
<span data-ttu-id="e1b99-126">Keine</span><span class="sxs-lookup"><span data-stu-id="e1b99-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1b99-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e1b99-127">JSON Representation</span></span>
<span data-ttu-id="e1b99-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e1b99-128">Here is a JSON representation of the resource.</span></span>
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



