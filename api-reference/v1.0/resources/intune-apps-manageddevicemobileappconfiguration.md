---
title: managedDeviceMobileAppConfiguration-Ressourcentyp
description: Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1a249325f7e4c9be196c5adda695b84e5f8a94c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258597"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="152ff-103">managedDeviceMobileAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="152ff-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="152ff-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="152ff-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="152ff-105">Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.</span><span class="sxs-lookup"><span data-stu-id="152ff-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="152ff-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="152ff-106">Methods</span></span>
|<span data-ttu-id="152ff-107">Methode</span><span class="sxs-lookup"><span data-stu-id="152ff-107">Method</span></span>|<span data-ttu-id="152ff-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="152ff-108">Return Type</span></span>|<span data-ttu-id="152ff-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="152ff-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="152ff-110">managedDeviceMobileAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="152ff-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="152ff-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="152ff-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="152ff-112">Auflisten von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="152ff-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="152ff-113">managedDeviceMobileAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="152ff-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="152ff-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="152ff-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="152ff-115">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="152ff-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="152ff-116">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="152ff-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="152ff-117">Keine</span><span class="sxs-lookup"><span data-stu-id="152ff-117">None</span></span>|<span data-ttu-id="152ff-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="152ff-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="152ff-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="152ff-119">Properties</span></span>
|<span data-ttu-id="152ff-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="152ff-120">Property</span></span>|<span data-ttu-id="152ff-121">Typ</span><span class="sxs-lookup"><span data-stu-id="152ff-121">Type</span></span>|<span data-ttu-id="152ff-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="152ff-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="152ff-123">id</span><span class="sxs-lookup"><span data-stu-id="152ff-123">id</span></span>|<span data-ttu-id="152ff-124">string</span><span class="sxs-lookup"><span data-stu-id="152ff-124">String</span></span>|<span data-ttu-id="152ff-125">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="152ff-125">Key of the entity.</span></span>|
|<span data-ttu-id="152ff-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="152ff-126">targetedMobileApps</span></span>|<span data-ttu-id="152ff-127">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="152ff-127">String collection</span></span>|<span data-ttu-id="152ff-128">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="152ff-128">the associated app.</span></span>|
|<span data-ttu-id="152ff-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="152ff-129">createdDateTime</span></span>|<span data-ttu-id="152ff-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="152ff-130">DateTimeOffset</span></span>|<span data-ttu-id="152ff-131">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="152ff-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="152ff-132">description</span><span class="sxs-lookup"><span data-stu-id="152ff-132">description</span></span>|<span data-ttu-id="152ff-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="152ff-133">String</span></span>|<span data-ttu-id="152ff-134">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="152ff-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="152ff-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="152ff-135">lastModifiedDateTime</span></span>|<span data-ttu-id="152ff-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="152ff-136">DateTimeOffset</span></span>|<span data-ttu-id="152ff-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="152ff-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="152ff-138">displayName</span><span class="sxs-lookup"><span data-stu-id="152ff-138">displayName</span></span>|<span data-ttu-id="152ff-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="152ff-139">String</span></span>|<span data-ttu-id="152ff-140">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="152ff-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="152ff-141">version</span><span class="sxs-lookup"><span data-stu-id="152ff-141">version</span></span>|<span data-ttu-id="152ff-142">Int32</span><span class="sxs-lookup"><span data-stu-id="152ff-142">Int32</span></span>|<span data-ttu-id="152ff-143">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="152ff-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="152ff-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="152ff-144">Relationships</span></span>
|<span data-ttu-id="152ff-145">Beziehung</span><span class="sxs-lookup"><span data-stu-id="152ff-145">Relationship</span></span>|<span data-ttu-id="152ff-146">Typ</span><span class="sxs-lookup"><span data-stu-id="152ff-146">Type</span></span>|<span data-ttu-id="152ff-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="152ff-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="152ff-148">assignments</span><span class="sxs-lookup"><span data-stu-id="152ff-148">assignments</span></span>|<span data-ttu-id="152ff-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="152ff-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="152ff-150">Die Liste der Gruppenzuweisungen für die App-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="152ff-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="152ff-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="152ff-151">deviceStatuses</span></span>|<span data-ttu-id="152ff-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="152ff-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="152ff-153">Liste der ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="152ff-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="152ff-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="152ff-154">userStatuses</span></span>|<span data-ttu-id="152ff-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="152ff-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="152ff-156">Liste von ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="152ff-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="152ff-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="152ff-157">deviceStatusSummary</span></span>|[<span data-ttu-id="152ff-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="152ff-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="152ff-159">Zusammenfassung der App-Konfiguration-Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="152ff-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="152ff-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="152ff-160">userStatusSummary</span></span>|[<span data-ttu-id="152ff-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="152ff-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="152ff-162">Zusammenfassung der App-Konfiguration-Benutzerstatus.</span><span class="sxs-lookup"><span data-stu-id="152ff-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="152ff-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="152ff-163">JSON Representation</span></span>
<span data-ttu-id="152ff-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="152ff-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



