---
title: deviceExchangeAccessStateSummary-Ressourcentyp
description: Exchange-Zugriffsstatus für Geräte – Zusammenfassung
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b8ca08b026b8e1cdbac4bd0dc73331a9d5df80fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889985"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="21a7f-103">deviceExchangeAccessStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="21a7f-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="21a7f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="21a7f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21a7f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21a7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21a7f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="21a7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21a7f-107">Exchange-Zugriffsstatus für Geräte – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="21a7f-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="21a7f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="21a7f-108">Properties</span></span>
|<span data-ttu-id="21a7f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21a7f-109">Property</span></span>|<span data-ttu-id="21a7f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="21a7f-110">Type</span></span>|<span data-ttu-id="21a7f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21a7f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21a7f-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21a7f-112">allowedDeviceCount</span></span>|<span data-ttu-id="21a7f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="21a7f-113">Int32</span></span>|<span data-ttu-id="21a7f-114">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Zulässig.</span><span class="sxs-lookup"><span data-stu-id="21a7f-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="21a7f-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21a7f-115">blockedDeviceCount</span></span>|<span data-ttu-id="21a7f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="21a7f-116">Int32</span></span>|<span data-ttu-id="21a7f-117">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Blockiert.</span><span class="sxs-lookup"><span data-stu-id="21a7f-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="21a7f-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21a7f-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="21a7f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="21a7f-119">Int32</span></span>|<span data-ttu-id="21a7f-120">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: In Quarantäne.</span><span class="sxs-lookup"><span data-stu-id="21a7f-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="21a7f-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21a7f-121">unknownDeviceCount</span></span>|<span data-ttu-id="21a7f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="21a7f-122">Int32</span></span>|<span data-ttu-id="21a7f-123">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="21a7f-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="21a7f-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21a7f-124">unavailableDeviceCount</span></span>|<span data-ttu-id="21a7f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="21a7f-125">Int32</span></span>|<span data-ttu-id="21a7f-126">Gesamtanzahl von Geräten, für die kein Exchange-Zugriffsstatus gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="21a7f-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21a7f-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="21a7f-127">Relationships</span></span>
<span data-ttu-id="21a7f-128">Keine</span><span class="sxs-lookup"><span data-stu-id="21a7f-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21a7f-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="21a7f-129">JSON Representation</span></span>
<span data-ttu-id="21a7f-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="21a7f-130">Here is a JSON representation of the resource.</span></span>
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





