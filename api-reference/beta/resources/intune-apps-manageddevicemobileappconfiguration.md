---
title: managedDeviceMobileAppConfiguration-Ressourcentyp
description: Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90ac67285ba856916194d30831f556ce6b521dbd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400144"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="ffb63-103">managedDeviceMobileAppConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ffb63-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="ffb63-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ffb63-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ffb63-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ffb63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffb63-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ffb63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffb63-107">Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.</span><span class="sxs-lookup"><span data-stu-id="ffb63-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="ffb63-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="ffb63-108">Methods</span></span>
|<span data-ttu-id="ffb63-109">Methode</span><span class="sxs-lookup"><span data-stu-id="ffb63-109">Method</span></span>|<span data-ttu-id="ffb63-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ffb63-110">Return Type</span></span>|<span data-ttu-id="ffb63-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffb63-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ffb63-112">managedDeviceMobileAppConfigurations auflisten</span><span class="sxs-lookup"><span data-stu-id="ffb63-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="ffb63-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ffb63-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="ffb63-114">Auflisten von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="ffb63-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ffb63-115">managedDeviceMobileAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="ffb63-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="ffb63-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ffb63-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="ffb63-117">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ffb63-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ffb63-118">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="ffb63-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="ffb63-119">Keine</span><span class="sxs-lookup"><span data-stu-id="ffb63-119">None</span></span>|<span data-ttu-id="ffb63-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ffb63-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ffb63-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ffb63-121">Properties</span></span>
|<span data-ttu-id="ffb63-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ffb63-122">Property</span></span>|<span data-ttu-id="ffb63-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ffb63-123">Type</span></span>|<span data-ttu-id="ffb63-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffb63-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffb63-125">id</span><span class="sxs-lookup"><span data-stu-id="ffb63-125">id</span></span>|<span data-ttu-id="ffb63-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffb63-126">String</span></span>|<span data-ttu-id="ffb63-127">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="ffb63-127">Key of the entity.</span></span>|
|<span data-ttu-id="ffb63-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ffb63-128">targetedMobileApps</span></span>|<span data-ttu-id="ffb63-129">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ffb63-129">String collection</span></span>|<span data-ttu-id="ffb63-130">Die zugeordnete App.</span><span class="sxs-lookup"><span data-stu-id="ffb63-130">the associated app.</span></span>|
|<span data-ttu-id="ffb63-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ffb63-131">roleScopeTagIds</span></span>|<span data-ttu-id="ffb63-132">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ffb63-132">String collection</span></span>|<span data-ttu-id="ffb63-133">Liste der Bereich Tags für diese App Konfigurationsentität.</span><span class="sxs-lookup"><span data-stu-id="ffb63-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="ffb63-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffb63-134">createdDateTime</span></span>|<span data-ttu-id="ffb63-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffb63-135">DateTimeOffset</span></span>|<span data-ttu-id="ffb63-136">Datum und Uhrzeit der Erstellung des Objekts</span><span class="sxs-lookup"><span data-stu-id="ffb63-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="ffb63-137">description</span><span class="sxs-lookup"><span data-stu-id="ffb63-137">description</span></span>|<span data-ttu-id="ffb63-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffb63-138">String</span></span>|<span data-ttu-id="ffb63-139">Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="ffb63-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="ffb63-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffb63-140">lastModifiedDateTime</span></span>|<span data-ttu-id="ffb63-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffb63-141">DateTimeOffset</span></span>|<span data-ttu-id="ffb63-142">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ffb63-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ffb63-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ffb63-143">displayName</span></span>|<span data-ttu-id="ffb63-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ffb63-144">String</span></span>|<span data-ttu-id="ffb63-145">Vom Administrator bereitgestellter Name der Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="ffb63-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="ffb63-146">version</span><span class="sxs-lookup"><span data-stu-id="ffb63-146">version</span></span>|<span data-ttu-id="ffb63-147">Int32</span><span class="sxs-lookup"><span data-stu-id="ffb63-147">Int32</span></span>|<span data-ttu-id="ffb63-148">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ffb63-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffb63-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ffb63-149">Relationships</span></span>
|<span data-ttu-id="ffb63-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="ffb63-150">Relationship</span></span>|<span data-ttu-id="ffb63-151">Typ</span><span class="sxs-lookup"><span data-stu-id="ffb63-151">Type</span></span>|<span data-ttu-id="ffb63-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffb63-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffb63-153">assignments</span><span class="sxs-lookup"><span data-stu-id="ffb63-153">assignments</span></span>|<span data-ttu-id="ffb63-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ffb63-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ffb63-155">Die Liste der Gruppenzuweisungen für die App-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="ffb63-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="ffb63-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ffb63-156">deviceStatuses</span></span>|<span data-ttu-id="ffb63-157">[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ffb63-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="ffb63-158">Liste der ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="ffb63-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="ffb63-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="ffb63-159">userStatuses</span></span>|<span data-ttu-id="ffb63-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ffb63-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="ffb63-161">Liste von ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="ffb63-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="ffb63-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="ffb63-162">deviceStatusSummary</span></span>|[<span data-ttu-id="ffb63-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="ffb63-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="ffb63-164">Zusammenfassung der App-Konfiguration-Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="ffb63-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="ffb63-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="ffb63-165">userStatusSummary</span></span>|[<span data-ttu-id="ffb63-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="ffb63-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="ffb63-167">Zusammenfassung der App-Konfiguration-Benutzerstatus.</span><span class="sxs-lookup"><span data-stu-id="ffb63-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffb63-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ffb63-168">JSON Representation</span></span>
<span data-ttu-id="ffb63-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ffb63-169">Here is a JSON representation of the resource.</span></span>
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




