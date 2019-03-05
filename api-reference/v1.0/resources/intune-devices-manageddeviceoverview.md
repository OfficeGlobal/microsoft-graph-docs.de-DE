---
title: managedDeviceOverview-Ressourcentyp
description: Zusammenfassungsdaten für verwaltete Geräte
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: accc6d976db80421cd06fd8071417bf07684a71a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250614"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="42887-103">managedDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="42887-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="42887-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="42887-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42887-105">Zusammenfassungsdaten für verwaltete Geräte</span><span class="sxs-lookup"><span data-stu-id="42887-105">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="42887-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="42887-106">Methods</span></span>
|<span data-ttu-id="42887-107">Methode</span><span class="sxs-lookup"><span data-stu-id="42887-107">Method</span></span>|<span data-ttu-id="42887-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="42887-108">Return Type</span></span>|<span data-ttu-id="42887-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42887-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42887-110">managedDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="42887-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="42887-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="42887-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="42887-112">Lesen von Eigenschaften und Beziehungen des [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="42887-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="42887-113">managedDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="42887-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="42887-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="42887-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="42887-115">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="42887-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="42887-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="42887-116">Properties</span></span>
|<span data-ttu-id="42887-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="42887-117">Property</span></span>|<span data-ttu-id="42887-118">Typ</span><span class="sxs-lookup"><span data-stu-id="42887-118">Type</span></span>|<span data-ttu-id="42887-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42887-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42887-120">id</span><span class="sxs-lookup"><span data-stu-id="42887-120">id</span></span>|<span data-ttu-id="42887-121">String</span><span class="sxs-lookup"><span data-stu-id="42887-121">String</span></span>|<span data-ttu-id="42887-122">Eindeutiger Bezeichner für die Zusammenfassung</span><span class="sxs-lookup"><span data-stu-id="42887-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="42887-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="42887-123">enrolledDeviceCount</span></span>|<span data-ttu-id="42887-124">Int32</span><span class="sxs-lookup"><span data-stu-id="42887-124">Int32</span></span>|<span data-ttu-id="42887-125">Gesamtanzahl von registrierten Geräten.</span><span class="sxs-lookup"><span data-stu-id="42887-125">Total enrolled device count.</span></span> <span data-ttu-id="42887-126">Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.</span><span class="sxs-lookup"><span data-stu-id="42887-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="42887-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="42887-127">mdmEnrolledCount</span></span>|<span data-ttu-id="42887-128">Int32</span><span class="sxs-lookup"><span data-stu-id="42887-128">Int32</span></span>|<span data-ttu-id="42887-129">Anzahl von in MDM registrierten Geräten</span><span class="sxs-lookup"><span data-stu-id="42887-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="42887-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="42887-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="42887-131">Int32</span><span class="sxs-lookup"><span data-stu-id="42887-131">Int32</span></span>|<span data-ttu-id="42887-132">Anzahl von Geräten, die in MDM und EAS registriert sind</span><span class="sxs-lookup"><span data-stu-id="42887-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="42887-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="42887-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="42887-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="42887-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="42887-135">Betriebssystemzusammenfassung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="42887-135">Device operating system summary.</span></span>|
|<span data-ttu-id="42887-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="42887-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="42887-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="42887-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="42887-138">Verteilung des Exchange-Zugriffsstatus in Intune</span><span class="sxs-lookup"><span data-stu-id="42887-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="42887-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="42887-139">Relationships</span></span>
<span data-ttu-id="42887-140">Keine</span><span class="sxs-lookup"><span data-stu-id="42887-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42887-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="42887-141">JSON Representation</span></span>
<span data-ttu-id="42887-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="42887-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```



