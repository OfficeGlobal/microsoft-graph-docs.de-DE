---
title: deviceExchangeAccessStateSummary-Ressourcentyp
description: Exchange-Zugriffsstatus für Geräte – Zusammenfassung
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 49afbb3383035711bc950a9a7226a354ae78f0e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920429"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="88ba8-103">deviceExchangeAccessStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="88ba8-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="88ba8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="88ba8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88ba8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88ba8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88ba8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="88ba8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88ba8-107">Exchange-Zugriffsstatus für Geräte – Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="88ba8-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="88ba8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88ba8-108">Properties</span></span>
|<span data-ttu-id="88ba8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88ba8-109">Property</span></span>|<span data-ttu-id="88ba8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="88ba8-110">Type</span></span>|<span data-ttu-id="88ba8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88ba8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ba8-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ba8-112">allowedDeviceCount</span></span>|<span data-ttu-id="88ba8-113">Int32</span><span class="sxs-lookup"><span data-stu-id="88ba8-113">Int32</span></span>|<span data-ttu-id="88ba8-114">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Zulässig.</span><span class="sxs-lookup"><span data-stu-id="88ba8-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="88ba8-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ba8-115">blockedDeviceCount</span></span>|<span data-ttu-id="88ba8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="88ba8-116">Int32</span></span>|<span data-ttu-id="88ba8-117">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Blockiert.</span><span class="sxs-lookup"><span data-stu-id="88ba8-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="88ba8-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ba8-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="88ba8-119">Int32</span><span class="sxs-lookup"><span data-stu-id="88ba8-119">Int32</span></span>|<span data-ttu-id="88ba8-120">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: In Quarantäne.</span><span class="sxs-lookup"><span data-stu-id="88ba8-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="88ba8-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ba8-121">unknownDeviceCount</span></span>|<span data-ttu-id="88ba8-122">Int32</span><span class="sxs-lookup"><span data-stu-id="88ba8-122">Int32</span></span>|<span data-ttu-id="88ba8-123">Gesamtanzahl von Geräten mit Exchange-Zugriffsstatus: Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="88ba8-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="88ba8-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="88ba8-124">unavailableDeviceCount</span></span>|<span data-ttu-id="88ba8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="88ba8-125">Int32</span></span>|<span data-ttu-id="88ba8-126">Gesamtanzahl von Geräten, für die kein Exchange-Zugriffsstatus gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="88ba8-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88ba8-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="88ba8-127">Relationships</span></span>
<span data-ttu-id="88ba8-128">Keine</span><span class="sxs-lookup"><span data-stu-id="88ba8-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="88ba8-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88ba8-129">JSON Representation</span></span>
<span data-ttu-id="88ba8-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88ba8-130">Here is a JSON representation of the resource.</span></span>
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





