---
title: deviceConfigurationDeviceOverview-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe9c94c5ca430f72e2433755533ccb221063cda7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251951"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="30f09-103">deviceConfigurationDeviceOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="30f09-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="30f09-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="30f09-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30f09-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="30f09-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="30f09-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="30f09-106">Methods</span></span>
|<span data-ttu-id="30f09-107">Methode</span><span class="sxs-lookup"><span data-stu-id="30f09-107">Method</span></span>|<span data-ttu-id="30f09-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="30f09-108">Return Type</span></span>|<span data-ttu-id="30f09-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30f09-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="30f09-110">deviceConfigurationDeviceOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="30f09-110">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="30f09-111">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="30f09-111">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="30f09-112">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="30f09-112">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="30f09-113">deviceConfigurationDeviceOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="30f09-113">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="30f09-114">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="30f09-114">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="30f09-115">Aktualisieren der Eigenschaften eines [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="30f09-115">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="30f09-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="30f09-116">Properties</span></span>
|<span data-ttu-id="30f09-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="30f09-117">Property</span></span>|<span data-ttu-id="30f09-118">Typ</span><span class="sxs-lookup"><span data-stu-id="30f09-118">Type</span></span>|<span data-ttu-id="30f09-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30f09-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30f09-120">id</span><span class="sxs-lookup"><span data-stu-id="30f09-120">id</span></span>|<span data-ttu-id="30f09-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="30f09-121">String</span></span>|<span data-ttu-id="30f09-122">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="30f09-122">Key of the entity.</span></span>|
|<span data-ttu-id="30f09-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="30f09-123">pendingCount</span></span>|<span data-ttu-id="30f09-124">Int32</span><span class="sxs-lookup"><span data-stu-id="30f09-124">Int32</span></span>|<span data-ttu-id="30f09-125">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="30f09-125">Number of pending devices</span></span>|
|<span data-ttu-id="30f09-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="30f09-126">notApplicableCount</span></span>|<span data-ttu-id="30f09-127">Int32</span><span class="sxs-lookup"><span data-stu-id="30f09-127">Int32</span></span>|<span data-ttu-id="30f09-128">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="30f09-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="30f09-129">successCount</span><span class="sxs-lookup"><span data-stu-id="30f09-129">successCount</span></span>|<span data-ttu-id="30f09-130">Int32</span><span class="sxs-lookup"><span data-stu-id="30f09-130">Int32</span></span>|<span data-ttu-id="30f09-131">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="30f09-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="30f09-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="30f09-132">errorCount</span></span>|<span data-ttu-id="30f09-133">Int32</span><span class="sxs-lookup"><span data-stu-id="30f09-133">Int32</span></span>|<span data-ttu-id="30f09-134">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="30f09-134">Number of error devices</span></span>|
|<span data-ttu-id="30f09-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="30f09-135">failedCount</span></span>|<span data-ttu-id="30f09-136">Int32</span><span class="sxs-lookup"><span data-stu-id="30f09-136">Int32</span></span>|<span data-ttu-id="30f09-137">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="30f09-137">Number of failed devices</span></span>|
|<span data-ttu-id="30f09-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="30f09-138">lastUpdateDateTime</span></span>|<span data-ttu-id="30f09-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30f09-139">DateTimeOffset</span></span>|<span data-ttu-id="30f09-140">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="30f09-140">Last update time</span></span>|
|<span data-ttu-id="30f09-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="30f09-141">configurationVersion</span></span>|<span data-ttu-id="30f09-142">Int32</span><span class="sxs-lookup"><span data-stu-id="30f09-142">Int32</span></span>|<span data-ttu-id="30f09-143">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="30f09-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="30f09-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="30f09-144">Relationships</span></span>
<span data-ttu-id="30f09-145">Keine</span><span class="sxs-lookup"><span data-stu-id="30f09-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30f09-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="30f09-146">JSON Representation</span></span>
<span data-ttu-id="30f09-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="30f09-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



