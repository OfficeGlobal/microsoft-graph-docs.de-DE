---
title: managedDeviceMobileAppConfiguration-Ressourcentyp
description: Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dacccb00a30028a5b9e5144eb843ca52c60da876
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154250"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="3783f-103">managedDeviceMobileAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3783f-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="3783f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3783f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3783f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3783f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3783f-106">Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.</span><span class="sxs-lookup"><span data-stu-id="3783f-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="3783f-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="3783f-107">Methods</span></span>
|<span data-ttu-id="3783f-108">Methode</span><span class="sxs-lookup"><span data-stu-id="3783f-108">Method</span></span>|<span data-ttu-id="3783f-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3783f-109">Return Type</span></span>|<span data-ttu-id="3783f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3783f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3783f-111">managedDeviceMobileAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="3783f-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="3783f-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3783f-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="3783f-113">Auflisten von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="3783f-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3783f-114">managedDeviceMobileAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="3783f-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="3783f-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3783f-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="3783f-116">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3783f-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3783f-117">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="3783f-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="3783f-118">Keine</span><span class="sxs-lookup"><span data-stu-id="3783f-118">None</span></span>|<span data-ttu-id="3783f-119">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3783f-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3783f-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3783f-120">Properties</span></span>
|<span data-ttu-id="3783f-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3783f-121">Property</span></span>|<span data-ttu-id="3783f-122">Typ</span><span class="sxs-lookup"><span data-stu-id="3783f-122">Type</span></span>|<span data-ttu-id="3783f-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3783f-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3783f-124">id</span><span class="sxs-lookup"><span data-stu-id="3783f-124">id</span></span>|<span data-ttu-id="3783f-125">string</span><span class="sxs-lookup"><span data-stu-id="3783f-125">String</span></span>|<span data-ttu-id="3783f-126">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="3783f-126">Key of the entity.</span></span>|
|<span data-ttu-id="3783f-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="3783f-127">targetedMobileApps</span></span>|<span data-ttu-id="3783f-128">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3783f-128">String collection</span></span>|<span data-ttu-id="3783f-129">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="3783f-129">the associated app.</span></span>|
|<span data-ttu-id="3783f-130">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="3783f-130">roleScopeTagIds</span></span>|<span data-ttu-id="3783f-131">String collection</span><span class="sxs-lookup"><span data-stu-id="3783f-131">String collection</span></span>|<span data-ttu-id="3783f-132">Liste der Bereichs Tags für diese APP-Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="3783f-132">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="3783f-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3783f-133">createdDateTime</span></span>|<span data-ttu-id="3783f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3783f-134">DateTimeOffset</span></span>|<span data-ttu-id="3783f-135">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="3783f-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="3783f-136">description</span><span class="sxs-lookup"><span data-stu-id="3783f-136">description</span></span>|<span data-ttu-id="3783f-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3783f-137">String</span></span>|<span data-ttu-id="3783f-138">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="3783f-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="3783f-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3783f-139">lastModifiedDateTime</span></span>|<span data-ttu-id="3783f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3783f-140">DateTimeOffset</span></span>|<span data-ttu-id="3783f-141">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3783f-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3783f-142">displayName</span><span class="sxs-lookup"><span data-stu-id="3783f-142">displayName</span></span>|<span data-ttu-id="3783f-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3783f-143">String</span></span>|<span data-ttu-id="3783f-144">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="3783f-144">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="3783f-145">version</span><span class="sxs-lookup"><span data-stu-id="3783f-145">version</span></span>|<span data-ttu-id="3783f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3783f-146">Int32</span></span>|<span data-ttu-id="3783f-147">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3783f-147">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3783f-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3783f-148">Relationships</span></span>
|<span data-ttu-id="3783f-149">Beziehung</span><span class="sxs-lookup"><span data-stu-id="3783f-149">Relationship</span></span>|<span data-ttu-id="3783f-150">Typ</span><span class="sxs-lookup"><span data-stu-id="3783f-150">Type</span></span>|<span data-ttu-id="3783f-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3783f-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3783f-152">assignments</span><span class="sxs-lookup"><span data-stu-id="3783f-152">assignments</span></span>|<span data-ttu-id="3783f-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3783f-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3783f-154">Die Liste der Gruppenzuweisungen für die App-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="3783f-154">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="3783f-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3783f-155">deviceStatuses</span></span>|<span data-ttu-id="3783f-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="3783f-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="3783f-157">Liste der ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="3783f-157">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="3783f-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="3783f-158">userStatuses</span></span>|<span data-ttu-id="3783f-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3783f-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="3783f-160">Liste von ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="3783f-160">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="3783f-161">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="3783f-161">deviceStatusSummary</span></span>|[<span data-ttu-id="3783f-162">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="3783f-162">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="3783f-163">Zusammenfassung der App-Konfiguration-Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="3783f-163">App configuration device status summary.</span></span>|
|<span data-ttu-id="3783f-164">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="3783f-164">userStatusSummary</span></span>|[<span data-ttu-id="3783f-165">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="3783f-165">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="3783f-166">Zusammenfassung der App-Konfiguration-Benutzerstatus.</span><span class="sxs-lookup"><span data-stu-id="3783f-166">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3783f-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3783f-167">JSON Representation</span></span>
<span data-ttu-id="3783f-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3783f-168">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




