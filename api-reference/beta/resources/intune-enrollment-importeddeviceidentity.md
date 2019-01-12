---
title: Ressourcentyp importedDeviceIdentity
description: Die Ressource ImportedDeviceIdentity stellt eine eindeutige Hardware Identität eines Geräts für die Konfiguration der Registrierung vor dem bereits bereitgestellt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fe03159f79bb1198db80cbba130601614df8865
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966566"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="eaeb3-103">Ressourcentyp importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eaeb3-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="eaeb3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaeb3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eaeb3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eaeb3-107">Die Ressource ImportedDeviceIdentity stellt eine eindeutige Hardware Identität eines Geräts für die Konfiguration der Registrierung vor dem bereits bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="eaeb3-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="eaeb3-108">Methods</span></span>
|<span data-ttu-id="eaeb3-109">Methode</span><span class="sxs-lookup"><span data-stu-id="eaeb3-109">Method</span></span>|<span data-ttu-id="eaeb3-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="eaeb3-110">Return Type</span></span>|<span data-ttu-id="eaeb3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eaeb3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eaeb3-112">Liste importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="eaeb3-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="eaeb3-113">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="eaeb3-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="eaeb3-114">Listeneigenschaften und Beziehungen der [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="eaeb3-115">Abrufen von importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eaeb3-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="eaeb3-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eaeb3-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="eaeb3-117">Lesen Sie Eigenschaften und Beziehungen des [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="eaeb3-118">Erstellen von importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eaeb3-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="eaeb3-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eaeb3-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="eaeb3-120">Erstellen eines neuen [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="eaeb3-121">ImportedDeviceIdentity löschen</span><span class="sxs-lookup"><span data-stu-id="eaeb3-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="eaeb3-122">Keine</span><span class="sxs-lookup"><span data-stu-id="eaeb3-122">None</span></span>|<span data-ttu-id="eaeb3-123">Löscht eine [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="eaeb3-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="eaeb3-124">ImportedDeviceIdentity aktualisieren</span><span class="sxs-lookup"><span data-stu-id="eaeb3-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="eaeb3-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="eaeb3-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="eaeb3-126">Aktualisieren Sie die Eigenschaften eines [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="eaeb3-127">ImportDeviceIdentityList Aktion</span><span class="sxs-lookup"><span data-stu-id="eaeb3-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="eaeb3-128">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="eaeb3-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="eaeb3-129">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="eaeb3-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="eaeb3-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eaeb3-130">Properties</span></span>
|<span data-ttu-id="eaeb3-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eaeb3-131">Property</span></span>|<span data-ttu-id="eaeb3-132">Typ</span><span class="sxs-lookup"><span data-stu-id="eaeb3-132">Type</span></span>|<span data-ttu-id="eaeb3-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eaeb3-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaeb3-134">id</span><span class="sxs-lookup"><span data-stu-id="eaeb3-134">id</span></span>|<span data-ttu-id="eaeb3-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eaeb3-135">String</span></span>|<span data-ttu-id="eaeb3-136">ID der Identität des importierten Geräts</span><span class="sxs-lookup"><span data-stu-id="eaeb3-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="eaeb3-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="eaeb3-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="eaeb3-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eaeb3-138">String</span></span>|<span data-ttu-id="eaeb3-139">Importierte Geräte-ID</span><span class="sxs-lookup"><span data-stu-id="eaeb3-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="eaeb3-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="eaeb3-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="eaeb3-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="eaeb3-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="eaeb3-142">Art der importierten Gerät Identität.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="eaeb3-143">Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="eaeb3-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaeb3-144">lastModifiedDateTime</span></span>|<span data-ttu-id="eaeb3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaeb3-145">DateTimeOffset</span></span>|<span data-ttu-id="eaeb3-146">Letzte Änderung DateTime der Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eaeb3-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="eaeb3-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eaeb3-147">createdDateTime</span></span>|<span data-ttu-id="eaeb3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaeb3-148">DateTimeOffset</span></span>|<span data-ttu-id="eaeb3-149">Erstellte Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="eaeb3-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="eaeb3-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaeb3-150">lastContactedDateTime</span></span>|<span data-ttu-id="eaeb3-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaeb3-151">DateTimeOffset</span></span>|<span data-ttu-id="eaeb3-152">Letzte kontaktiert Datum-Uhrzeit des Geräts</span><span class="sxs-lookup"><span data-stu-id="eaeb3-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="eaeb3-153">description</span><span class="sxs-lookup"><span data-stu-id="eaeb3-153">description</span></span>|<span data-ttu-id="eaeb3-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eaeb3-154">String</span></span>|<span data-ttu-id="eaeb3-155">Die Beschreibung des Geräts</span><span class="sxs-lookup"><span data-stu-id="eaeb3-155">The description of the device</span></span>|
|<span data-ttu-id="eaeb3-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="eaeb3-156">enrollmentState</span></span>|[<span data-ttu-id="eaeb3-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="eaeb3-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="eaeb3-158">Der Zustand des Geräts in Intune.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-158">The state of the device in Intune.</span></span> <span data-ttu-id="eaeb3-159">Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="eaeb3-160">Plattform</span><span class="sxs-lookup"><span data-stu-id="eaeb3-160">platform</span></span>|[<span data-ttu-id="eaeb3-161">Plattform</span><span class="sxs-lookup"><span data-stu-id="eaeb3-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="eaeb3-162">Die Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-162">The platform of the Device.</span></span> <span data-ttu-id="eaeb3-163">Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaeb3-164">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="eaeb3-164">Relationships</span></span>
<span data-ttu-id="eaeb3-165">Keine</span><span class="sxs-lookup"><span data-stu-id="eaeb3-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eaeb3-166">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eaeb3-166">JSON Representation</span></span>
<span data-ttu-id="eaeb3-167">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eaeb3-167">Here is a JSON representation of the resource.</span></span>
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





