---
title: deviceConfiguration-Ressourcentyp
description: Gerätekonfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1a508a037dbd1271d30a226d9cf62fb0683b53af
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953147"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="a59c6-103">deviceConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a59c6-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="a59c6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a59c6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a59c6-105">Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a59c6-105">Device Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="a59c6-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="a59c6-106">Methods</span></span>
|<span data-ttu-id="a59c6-107">Methode</span><span class="sxs-lookup"><span data-stu-id="a59c6-107">Method</span></span>|<span data-ttu-id="a59c6-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a59c6-108">Return Type</span></span>|<span data-ttu-id="a59c6-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a59c6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a59c6-110">deviceConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="a59c6-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="a59c6-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a59c6-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="a59c6-112">Auflisten von Eigenschaften und Beziehungen der [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="a59c6-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a59c6-113">deviceConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="a59c6-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="a59c6-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a59c6-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="a59c6-115">Lesen von Eigenschaften und Beziehungen des [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a59c6-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a59c6-116">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="a59c6-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="a59c6-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a59c6-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a59c6-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a59c6-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a59c6-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a59c6-119">Properties</span></span>
|<span data-ttu-id="a59c6-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a59c6-120">Property</span></span>|<span data-ttu-id="a59c6-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a59c6-121">Type</span></span>|<span data-ttu-id="a59c6-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a59c6-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a59c6-123">id</span><span class="sxs-lookup"><span data-stu-id="a59c6-123">id</span></span>|<span data-ttu-id="a59c6-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a59c6-124">String</span></span>|<span data-ttu-id="a59c6-125">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a59c6-125">Key of the entity.</span></span>|
|<span data-ttu-id="a59c6-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a59c6-126">lastModifiedDateTime</span></span>|<span data-ttu-id="a59c6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a59c6-127">DateTimeOffset</span></span>|<span data-ttu-id="a59c6-128">DateTime der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a59c6-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a59c6-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a59c6-129">createdDateTime</span></span>|<span data-ttu-id="a59c6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a59c6-130">DateTimeOffset</span></span>|<span data-ttu-id="a59c6-131">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="a59c6-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="a59c6-132">description</span><span class="sxs-lookup"><span data-stu-id="a59c6-132">description</span></span>|<span data-ttu-id="a59c6-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a59c6-133">String</span></span>|<span data-ttu-id="a59c6-134">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a59c6-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="a59c6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a59c6-135">displayName</span></span>|<span data-ttu-id="a59c6-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a59c6-136">String</span></span>|<span data-ttu-id="a59c6-137">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="a59c6-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="a59c6-138">version</span><span class="sxs-lookup"><span data-stu-id="a59c6-138">version</span></span>|<span data-ttu-id="a59c6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a59c6-139">Int32</span></span>|<span data-ttu-id="a59c6-140">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a59c6-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a59c6-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a59c6-141">Relationships</span></span>
|<span data-ttu-id="a59c6-142">Beziehung</span><span class="sxs-lookup"><span data-stu-id="a59c6-142">Relationship</span></span>|<span data-ttu-id="a59c6-143">Typ</span><span class="sxs-lookup"><span data-stu-id="a59c6-143">Type</span></span>|<span data-ttu-id="a59c6-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a59c6-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a59c6-145">assignments</span><span class="sxs-lookup"><span data-stu-id="a59c6-145">assignments</span></span>|<span data-ttu-id="a59c6-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a59c6-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a59c6-147">Die Liste der Zuweisungen für das Gerätekonfigurationsprofil.</span><span class="sxs-lookup"><span data-stu-id="a59c6-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="a59c6-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a59c6-148">deviceStatuses</span></span>|<span data-ttu-id="a59c6-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a59c6-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a59c6-150">Installationsstatus der Gerätekonfiguration nach Gerät.</span><span class="sxs-lookup"><span data-stu-id="a59c6-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="a59c6-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a59c6-151">userStatuses</span></span>|<span data-ttu-id="a59c6-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a59c6-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a59c6-153">Gerät Konfiguration Installationsstatus durch Benutzer.</span><span class="sxs-lookup"><span data-stu-id="a59c6-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="a59c6-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a59c6-154">deviceStatusOverview</span></span>|[<span data-ttu-id="a59c6-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a59c6-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="a59c6-156">Übersicht über Gerätestatus der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="a59c6-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="a59c6-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a59c6-157">userStatusOverview</span></span>|[<span data-ttu-id="a59c6-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="a59c6-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="a59c6-159">Übersicht über Benutzerstatus der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="a59c6-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="a59c6-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a59c6-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a59c6-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a59c6-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a59c6-162">Übersicht über den Status der Gerätekonfigurationseinstellungen der Geräte</span><span class="sxs-lookup"><span data-stu-id="a59c6-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a59c6-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a59c6-163">JSON Representation</span></span>
<span data-ttu-id="a59c6-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a59c6-164">Here is a JSON representation of the resource.</span></span>
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



