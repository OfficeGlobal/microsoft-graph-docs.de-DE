---
title: managedDeviceMobileAppConfiguration-Ressourcentyp
description: Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.
author: tfitzmac
ms.openlocfilehash: a533d5d7c15a32d811a7fd23f9ab39b89db9b7da
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352038"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="14cac-103">managedDeviceMobileAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="14cac-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="14cac-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="14cac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14cac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="14cac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14cac-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="14cac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14cac-107">Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.</span><span class="sxs-lookup"><span data-stu-id="14cac-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="14cac-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="14cac-108">Methods</span></span>
|<span data-ttu-id="14cac-109">Methode</span><span class="sxs-lookup"><span data-stu-id="14cac-109">Method</span></span>|<span data-ttu-id="14cac-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="14cac-110">Return Type</span></span>|<span data-ttu-id="14cac-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14cac-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14cac-112">managedDeviceMobileAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="14cac-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="14cac-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="14cac-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="14cac-114">Auflisten von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="14cac-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="14cac-115">managedDeviceMobileAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="14cac-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="14cac-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="14cac-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="14cac-117">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="14cac-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="14cac-118">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="14cac-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="14cac-119">Keine</span><span class="sxs-lookup"><span data-stu-id="14cac-119">None</span></span>|<span data-ttu-id="14cac-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="14cac-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="14cac-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="14cac-121">Properties</span></span>
|<span data-ttu-id="14cac-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14cac-122">Property</span></span>|<span data-ttu-id="14cac-123">Typ</span><span class="sxs-lookup"><span data-stu-id="14cac-123">Type</span></span>|<span data-ttu-id="14cac-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14cac-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14cac-125">id</span><span class="sxs-lookup"><span data-stu-id="14cac-125">id</span></span>|<span data-ttu-id="14cac-126">String</span><span class="sxs-lookup"><span data-stu-id="14cac-126">String</span></span>|<span data-ttu-id="14cac-127">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="14cac-127">Key of the entity.</span></span>|
|<span data-ttu-id="14cac-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="14cac-128">targetedMobileApps</span></span>|<span data-ttu-id="14cac-129">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="14cac-129">String collection</span></span>|<span data-ttu-id="14cac-130">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="14cac-130">the associated app.</span></span>|
|<span data-ttu-id="14cac-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14cac-131">roleScopeTagIds</span></span>|<span data-ttu-id="14cac-132">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="14cac-132">String collection</span></span>|<span data-ttu-id="14cac-133">Liste der Bereich Tags für diese App Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="14cac-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="14cac-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14cac-134">createdDateTime</span></span>|<span data-ttu-id="14cac-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14cac-135">DateTimeOffset</span></span>|<span data-ttu-id="14cac-136">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="14cac-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="14cac-137">description</span><span class="sxs-lookup"><span data-stu-id="14cac-137">description</span></span>|<span data-ttu-id="14cac-138">String</span><span class="sxs-lookup"><span data-stu-id="14cac-138">String</span></span>|<span data-ttu-id="14cac-139">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="14cac-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="14cac-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14cac-140">lastModifiedDateTime</span></span>|<span data-ttu-id="14cac-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14cac-141">DateTimeOffset</span></span>|<span data-ttu-id="14cac-142">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="14cac-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="14cac-143">displayName</span><span class="sxs-lookup"><span data-stu-id="14cac-143">displayName</span></span>|<span data-ttu-id="14cac-144">String</span><span class="sxs-lookup"><span data-stu-id="14cac-144">String</span></span>|<span data-ttu-id="14cac-145">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="14cac-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="14cac-146">version</span><span class="sxs-lookup"><span data-stu-id="14cac-146">version</span></span>|<span data-ttu-id="14cac-147">Int32</span><span class="sxs-lookup"><span data-stu-id="14cac-147">Int32</span></span>|<span data-ttu-id="14cac-148">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="14cac-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14cac-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="14cac-149">Relationships</span></span>
|<span data-ttu-id="14cac-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="14cac-150">Relationship</span></span>|<span data-ttu-id="14cac-151">Typ</span><span class="sxs-lookup"><span data-stu-id="14cac-151">Type</span></span>|<span data-ttu-id="14cac-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14cac-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14cac-153">assignments</span><span class="sxs-lookup"><span data-stu-id="14cac-153">assignments</span></span>|<span data-ttu-id="14cac-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="14cac-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="14cac-155">Die Liste der Gruppenzuweisungen für die App-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="14cac-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="14cac-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="14cac-156">deviceStatuses</span></span>|<span data-ttu-id="14cac-157">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="14cac-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="14cac-158">Liste der ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="14cac-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="14cac-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="14cac-159">userStatuses</span></span>|<span data-ttu-id="14cac-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="14cac-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="14cac-161">Liste von ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="14cac-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="14cac-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="14cac-162">deviceStatusSummary</span></span>|[<span data-ttu-id="14cac-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="14cac-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="14cac-164">Zusammenfassung der App-Konfiguration-Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="14cac-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="14cac-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="14cac-165">userStatusSummary</span></span>|[<span data-ttu-id="14cac-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="14cac-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="14cac-167">Zusammenfassung der App-Konfiguration-Benutzerstatus.</span><span class="sxs-lookup"><span data-stu-id="14cac-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14cac-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="14cac-168">JSON Representation</span></span>
<span data-ttu-id="14cac-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="14cac-169">Here is a JSON representation of the resource.</span></span>
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





