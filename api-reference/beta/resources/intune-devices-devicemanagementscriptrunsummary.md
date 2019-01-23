---
title: Ressourcentyp deviceManagementScriptRunSummary
description: Enthält Eigenschaften für die Laufzeit Zusammenfassung für ein Gerät Management-Skript.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f49e08c0f6351133b953e566ba8e89afe945e990
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423853"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="55bcc-103">Ressourcentyp deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="55bcc-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="55bcc-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="55bcc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="55bcc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="55bcc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55bcc-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="55bcc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55bcc-107">Enthält Eigenschaften für die Laufzeit Zusammenfassung für ein Gerät Management-Skript.</span><span class="sxs-lookup"><span data-stu-id="55bcc-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="55bcc-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="55bcc-108">Methods</span></span>
|<span data-ttu-id="55bcc-109">Methode</span><span class="sxs-lookup"><span data-stu-id="55bcc-109">Method</span></span>|<span data-ttu-id="55bcc-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="55bcc-110">Return Type</span></span>|<span data-ttu-id="55bcc-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55bcc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55bcc-112">Abrufen von deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="55bcc-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="55bcc-113">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="55bcc-113">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="55bcc-114">Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="55bcc-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="55bcc-115">DeviceManagementScriptRunSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="55bcc-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="55bcc-116">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="55bcc-116">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="55bcc-117">Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="55bcc-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="55bcc-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="55bcc-118">Properties</span></span>
|<span data-ttu-id="55bcc-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="55bcc-119">Property</span></span>|<span data-ttu-id="55bcc-120">Typ</span><span class="sxs-lookup"><span data-stu-id="55bcc-120">Type</span></span>|<span data-ttu-id="55bcc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55bcc-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55bcc-122">id</span><span class="sxs-lookup"><span data-stu-id="55bcc-122">id</span></span>|<span data-ttu-id="55bcc-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="55bcc-123">String</span></span>|<span data-ttu-id="55bcc-124">Das Gerät Management-Skript ausführen Zusammenfassung Entität-Taste.</span><span class="sxs-lookup"><span data-stu-id="55bcc-124">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="55bcc-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55bcc-125">successDeviceCount</span></span>|<span data-ttu-id="55bcc-126">Int32</span><span class="sxs-lookup"><span data-stu-id="55bcc-126">Int32</span></span>|<span data-ttu-id="55bcc-127">Anzahl der Geräte Erfolg.</span><span class="sxs-lookup"><span data-stu-id="55bcc-127">Success device count.</span></span>|
|<span data-ttu-id="55bcc-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55bcc-128">errorDeviceCount</span></span>|<span data-ttu-id="55bcc-129">Int32</span><span class="sxs-lookup"><span data-stu-id="55bcc-129">Int32</span></span>|<span data-ttu-id="55bcc-130">Anzahl der Fehler Geräte.</span><span class="sxs-lookup"><span data-stu-id="55bcc-130">Error device count.</span></span>|
|<span data-ttu-id="55bcc-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="55bcc-131">successUserCount</span></span>|<span data-ttu-id="55bcc-132">Int32</span><span class="sxs-lookup"><span data-stu-id="55bcc-132">Int32</span></span>|<span data-ttu-id="55bcc-133">Benutzeranzahl Erfolg.</span><span class="sxs-lookup"><span data-stu-id="55bcc-133">Success user count.</span></span>|
|<span data-ttu-id="55bcc-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="55bcc-134">errorUserCount</span></span>|<span data-ttu-id="55bcc-135">Int32</span><span class="sxs-lookup"><span data-stu-id="55bcc-135">Int32</span></span>|<span data-ttu-id="55bcc-136">Anzahl der Fehler Benutzer.</span><span class="sxs-lookup"><span data-stu-id="55bcc-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55bcc-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="55bcc-137">Relationships</span></span>
<span data-ttu-id="55bcc-138">Keine</span><span class="sxs-lookup"><span data-stu-id="55bcc-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55bcc-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="55bcc-139">JSON Representation</span></span>
<span data-ttu-id="55bcc-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="55bcc-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```




