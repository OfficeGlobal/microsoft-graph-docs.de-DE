---
title: deviceConfigurationDeviceStateSummary-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: f298f2c93bcf886fc209184386951328395bfcbb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316926"
---
# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="0b249-103">deviceConfigurationDeviceStateSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0b249-103">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="0b249-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0b249-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b249-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0b249-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="0b249-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="0b249-106">Methods</span></span>
|<span data-ttu-id="0b249-107">Methode</span><span class="sxs-lookup"><span data-stu-id="0b249-107">Method</span></span>|<span data-ttu-id="0b249-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0b249-108">Return Type</span></span>|<span data-ttu-id="0b249-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b249-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0b249-110">deviceConfigurationDeviceStateSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="0b249-110">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-get.md)|[<span data-ttu-id="0b249-111">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="0b249-111">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="0b249-112">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0b249-112">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="0b249-113">deviceConfigurationDeviceStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0b249-113">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-update.md)|[<span data-ttu-id="0b249-114">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="0b249-114">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="0b249-115">Aktualisieren der Eigenschaften eines [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0b249-115">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b249-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0b249-116">Properties</span></span>
|<span data-ttu-id="0b249-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b249-117">Property</span></span>|<span data-ttu-id="0b249-118">Typ</span><span class="sxs-lookup"><span data-stu-id="0b249-118">Type</span></span>|<span data-ttu-id="0b249-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b249-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b249-120">id</span><span class="sxs-lookup"><span data-stu-id="0b249-120">id</span></span>|<span data-ttu-id="0b249-121">String</span><span class="sxs-lookup"><span data-stu-id="0b249-121">String</span></span>|<span data-ttu-id="0b249-122">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0b249-122">Key of the entity.</span></span>|
|<span data-ttu-id="0b249-123">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b249-123">unknownDeviceCount</span></span>|<span data-ttu-id="0b249-124">Int32</span><span class="sxs-lookup"><span data-stu-id="0b249-124">Int32</span></span>|<span data-ttu-id="0b249-125">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="0b249-125">Number of unknown devices</span></span>|
|<span data-ttu-id="0b249-126">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b249-126">notApplicableDeviceCount</span></span>|<span data-ttu-id="0b249-127">Int32</span><span class="sxs-lookup"><span data-stu-id="0b249-127">Int32</span></span>|<span data-ttu-id="0b249-128">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="0b249-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="0b249-129">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b249-129">compliantDeviceCount</span></span>|<span data-ttu-id="0b249-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0b249-130">Int32</span></span>|<span data-ttu-id="0b249-131">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="0b249-131">Number of compliant devices</span></span>|
|<span data-ttu-id="0b249-132">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b249-132">remediatedDeviceCount</span></span>|<span data-ttu-id="0b249-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0b249-133">Int32</span></span>|<span data-ttu-id="0b249-134">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="0b249-134">Number of remediated devices</span></span>|
|<span data-ttu-id="0b249-135">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b249-135">nonCompliantDeviceCount</span></span>|<span data-ttu-id="0b249-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0b249-136">Int32</span></span>|<span data-ttu-id="0b249-137">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="0b249-137">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="0b249-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b249-138">errorDeviceCount</span></span>|<span data-ttu-id="0b249-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0b249-139">Int32</span></span>|<span data-ttu-id="0b249-140">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="0b249-140">Number of error devices</span></span>|
|<span data-ttu-id="0b249-141">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b249-141">conflictDeviceCount</span></span>|<span data-ttu-id="0b249-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0b249-142">Int32</span></span>|<span data-ttu-id="0b249-143">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="0b249-143">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b249-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0b249-144">Relationships</span></span>
<span data-ttu-id="0b249-145">Keine</span><span class="sxs-lookup"><span data-stu-id="0b249-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b249-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0b249-146">JSON Representation</span></span>
<span data-ttu-id="0b249-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0b249-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



