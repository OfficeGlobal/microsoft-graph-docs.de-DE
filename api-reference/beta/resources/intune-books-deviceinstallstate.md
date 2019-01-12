---
title: deviceInstallState-Ressourcentyp
description: Enthält Eigenschaften für den Installationsstatus für ein Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1b495bc41590ada44a9986dd9cc9cb262bcc68b6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959888"
---
# <a name="deviceinstallstate-resource-type"></a><span data-ttu-id="dfe14-103">deviceInstallState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dfe14-103">deviceInstallState resource type</span></span>

> <span data-ttu-id="dfe14-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dfe14-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfe14-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dfe14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfe14-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dfe14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfe14-107">Enthält Eigenschaften für den Installationsstatus für ein Gerät.</span><span class="sxs-lookup"><span data-stu-id="dfe14-107">Contains properties for the installation state for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="dfe14-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="dfe14-108">Methods</span></span>
|<span data-ttu-id="dfe14-109">Methode</span><span class="sxs-lookup"><span data-stu-id="dfe14-109">Method</span></span>|<span data-ttu-id="dfe14-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="dfe14-110">Return Type</span></span>|<span data-ttu-id="dfe14-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dfe14-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dfe14-112">deviceInstallStates auflisten</span><span class="sxs-lookup"><span data-stu-id="dfe14-112">List deviceInstallStates</span></span>](../api/intune-books-deviceinstallstate-list.md)|<span data-ttu-id="dfe14-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="dfe14-113">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="dfe14-114">Auflisten von Eigenschaften und Beziehungen der [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="dfe14-114">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>|
|[<span data-ttu-id="dfe14-115">deviceInstallState abrufen</span><span class="sxs-lookup"><span data-stu-id="dfe14-115">Get deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-get.md)|[<span data-ttu-id="dfe14-116">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dfe14-116">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="dfe14-117">Lesen von Eigenschaften und Beziehungen des [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dfe14-117">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="dfe14-118">deviceInstallState erstellen</span><span class="sxs-lookup"><span data-stu-id="dfe14-118">Create deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-create.md)|[<span data-ttu-id="dfe14-119">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dfe14-119">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="dfe14-120">Erstellen eines neuen [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dfe14-120">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|
|[<span data-ttu-id="dfe14-121">deviceInstallState löschen</span><span class="sxs-lookup"><span data-stu-id="dfe14-121">Delete deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-delete.md)|<span data-ttu-id="dfe14-122">Keine</span><span class="sxs-lookup"><span data-stu-id="dfe14-122">None</span></span>|<span data-ttu-id="dfe14-123">Löscht ein [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="dfe14-123">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>|
|[<span data-ttu-id="dfe14-124">deviceInstallState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="dfe14-124">Update deviceInstallState</span></span>](../api/intune-books-deviceinstallstate-update.md)|[<span data-ttu-id="dfe14-125">deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="dfe14-125">deviceInstallState</span></span>](../resources/intune-books-deviceinstallstate.md)|<span data-ttu-id="dfe14-126">Aktualisieren der Eigenschaften eines [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dfe14-126">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dfe14-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dfe14-127">Properties</span></span>
|<span data-ttu-id="dfe14-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dfe14-128">Property</span></span>|<span data-ttu-id="dfe14-129">Typ</span><span class="sxs-lookup"><span data-stu-id="dfe14-129">Type</span></span>|<span data-ttu-id="dfe14-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dfe14-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfe14-131">id</span><span class="sxs-lookup"><span data-stu-id="dfe14-131">id</span></span>|<span data-ttu-id="dfe14-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfe14-132">String</span></span>|<span data-ttu-id="dfe14-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dfe14-133">Key of the entity.</span></span>|
|<span data-ttu-id="dfe14-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="dfe14-134">deviceName</span></span>|<span data-ttu-id="dfe14-135">String</span><span class="sxs-lookup"><span data-stu-id="dfe14-135">String</span></span>|<span data-ttu-id="dfe14-136">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="dfe14-136">Device name.</span></span>|
|<span data-ttu-id="dfe14-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="dfe14-137">deviceId</span></span>|<span data-ttu-id="dfe14-138">String</span><span class="sxs-lookup"><span data-stu-id="dfe14-138">String</span></span>|<span data-ttu-id="dfe14-139">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="dfe14-139">Device Id.</span></span>|
|<span data-ttu-id="dfe14-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="dfe14-140">lastSyncDateTime</span></span>|<span data-ttu-id="dfe14-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfe14-141">DateTimeOffset</span></span>|<span data-ttu-id="dfe14-142">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="dfe14-142">Last sync date and time.</span></span>|
|<span data-ttu-id="dfe14-143">installState</span><span class="sxs-lookup"><span data-stu-id="dfe14-143">installState</span></span>|[<span data-ttu-id="dfe14-144">installState</span><span class="sxs-lookup"><span data-stu-id="dfe14-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="dfe14-145">Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="dfe14-145">The install state of the eBook.</span></span> <span data-ttu-id="dfe14-146">Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="dfe14-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="dfe14-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="dfe14-147">errorCode</span></span>|<span data-ttu-id="dfe14-148">String</span><span class="sxs-lookup"><span data-stu-id="dfe14-148">String</span></span>|<span data-ttu-id="dfe14-149">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="dfe14-149">The error code for install failures.</span></span>|
|<span data-ttu-id="dfe14-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="dfe14-150">osVersion</span></span>|<span data-ttu-id="dfe14-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfe14-151">String</span></span>|<span data-ttu-id="dfe14-152">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="dfe14-152">OS Version.</span></span>|
|<span data-ttu-id="dfe14-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="dfe14-153">osDescription</span></span>|<span data-ttu-id="dfe14-154">String</span><span class="sxs-lookup"><span data-stu-id="dfe14-154">String</span></span>|<span data-ttu-id="dfe14-155">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="dfe14-155">OS Description.</span></span>|
|<span data-ttu-id="dfe14-156">userName</span><span class="sxs-lookup"><span data-stu-id="dfe14-156">userName</span></span>|<span data-ttu-id="dfe14-157">String</span><span class="sxs-lookup"><span data-stu-id="dfe14-157">String</span></span>|<span data-ttu-id="dfe14-158">Benutzername des Geräts</span><span class="sxs-lookup"><span data-stu-id="dfe14-158">Device User Name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfe14-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dfe14-159">Relationships</span></span>
<span data-ttu-id="dfe14-160">Keine</span><span class="sxs-lookup"><span data-stu-id="dfe14-160">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dfe14-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dfe14-161">JSON Representation</span></span>
<span data-ttu-id="dfe14-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dfe14-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```





