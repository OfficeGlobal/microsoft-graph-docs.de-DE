---
title: importedDeviceIdentity-Ressourcentyp
description: Die importedDeviceIdentity-Ressource stellt eine eindeutige Hardware Identität eines Geräts dar, das für die Konfiguration vor der Registrierung vorab bereitgestellt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f5dcc3d7ef6cb59bffe1d7b8cfda958e76c3e35
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572103"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="44ea8-103">importedDeviceIdentity-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="44ea8-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="44ea8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44ea8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44ea8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="44ea8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44ea8-106">Die importedDeviceIdentity-Ressource stellt eine eindeutige Hardware Identität eines Geräts dar, das für die Konfiguration vor der Registrierung vorab bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="44ea8-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="44ea8-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="44ea8-107">Methods</span></span>
|<span data-ttu-id="44ea8-108">Methode</span><span class="sxs-lookup"><span data-stu-id="44ea8-108">Method</span></span>|<span data-ttu-id="44ea8-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="44ea8-109">Return Type</span></span>|<span data-ttu-id="44ea8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44ea8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="44ea8-111">ImportedDeviceIdentities aufListen</span><span class="sxs-lookup"><span data-stu-id="44ea8-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="44ea8-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="44ea8-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="44ea8-113">AufListen von Eigenschaften und Beziehungen der [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="44ea8-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="44ea8-114">ImportedDeviceIdentity abrufen</span><span class="sxs-lookup"><span data-stu-id="44ea8-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="44ea8-115">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="44ea8-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="44ea8-116">Lesen von Eigenschaften und Beziehungen des [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="44ea8-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="44ea8-117">ImportedDeviceIdentity erstellen</span><span class="sxs-lookup"><span data-stu-id="44ea8-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="44ea8-118">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="44ea8-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="44ea8-119">Erstellen eines neuen [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="44ea8-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="44ea8-120">ImportedDeviceIdentity löschen</span><span class="sxs-lookup"><span data-stu-id="44ea8-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="44ea8-121">None</span><span class="sxs-lookup"><span data-stu-id="44ea8-121">None</span></span>|<span data-ttu-id="44ea8-122">Löscht eine [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="44ea8-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="44ea8-123">ImportedDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="44ea8-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="44ea8-124">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="44ea8-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="44ea8-125">Aktualisieren der Eigenschaften eines [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="44ea8-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="44ea8-126">importDeviceIdentityList-Aktion</span><span class="sxs-lookup"><span data-stu-id="44ea8-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="44ea8-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="44ea8-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="44ea8-128">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="44ea8-128">Not yet documented</span></span>|
|[<span data-ttu-id="44ea8-129">searchExistingIdentities-Aktion</span><span class="sxs-lookup"><span data-stu-id="44ea8-129">searchExistingIdentities action</span></span>](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|<span data-ttu-id="44ea8-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="44ea8-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="44ea8-131">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="44ea8-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="44ea8-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="44ea8-132">Properties</span></span>
|<span data-ttu-id="44ea8-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="44ea8-133">Property</span></span>|<span data-ttu-id="44ea8-134">Typ</span><span class="sxs-lookup"><span data-stu-id="44ea8-134">Type</span></span>|<span data-ttu-id="44ea8-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44ea8-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ea8-136">id</span><span class="sxs-lookup"><span data-stu-id="44ea8-136">id</span></span>|<span data-ttu-id="44ea8-137">String</span><span class="sxs-lookup"><span data-stu-id="44ea8-137">String</span></span>|<span data-ttu-id="44ea8-138">ID der importierten Geräte Identität</span><span class="sxs-lookup"><span data-stu-id="44ea8-138">Id of the imported device identity</span></span>|
|<span data-ttu-id="44ea8-139">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="44ea8-139">importedDeviceIdentifier</span></span>|<span data-ttu-id="44ea8-140">String</span><span class="sxs-lookup"><span data-stu-id="44ea8-140">String</span></span>|<span data-ttu-id="44ea8-141">Importierter Gerätebezeichner</span><span class="sxs-lookup"><span data-stu-id="44ea8-141">Imported Device Identifier</span></span>|
|<span data-ttu-id="44ea8-142">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="44ea8-142">importedDeviceIdentityType</span></span>|[<span data-ttu-id="44ea8-143">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="44ea8-143">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="44ea8-144">Typ der importierten Geräte Identität.</span><span class="sxs-lookup"><span data-stu-id="44ea8-144">Type of Imported Device Identity.</span></span> <span data-ttu-id="44ea8-145">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="44ea8-145">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="44ea8-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44ea8-146">lastModifiedDateTime</span></span>|<span data-ttu-id="44ea8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44ea8-147">DateTimeOffset</span></span>|<span data-ttu-id="44ea8-148">Datum der letzten Änderung der Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44ea8-148">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="44ea8-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44ea8-149">createdDateTime</span></span>|<span data-ttu-id="44ea8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44ea8-150">DateTimeOffset</span></span>|<span data-ttu-id="44ea8-151">ErstellungsDatum des Geräts</span><span class="sxs-lookup"><span data-stu-id="44ea8-151">Created Date Time of the device</span></span>|
|<span data-ttu-id="44ea8-152">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="44ea8-152">lastContactedDateTime</span></span>|<span data-ttu-id="44ea8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44ea8-153">DateTimeOffset</span></span>|<span data-ttu-id="44ea8-154">Datum der letzten Kontaktaufnahme des Geräts</span><span class="sxs-lookup"><span data-stu-id="44ea8-154">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="44ea8-155">description</span><span class="sxs-lookup"><span data-stu-id="44ea8-155">description</span></span>|<span data-ttu-id="44ea8-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="44ea8-156">String</span></span>|<span data-ttu-id="44ea8-157">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="44ea8-157">The description of the device</span></span>|
|<span data-ttu-id="44ea8-158">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="44ea8-158">enrollmentState</span></span>|[<span data-ttu-id="44ea8-159">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="44ea8-159">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="44ea8-160">Der Status des Geräts in InTune.</span><span class="sxs-lookup"><span data-stu-id="44ea8-160">The state of the device in Intune.</span></span> <span data-ttu-id="44ea8-161">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="44ea8-161">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="44ea8-162">Plattform</span><span class="sxs-lookup"><span data-stu-id="44ea8-162">platform</span></span>|[<span data-ttu-id="44ea8-163">Plattform</span><span class="sxs-lookup"><span data-stu-id="44ea8-163">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="44ea8-164">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="44ea8-164">The platform of the Device.</span></span> <span data-ttu-id="44ea8-165">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="44ea8-165">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44ea8-166">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="44ea8-166">Relationships</span></span>
<span data-ttu-id="44ea8-167">Keine</span><span class="sxs-lookup"><span data-stu-id="44ea8-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44ea8-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="44ea8-168">JSON Representation</span></span>
<span data-ttu-id="44ea8-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="44ea8-169">Here is a JSON representation of the resource.</span></span>
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




