---
title: detectedApp-Ressourcentyp
description: Eine verwaltete oder nicht verwaltete App, die auf einem verwalteten Gerät installiert ist. Nicht verwaltete Apps werden nur für als unternehmenseigen gekennzeichnete Geräte angezeigt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cba801689cb5051926a3139574d5a27294090a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403098"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="38aa8-104">detectedApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="38aa8-104">detectedApp resource type</span></span>

> <span data-ttu-id="38aa8-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="38aa8-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38aa8-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="38aa8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38aa8-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38aa8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38aa8-108">Eine verwaltete oder nicht verwaltete App, die auf einem verwalteten Gerät installiert ist.</span><span class="sxs-lookup"><span data-stu-id="38aa8-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="38aa8-109">Nicht verwaltete Apps werden nur für als unternehmenseigen gekennzeichnete Geräte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="38aa8-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="38aa8-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="38aa8-110">Methods</span></span>
|<span data-ttu-id="38aa8-111">Methode</span><span class="sxs-lookup"><span data-stu-id="38aa8-111">Method</span></span>|<span data-ttu-id="38aa8-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="38aa8-112">Return Type</span></span>|<span data-ttu-id="38aa8-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38aa8-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="38aa8-114">detectedApps auflisten</span><span class="sxs-lookup"><span data-stu-id="38aa8-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="38aa8-115">[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="38aa8-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="38aa8-116">Auflisten von Eigenschaften und Beziehungen der [detectedApp](../resources/intune-devices-detectedapp.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="38aa8-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="38aa8-117">detectedApp abrufen</span><span class="sxs-lookup"><span data-stu-id="38aa8-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="38aa8-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="38aa8-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="38aa8-119">Auflisten von Eigenschaften und Beziehungen des [detectedApp](../resources/intune-devices-detectedapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="38aa8-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="38aa8-120">detectedApp erstellen</span><span class="sxs-lookup"><span data-stu-id="38aa8-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="38aa8-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="38aa8-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="38aa8-122">Erstellen eines neuen [detectedApp](../resources/intune-devices-detectedapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="38aa8-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="38aa8-123">detectedApp löschen</span><span class="sxs-lookup"><span data-stu-id="38aa8-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="38aa8-124">Keine</span><span class="sxs-lookup"><span data-stu-id="38aa8-124">None</span></span>|<span data-ttu-id="38aa8-125">Löscht ein [detectedApp](../resources/intune-devices-detectedapp.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="38aa8-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="38aa8-126">detectedApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="38aa8-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="38aa8-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="38aa8-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="38aa8-128">Aktualisieren der Eigenschaften eines [detectedApp](../resources/intune-devices-detectedapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="38aa8-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="38aa8-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="38aa8-129">Properties</span></span>
|<span data-ttu-id="38aa8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38aa8-130">Property</span></span>|<span data-ttu-id="38aa8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="38aa8-131">Type</span></span>|<span data-ttu-id="38aa8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38aa8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38aa8-133">id</span><span class="sxs-lookup"><span data-stu-id="38aa8-133">id</span></span>|<span data-ttu-id="38aa8-134">String</span><span class="sxs-lookup"><span data-stu-id="38aa8-134">String</span></span>|<span data-ttu-id="38aa8-135">Eindeutiger Bezeichner für die erkannte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="38aa8-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="38aa8-136">Dieser wird automatisch von Intune generiert, wenn die Anwendung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="38aa8-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="38aa8-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="38aa8-137">Read-only.</span></span>|
|<span data-ttu-id="38aa8-138">displayName</span><span class="sxs-lookup"><span data-stu-id="38aa8-138">displayName</span></span>|<span data-ttu-id="38aa8-139">String</span><span class="sxs-lookup"><span data-stu-id="38aa8-139">String</span></span>|<span data-ttu-id="38aa8-140">Name der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="38aa8-140">Name of the discovered application.</span></span> <span data-ttu-id="38aa8-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="38aa8-141">Read-only</span></span>|
|<span data-ttu-id="38aa8-142">version</span><span class="sxs-lookup"><span data-stu-id="38aa8-142">version</span></span>|<span data-ttu-id="38aa8-143">String</span><span class="sxs-lookup"><span data-stu-id="38aa8-143">String</span></span>|<span data-ttu-id="38aa8-144">Version der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="38aa8-144">Version of the discovered application.</span></span> <span data-ttu-id="38aa8-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="38aa8-145">Read-only</span></span>|
|<span data-ttu-id="38aa8-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="38aa8-146">sizeInByte</span></span>|<span data-ttu-id="38aa8-147">Int64</span><span class="sxs-lookup"><span data-stu-id="38aa8-147">Int64</span></span>|<span data-ttu-id="38aa8-148">Größe der ermittelten Anwendung in Byte.</span><span class="sxs-lookup"><span data-stu-id="38aa8-148">Discovered application size in bytes.</span></span> <span data-ttu-id="38aa8-149">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="38aa8-149">Read-only</span></span>|
|<span data-ttu-id="38aa8-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="38aa8-150">deviceCount</span></span>|<span data-ttu-id="38aa8-151">Int32</span><span class="sxs-lookup"><span data-stu-id="38aa8-151">Int32</span></span>|<span data-ttu-id="38aa8-152">Die Anzahl von Geräten, auf denen diese Anwendung installiert ist.</span><span class="sxs-lookup"><span data-stu-id="38aa8-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="38aa8-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="38aa8-153">Relationships</span></span>
|<span data-ttu-id="38aa8-154">Beziehung</span><span class="sxs-lookup"><span data-stu-id="38aa8-154">Relationship</span></span>|<span data-ttu-id="38aa8-155">Typ</span><span class="sxs-lookup"><span data-stu-id="38aa8-155">Type</span></span>|<span data-ttu-id="38aa8-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38aa8-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38aa8-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="38aa8-157">managedDevices</span></span>|<span data-ttu-id="38aa8-158">[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="38aa8-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="38aa8-159">Die Geräte, auf denen die ermittelte Anwendung installiert ist.</span><span class="sxs-lookup"><span data-stu-id="38aa8-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38aa8-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="38aa8-160">JSON Representation</span></span>
<span data-ttu-id="38aa8-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="38aa8-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```




