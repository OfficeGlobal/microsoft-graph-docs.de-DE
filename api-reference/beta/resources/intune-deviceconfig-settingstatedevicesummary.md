---
title: settingStateDeviceSummary-Ressourcentyp
description: Zusammenfassung des Zustands der Gerätekonformitätsrichtlinien und -konfigurations-Einstellung
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2104998cfdd65659114b1850d3cfcf1392bf9642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925875"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="1c7a3-103">settingStateDeviceSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1c7a3-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="1c7a3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1c7a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c7a3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1c7a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c7a3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1c7a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c7a3-107">Zusammenfassung des Zustands der Gerätekonformitätsrichtlinien und -konfigurations-Einstellung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>
## <a name="methods"></a><span data-ttu-id="1c7a3-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="1c7a3-108">Methods</span></span>
|<span data-ttu-id="1c7a3-109">Methode</span><span class="sxs-lookup"><span data-stu-id="1c7a3-109">Method</span></span>|<span data-ttu-id="1c7a3-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1c7a3-110">Return Type</span></span>|<span data-ttu-id="1c7a3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1c7a3-112">settingStateDeviceSummaries auflisten</span><span class="sxs-lookup"><span data-stu-id="1c7a3-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="1c7a3-113"> [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="1c7a3-114">Auflisten von Eigenschaften und Beziehungen der [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="1c7a3-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="1c7a3-115">settingStateDeviceSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="1c7a3-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="1c7a3-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1c7a3-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="1c7a3-117">Lesen von Eigenschaften und Beziehungen des [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1c7a3-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="1c7a3-118">settingStateDeviceSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="1c7a3-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="1c7a3-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1c7a3-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="1c7a3-120">Erstellen eines neuen [SettingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1c7a3-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="1c7a3-121">settingStateDeviceSummary löschen</span><span class="sxs-lookup"><span data-stu-id="1c7a3-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="1c7a3-122">Keine</span><span class="sxs-lookup"><span data-stu-id="1c7a3-122">None</span></span>|<span data-ttu-id="1c7a3-123">Löscht eine [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1c7a3-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="1c7a3-124">settingStateDeviceSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1c7a3-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="1c7a3-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1c7a3-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="1c7a3-126">Aktualisieren der Eigenschaften eines [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1c7a3-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1c7a3-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1c7a3-127">Properties</span></span>
|<span data-ttu-id="1c7a3-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c7a3-128">Property</span></span>|<span data-ttu-id="1c7a3-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1c7a3-129">Type</span></span>|<span data-ttu-id="1c7a3-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c7a3-131">id</span><span class="sxs-lookup"><span data-stu-id="1c7a3-131">id</span></span>|<span data-ttu-id="1c7a3-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1c7a3-132">String</span></span>|<span data-ttu-id="1c7a3-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1c7a3-133">Key of the entity.</span></span>|
|<span data-ttu-id="1c7a3-134">settingName</span><span class="sxs-lookup"><span data-stu-id="1c7a3-134">settingName</span></span>|<span data-ttu-id="1c7a3-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1c7a3-135">String</span></span>|<span data-ttu-id="1c7a3-136">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-136">Name of the setting</span></span>|
|<span data-ttu-id="1c7a3-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="1c7a3-137">instancePath</span></span>|<span data-ttu-id="1c7a3-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1c7a3-138">String</span></span>|<span data-ttu-id="1c7a3-139">Name des zur Einstellung gehörenden Objekts des Typs „InstancePath“</span><span class="sxs-lookup"><span data-stu-id="1c7a3-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="1c7a3-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c7a3-140">unknownDeviceCount</span></span>|<span data-ttu-id="1c7a3-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1c7a3-141">Int32</span></span>|<span data-ttu-id="1c7a3-142">Anzahl der Geräte mit Meldung „Unknown“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="1c7a3-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c7a3-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="1c7a3-144">Int32</span><span class="sxs-lookup"><span data-stu-id="1c7a3-144">Int32</span></span>|<span data-ttu-id="1c7a3-145">Anzahl der Geräte mit Meldung „Not Applicable“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="1c7a3-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c7a3-146">compliantDeviceCount</span></span>|<span data-ttu-id="1c7a3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1c7a3-147">Int32</span></span>|<span data-ttu-id="1c7a3-148">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="1c7a3-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c7a3-149">remediatedDeviceCount</span></span>|<span data-ttu-id="1c7a3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1c7a3-150">Int32</span></span>|<span data-ttu-id="1c7a3-151">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="1c7a3-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c7a3-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="1c7a3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1c7a3-153">Int32</span></span>|<span data-ttu-id="1c7a3-154">Anzahl der Geräte mit Meldung „NonCompliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="1c7a3-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c7a3-155">errorDeviceCount</span></span>|<span data-ttu-id="1c7a3-156">Int32</span><span class="sxs-lookup"><span data-stu-id="1c7a3-156">Int32</span></span>|<span data-ttu-id="1c7a3-157">Anzahl der Geräte mit Meldung „Error“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-157">Device error count for the setting</span></span>|
|<span data-ttu-id="1c7a3-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1c7a3-158">conflictDeviceCount</span></span>|<span data-ttu-id="1c7a3-159">Int32</span><span class="sxs-lookup"><span data-stu-id="1c7a3-159">Int32</span></span>|<span data-ttu-id="1c7a3-160">Anzahl der Geräte mit Konfliktfehler für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c7a3-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1c7a3-161">Relationships</span></span>
<span data-ttu-id="1c7a3-162">Keine</span><span class="sxs-lookup"><span data-stu-id="1c7a3-162">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1c7a3-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1c7a3-163">JSON Representation</span></span>
<span data-ttu-id="1c7a3-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1c7a3-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





