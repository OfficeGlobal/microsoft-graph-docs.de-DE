---
title: deviceExchangeAccessStateSummary-Ressourcentyp
description: Exchange-Zugriffsstatus für Geräte – Zusammenfassung
author: tfitzmac
ms.openlocfilehash: dd2784078e8b44b1a02cb5a0013c1e38804912c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301743"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="880bd-103">deviceExchangeAccessStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="880bd-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="880bd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="880bd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="880bd-105">Exchange-Zugriffsstatus für Geräte – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="880bd-105">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="880bd-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="880bd-106">Properties</span></span>
|<span data-ttu-id="880bd-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="880bd-107">Property</span></span>|<span data-ttu-id="880bd-108">Typ</span><span class="sxs-lookup"><span data-stu-id="880bd-108">Type</span></span>|<span data-ttu-id="880bd-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="880bd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="880bd-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="880bd-110">allowedDeviceCount</span></span>|<span data-ttu-id="880bd-111">Int32</span><span class="sxs-lookup"><span data-stu-id="880bd-111">Int32</span></span>|<span data-ttu-id="880bd-112">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Zulässig.</span><span class="sxs-lookup"><span data-stu-id="880bd-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="880bd-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="880bd-113">blockedDeviceCount</span></span>|<span data-ttu-id="880bd-114">Int32</span><span class="sxs-lookup"><span data-stu-id="880bd-114">Int32</span></span>|<span data-ttu-id="880bd-115">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Blockiert.</span><span class="sxs-lookup"><span data-stu-id="880bd-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="880bd-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="880bd-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="880bd-117">Int32</span><span class="sxs-lookup"><span data-stu-id="880bd-117">Int32</span></span>|<span data-ttu-id="880bd-118">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: In Quarantäne.</span><span class="sxs-lookup"><span data-stu-id="880bd-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="880bd-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="880bd-119">unknownDeviceCount</span></span>|<span data-ttu-id="880bd-120">Int32</span><span class="sxs-lookup"><span data-stu-id="880bd-120">Int32</span></span>|<span data-ttu-id="880bd-121">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="880bd-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="880bd-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="880bd-122">unavailableDeviceCount</span></span>|<span data-ttu-id="880bd-123">Int32</span><span class="sxs-lookup"><span data-stu-id="880bd-123">Int32</span></span>|<span data-ttu-id="880bd-124">Gesamtanzahl von Geräten, für die kein Exchange-Zugriffsstatus gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="880bd-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="880bd-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="880bd-125">Relationships</span></span>
<span data-ttu-id="880bd-126">Keine</span><span class="sxs-lookup"><span data-stu-id="880bd-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="880bd-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="880bd-127">JSON Representation</span></span>
<span data-ttu-id="880bd-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="880bd-128">Here is a JSON representation of the resource.</span></span>
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



