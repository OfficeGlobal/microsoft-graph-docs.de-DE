---
title: deviceConfiguration-Ressourcentyp
description: Gerätekonfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a3d0ecc27fc0fe29ed2ed3ca4080e3fea70d264
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250495"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="c7f98-103">deviceConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c7f98-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="c7f98-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c7f98-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7f98-105">Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c7f98-105">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="c7f98-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="c7f98-106">Methods</span></span>
|<span data-ttu-id="c7f98-107">Methode</span><span class="sxs-lookup"><span data-stu-id="c7f98-107">Method</span></span>|<span data-ttu-id="c7f98-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c7f98-108">Return Type</span></span>|<span data-ttu-id="c7f98-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7f98-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7f98-110">deviceConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="c7f98-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="c7f98-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c7f98-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="c7f98-112">Auflisten von Eigenschaften und Beziehungen der [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="c7f98-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c7f98-113">deviceConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="c7f98-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="c7f98-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7f98-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="c7f98-115">Lesen von Eigenschaften und Beziehungen des [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7f98-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c7f98-116">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="c7f98-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="c7f98-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c7f98-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c7f98-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c7f98-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c7f98-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7f98-119">Properties</span></span>
|<span data-ttu-id="c7f98-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7f98-120">Property</span></span>|<span data-ttu-id="c7f98-121">Typ</span><span class="sxs-lookup"><span data-stu-id="c7f98-121">Type</span></span>|<span data-ttu-id="c7f98-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7f98-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7f98-123">id</span><span class="sxs-lookup"><span data-stu-id="c7f98-123">id</span></span>|<span data-ttu-id="c7f98-124">string</span><span class="sxs-lookup"><span data-stu-id="c7f98-124">String</span></span>|<span data-ttu-id="c7f98-125">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c7f98-125">Key of the entity.</span></span>|
|<span data-ttu-id="c7f98-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f98-126">lastModifiedDateTime</span></span>|<span data-ttu-id="c7f98-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f98-127">DateTimeOffset</span></span>|<span data-ttu-id="c7f98-128">DateTime der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7f98-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c7f98-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f98-129">createdDateTime</span></span>|<span data-ttu-id="c7f98-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f98-130">DateTimeOffset</span></span>|<span data-ttu-id="c7f98-131">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="c7f98-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="c7f98-132">description</span><span class="sxs-lookup"><span data-stu-id="c7f98-132">description</span></span>|<span data-ttu-id="c7f98-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7f98-133">String</span></span>|<span data-ttu-id="c7f98-134">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c7f98-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c7f98-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c7f98-135">displayName</span></span>|<span data-ttu-id="c7f98-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7f98-136">String</span></span>|<span data-ttu-id="c7f98-137">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="c7f98-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c7f98-138">version</span><span class="sxs-lookup"><span data-stu-id="c7f98-138">version</span></span>|<span data-ttu-id="c7f98-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f98-139">Int32</span></span>|<span data-ttu-id="c7f98-140">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c7f98-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7f98-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c7f98-141">Relationships</span></span>
|<span data-ttu-id="c7f98-142">Beziehung</span><span class="sxs-lookup"><span data-stu-id="c7f98-142">Relationship</span></span>|<span data-ttu-id="c7f98-143">Typ</span><span class="sxs-lookup"><span data-stu-id="c7f98-143">Type</span></span>|<span data-ttu-id="c7f98-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7f98-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7f98-145">assignments</span><span class="sxs-lookup"><span data-stu-id="c7f98-145">assignments</span></span>|<span data-ttu-id="c7f98-146">Sammlung von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7f98-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c7f98-147">Die Liste der Zuweisungen für das Gerätekonfigurationsprofil.</span><span class="sxs-lookup"><span data-stu-id="c7f98-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="c7f98-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c7f98-148">deviceStatuses</span></span>|<span data-ttu-id="c7f98-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c7f98-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="c7f98-150">Installationsstatus der Gerätekonfiguration nach Gerät.</span><span class="sxs-lookup"><span data-stu-id="c7f98-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="c7f98-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c7f98-151">userStatuses</span></span>|<span data-ttu-id="c7f98-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c7f98-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="c7f98-153">Installationsstatus der Gerätekonfiguration nach Benutzer.</span><span class="sxs-lookup"><span data-stu-id="c7f98-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="c7f98-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c7f98-154">deviceStatusOverview</span></span>|[<span data-ttu-id="c7f98-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c7f98-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="c7f98-156">Übersicht über Gerätestatus der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="c7f98-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="c7f98-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c7f98-157">userStatusOverview</span></span>|[<span data-ttu-id="c7f98-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c7f98-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c7f98-159">Übersicht über Benutzerstatus der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="c7f98-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="c7f98-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c7f98-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c7f98-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c7f98-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c7f98-162">Übersicht über den Status der Gerätekonfigurationseinstellungen der Geräte</span><span class="sxs-lookup"><span data-stu-id="c7f98-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7f98-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7f98-163">JSON Representation</span></span>
<span data-ttu-id="c7f98-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7f98-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```



