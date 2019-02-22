---
title: restrictedAppsViolation-Ressourcentyp
description: Verletzung des Konfigurationsprofils für eingeschränkte apps pro Gerät und Benutzer
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8764d3d84ba0706f3769ef019def43cb080660d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139914"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="cba0b-103">restrictedAppsViolation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cba0b-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="cba0b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cba0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cba0b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cba0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cba0b-106">Verletzung des Konfigurationsprofils für eingeschränkte apps pro Gerät und Benutzer</span><span class="sxs-lookup"><span data-stu-id="cba0b-106">Violation of restricted apps configuration profile per device per user</span></span>

## <a name="methods"></a><span data-ttu-id="cba0b-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="cba0b-107">Methods</span></span>
|<span data-ttu-id="cba0b-108">Methode</span><span class="sxs-lookup"><span data-stu-id="cba0b-108">Method</span></span>|<span data-ttu-id="cba0b-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cba0b-109">Return Type</span></span>|<span data-ttu-id="cba0b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cba0b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cba0b-111">RestrictedAppsViolations aufListen</span><span class="sxs-lookup"><span data-stu-id="cba0b-111">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="cba0b-112">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="cba0b-112">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="cba0b-113">AufListen von Eigenschaften und Beziehungen der [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="cba0b-113">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="cba0b-114">RestrictedAppsViolation abrufen</span><span class="sxs-lookup"><span data-stu-id="cba0b-114">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="cba0b-115">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="cba0b-115">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="cba0b-116">Lesen von Eigenschaften und Beziehungen des [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cba0b-116">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="cba0b-117">RestrictedAppsViolation erstellen</span><span class="sxs-lookup"><span data-stu-id="cba0b-117">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="cba0b-118">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="cba0b-118">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="cba0b-119">Erstellen eines neuen [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cba0b-119">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="cba0b-120">RestrictedAppsViolation löschen</span><span class="sxs-lookup"><span data-stu-id="cba0b-120">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="cba0b-121">Keine</span><span class="sxs-lookup"><span data-stu-id="cba0b-121">None</span></span>|<span data-ttu-id="cba0b-122">Löscht eine [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="cba0b-122">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="cba0b-123">RestrictedAppsViolation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cba0b-123">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="cba0b-124">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="cba0b-124">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="cba0b-125">Aktualisieren der Eigenschaften eines [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cba0b-125">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cba0b-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cba0b-126">Properties</span></span>
|<span data-ttu-id="cba0b-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cba0b-127">Property</span></span>|<span data-ttu-id="cba0b-128">Typ</span><span class="sxs-lookup"><span data-stu-id="cba0b-128">Type</span></span>|<span data-ttu-id="cba0b-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cba0b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cba0b-130">id</span><span class="sxs-lookup"><span data-stu-id="cba0b-130">id</span></span>|<span data-ttu-id="cba0b-131">string</span><span class="sxs-lookup"><span data-stu-id="cba0b-131">String</span></span>|<span data-ttu-id="cba0b-132">Eindeutiger Bezeichner für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="cba0b-132">Unique identifier for the object.</span></span> <span data-ttu-id="cba0b-133">Zusammengesetzt aus "Account-ID", "Device", "Policies" und "userId"</span><span class="sxs-lookup"><span data-stu-id="cba0b-133">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="cba0b-134">userId</span><span class="sxs-lookup"><span data-stu-id="cba0b-134">userId</span></span>|<span data-ttu-id="cba0b-135">String</span><span class="sxs-lookup"><span data-stu-id="cba0b-135">String</span></span>|<span data-ttu-id="cba0b-136">Benutzer eindeutiger Bezeichner, muss GUID sein</span><span class="sxs-lookup"><span data-stu-id="cba0b-136">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="cba0b-137">userName</span><span class="sxs-lookup"><span data-stu-id="cba0b-137">userName</span></span>|<span data-ttu-id="cba0b-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cba0b-138">String</span></span>|<span data-ttu-id="cba0b-139">Benutzername</span><span class="sxs-lookup"><span data-stu-id="cba0b-139">User name</span></span>|
|<span data-ttu-id="cba0b-140">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="cba0b-140">managedDeviceId</span></span>|<span data-ttu-id="cba0b-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cba0b-141">String</span></span>|<span data-ttu-id="cba0b-142">Eindeutiger Bezeichner für verwaltetes Gerät, muss GUID sein</span><span class="sxs-lookup"><span data-stu-id="cba0b-142">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="cba0b-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="cba0b-143">deviceName</span></span>|<span data-ttu-id="cba0b-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cba0b-144">String</span></span>|<span data-ttu-id="cba0b-145">Gerätename</span><span class="sxs-lookup"><span data-stu-id="cba0b-145">Device name</span></span>|
|<span data-ttu-id="cba0b-146">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="cba0b-146">deviceConfigurationId</span></span>|<span data-ttu-id="cba0b-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cba0b-147">String</span></span>|<span data-ttu-id="cba0b-148">Device Configuration Profile Unique Identifier, must be GUID</span><span class="sxs-lookup"><span data-stu-id="cba0b-148">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="cba0b-149">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="cba0b-149">deviceConfigurationName</span></span>|<span data-ttu-id="cba0b-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cba0b-150">String</span></span>|<span data-ttu-id="cba0b-151">Name des Geräte Konfigurationsprofils</span><span class="sxs-lookup"><span data-stu-id="cba0b-151">Device configuration profile name</span></span>|
|<span data-ttu-id="cba0b-152">platformType</span><span class="sxs-lookup"><span data-stu-id="cba0b-152">platformType</span></span>|[<span data-ttu-id="cba0b-153">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="cba0b-153">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="cba0b-154">Plattformtyp.</span><span class="sxs-lookup"><span data-stu-id="cba0b-154">Platform type.</span></span> <span data-ttu-id="cba0b-155">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="cba0b-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="cba0b-156">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="cba0b-156">restrictedAppsState</span></span>|[<span data-ttu-id="cba0b-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="cba0b-157">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="cba0b-158">Eingeschränkter apps-Status.</span><span class="sxs-lookup"><span data-stu-id="cba0b-158">Restricted apps state.</span></span> <span data-ttu-id="cba0b-159">Mögliche Werte sind: `prohibitedApps` und `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="cba0b-159">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="cba0b-160">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="cba0b-160">restrictedApps</span></span>|<span data-ttu-id="cba0b-161">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="cba0b-161">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="cba0b-162">Liste der verletzten eingeschränkten apps</span><span class="sxs-lookup"><span data-stu-id="cba0b-162">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="cba0b-163">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cba0b-163">Relationships</span></span>
<span data-ttu-id="cba0b-164">Keine</span><span class="sxs-lookup"><span data-stu-id="cba0b-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cba0b-165">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cba0b-165">JSON Representation</span></span>
<span data-ttu-id="cba0b-166">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cba0b-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```




