---
title: deviceExchangeAccessStateSummary-Ressourcentyp
description: Exchange-Zugriffsstatus für Geräte – Zusammenfassung
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a01a1207801063285d7b59f0fa51c474ae78fb6d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418554"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="cb07f-103">deviceExchangeAccessStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cb07f-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="cb07f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cb07f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cb07f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cb07f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb07f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cb07f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb07f-107">Exchange-Zugriffsstatus für Geräte – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="cb07f-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="cb07f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cb07f-108">Properties</span></span>
|<span data-ttu-id="cb07f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb07f-109">Property</span></span>|<span data-ttu-id="cb07f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="cb07f-110">Type</span></span>|<span data-ttu-id="cb07f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb07f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb07f-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb07f-112">allowedDeviceCount</span></span>|<span data-ttu-id="cb07f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="cb07f-113">Int32</span></span>|<span data-ttu-id="cb07f-114">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Zulässig.</span><span class="sxs-lookup"><span data-stu-id="cb07f-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="cb07f-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb07f-115">blockedDeviceCount</span></span>|<span data-ttu-id="cb07f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="cb07f-116">Int32</span></span>|<span data-ttu-id="cb07f-117">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Blockiert.</span><span class="sxs-lookup"><span data-stu-id="cb07f-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="cb07f-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb07f-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="cb07f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="cb07f-119">Int32</span></span>|<span data-ttu-id="cb07f-120">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: In Quarantäne.</span><span class="sxs-lookup"><span data-stu-id="cb07f-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="cb07f-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb07f-121">unknownDeviceCount</span></span>|<span data-ttu-id="cb07f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="cb07f-122">Int32</span></span>|<span data-ttu-id="cb07f-123">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="cb07f-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="cb07f-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cb07f-124">unavailableDeviceCount</span></span>|<span data-ttu-id="cb07f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="cb07f-125">Int32</span></span>|<span data-ttu-id="cb07f-126">Gesamtanzahl von Geräten, für die kein Exchange-Zugriffsstatus gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="cb07f-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb07f-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cb07f-127">Relationships</span></span>
<span data-ttu-id="cb07f-128">Keine</span><span class="sxs-lookup"><span data-stu-id="cb07f-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb07f-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cb07f-129">JSON Representation</span></span>
<span data-ttu-id="cb07f-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cb07f-130">Here is a JSON representation of the resource.</span></span>
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




