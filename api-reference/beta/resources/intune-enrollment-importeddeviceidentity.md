---
title: importedDeviceIdentity-Ressourcentyp
description: Die importedDeviceIdentity-Ressource stellt eine eindeutige Hardware Identität eines Geräts dar, das für die Konfiguration vor der Registrierung vorab bereitgestellt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7ef77b550060d5544a6ee0eda4e6b11923d3571
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151226"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="6799b-103">importedDeviceIdentity-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6799b-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="6799b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6799b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6799b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6799b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6799b-106">Die importedDeviceIdentity-Ressource stellt eine eindeutige Hardware Identität eines Geräts dar, das für die Konfiguration vor der Registrierung vorab bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="6799b-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="6799b-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="6799b-107">Methods</span></span>
|<span data-ttu-id="6799b-108">Methode</span><span class="sxs-lookup"><span data-stu-id="6799b-108">Method</span></span>|<span data-ttu-id="6799b-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6799b-109">Return Type</span></span>|<span data-ttu-id="6799b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6799b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6799b-111">ImportedDeviceIdentities aufListen</span><span class="sxs-lookup"><span data-stu-id="6799b-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="6799b-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="6799b-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="6799b-113">AufListen von Eigenschaften und Beziehungen der [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="6799b-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="6799b-114">ImportedDeviceIdentity abrufen</span><span class="sxs-lookup"><span data-stu-id="6799b-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="6799b-115">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="6799b-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="6799b-116">Lesen von Eigenschaften und Beziehungen des [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6799b-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="6799b-117">ImportedDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="6799b-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="6799b-118">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="6799b-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="6799b-119">Erstellen eines neuen [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6799b-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="6799b-120">ImportedDeviceIdentity löschen</span><span class="sxs-lookup"><span data-stu-id="6799b-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="6799b-121">Keine</span><span class="sxs-lookup"><span data-stu-id="6799b-121">None</span></span>|<span data-ttu-id="6799b-122">Löscht eine [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="6799b-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="6799b-123">ImportedDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6799b-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="6799b-124">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="6799b-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="6799b-125">Aktualisieren der Eigenschaften eines [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6799b-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="6799b-126">importDeviceIdentityList-Aktion</span><span class="sxs-lookup"><span data-stu-id="6799b-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="6799b-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="6799b-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="6799b-128">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6799b-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6799b-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6799b-129">Properties</span></span>
|<span data-ttu-id="6799b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6799b-130">Property</span></span>|<span data-ttu-id="6799b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6799b-131">Type</span></span>|<span data-ttu-id="6799b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6799b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6799b-133">id</span><span class="sxs-lookup"><span data-stu-id="6799b-133">id</span></span>|<span data-ttu-id="6799b-134">string</span><span class="sxs-lookup"><span data-stu-id="6799b-134">String</span></span>|<span data-ttu-id="6799b-135">ID der importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="6799b-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="6799b-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6799b-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="6799b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6799b-137">String</span></span>|<span data-ttu-id="6799b-138">Importierter Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="6799b-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="6799b-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="6799b-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="6799b-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="6799b-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="6799b-141">Typ der importierten Geräte Identität.</span><span class="sxs-lookup"><span data-stu-id="6799b-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="6799b-142">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="6799b-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="6799b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6799b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6799b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6799b-144">DateTimeOffset</span></span>|<span data-ttu-id="6799b-145">Datum der letzten Änderung der Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6799b-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="6799b-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6799b-146">createdDateTime</span></span>|<span data-ttu-id="6799b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6799b-147">DateTimeOffset</span></span>|<span data-ttu-id="6799b-148">ErstellungsDatum des Geräts</span><span class="sxs-lookup"><span data-stu-id="6799b-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="6799b-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="6799b-149">lastContactedDateTime</span></span>|<span data-ttu-id="6799b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6799b-150">DateTimeOffset</span></span>|<span data-ttu-id="6799b-151">Datum der letzten Kontaktaufnahme des Geräts</span><span class="sxs-lookup"><span data-stu-id="6799b-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="6799b-152">description</span><span class="sxs-lookup"><span data-stu-id="6799b-152">description</span></span>|<span data-ttu-id="6799b-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6799b-153">String</span></span>|<span data-ttu-id="6799b-154">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="6799b-154">The description of the device</span></span>|
|<span data-ttu-id="6799b-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="6799b-155">enrollmentState</span></span>|[<span data-ttu-id="6799b-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="6799b-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="6799b-157">Der Status des Geräts in InTune.</span><span class="sxs-lookup"><span data-stu-id="6799b-157">The state of the device in Intune.</span></span> <span data-ttu-id="6799b-158">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="6799b-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="6799b-159">Plattform</span><span class="sxs-lookup"><span data-stu-id="6799b-159">platform</span></span>|[<span data-ttu-id="6799b-160">Plattform</span><span class="sxs-lookup"><span data-stu-id="6799b-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="6799b-161">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="6799b-161">The platform of the Device.</span></span> <span data-ttu-id="6799b-162">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="6799b-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6799b-163">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6799b-163">Relationships</span></span>
<span data-ttu-id="6799b-164">Keine</span><span class="sxs-lookup"><span data-stu-id="6799b-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6799b-165">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6799b-165">JSON Representation</span></span>
<span data-ttu-id="6799b-166">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6799b-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




