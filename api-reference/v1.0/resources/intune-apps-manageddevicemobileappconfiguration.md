---
title: managedDeviceMobileAppConfiguration-Ressourcentyp
description: Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.
ms.openlocfilehash: dd3b77b3e53c1eacc049af35274e20c5bbaa8e14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016075"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="fa2bc-103">managedDeviceMobileAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fa2bc-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="fa2bc-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa2bc-105">Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="fa2bc-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="fa2bc-106">Methods</span></span>
|<span data-ttu-id="fa2bc-107">Methode</span><span class="sxs-lookup"><span data-stu-id="fa2bc-107">Method</span></span>|<span data-ttu-id="fa2bc-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fa2bc-108">Return Type</span></span>|<span data-ttu-id="fa2bc-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa2bc-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fa2bc-110">managedDeviceMobileAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="fa2bc-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="fa2bc-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fa2bc-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="fa2bc-112">Auflisten von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="fa2bc-113">managedDeviceMobileAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="fa2bc-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="fa2bc-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa2bc-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="fa2bc-115">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="fa2bc-116">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="fa2bc-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="fa2bc-117">Keine</span><span class="sxs-lookup"><span data-stu-id="fa2bc-117">None</span></span>|<span data-ttu-id="fa2bc-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fa2bc-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fa2bc-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fa2bc-119">Properties</span></span>
|<span data-ttu-id="fa2bc-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa2bc-120">Property</span></span>|<span data-ttu-id="fa2bc-121">Typ</span><span class="sxs-lookup"><span data-stu-id="fa2bc-121">Type</span></span>|<span data-ttu-id="fa2bc-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa2bc-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa2bc-123">id</span><span class="sxs-lookup"><span data-stu-id="fa2bc-123">id</span></span>|<span data-ttu-id="fa2bc-124">String</span><span class="sxs-lookup"><span data-stu-id="fa2bc-124">String</span></span>|<span data-ttu-id="fa2bc-125">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-125">Key of the entity.</span></span>|
|<span data-ttu-id="fa2bc-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="fa2bc-126">targetedMobileApps</span></span>|<span data-ttu-id="fa2bc-127">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fa2bc-127">String collection</span></span>|<span data-ttu-id="fa2bc-128">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-128">the associated app.</span></span>|
|<span data-ttu-id="fa2bc-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa2bc-129">createdDateTime</span></span>|<span data-ttu-id="fa2bc-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa2bc-130">DateTimeOffset</span></span>|<span data-ttu-id="fa2bc-131">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="fa2bc-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="fa2bc-132">description</span><span class="sxs-lookup"><span data-stu-id="fa2bc-132">description</span></span>|<span data-ttu-id="fa2bc-133">String</span><span class="sxs-lookup"><span data-stu-id="fa2bc-133">String</span></span>|<span data-ttu-id="fa2bc-134">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="fa2bc-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="fa2bc-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa2bc-135">lastModifiedDateTime</span></span>|<span data-ttu-id="fa2bc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa2bc-136">DateTimeOffset</span></span>|<span data-ttu-id="fa2bc-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="fa2bc-138">displayName</span><span class="sxs-lookup"><span data-stu-id="fa2bc-138">displayName</span></span>|<span data-ttu-id="fa2bc-139">String</span><span class="sxs-lookup"><span data-stu-id="fa2bc-139">String</span></span>|<span data-ttu-id="fa2bc-140">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="fa2bc-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="fa2bc-141">version</span><span class="sxs-lookup"><span data-stu-id="fa2bc-141">version</span></span>|<span data-ttu-id="fa2bc-142">Int32</span><span class="sxs-lookup"><span data-stu-id="fa2bc-142">Int32</span></span>|<span data-ttu-id="fa2bc-143">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa2bc-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fa2bc-144">Relationships</span></span>
|<span data-ttu-id="fa2bc-145">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fa2bc-145">Relationship</span></span>|<span data-ttu-id="fa2bc-146">Typ</span><span class="sxs-lookup"><span data-stu-id="fa2bc-146">Type</span></span>|<span data-ttu-id="fa2bc-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa2bc-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa2bc-148">assignments</span><span class="sxs-lookup"><span data-stu-id="fa2bc-148">assignments</span></span>|<span data-ttu-id="fa2bc-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fa2bc-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="fa2bc-150">Die Liste der Gruppenzuweisungen für die App-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="fa2bc-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="fa2bc-151">deviceStatuses</span></span>|<span data-ttu-id="fa2bc-152">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="fa2bc-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="fa2bc-153">Liste der ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="fa2bc-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="fa2bc-154">userStatuses</span></span>|<span data-ttu-id="fa2bc-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fa2bc-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="fa2bc-156">Liste von ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="fa2bc-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="fa2bc-157">deviceStatusSummary</span></span>|[<span data-ttu-id="fa2bc-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="fa2bc-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="fa2bc-159">Zusammenfassung der App-Konfiguration-Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="fa2bc-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="fa2bc-160">userStatusSummary</span></span>|[<span data-ttu-id="fa2bc-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="fa2bc-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="fa2bc-162">Zusammenfassung der App-Konfiguration-Benutzerstatus.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa2bc-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fa2bc-163">JSON Representation</span></span>
<span data-ttu-id="fa2bc-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fa2bc-164">Here is a JSON representation of the resource.</span></span>
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



