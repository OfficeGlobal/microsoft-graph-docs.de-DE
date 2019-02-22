---
title: deviceManagementScriptRunSummary-Ressourcentyp
description: Enthält Eigenschaften für die Ausführungs Zusammenfassung eines Geräteverwaltungsskripts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3fe26fc121d0d1d9339de999101975d2c4c225a5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174270"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="e9360-103">deviceManagementScriptRunSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e9360-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="e9360-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e9360-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9360-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e9360-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9360-106">Enthält Eigenschaften für die Ausführungs Zusammenfassung eines Geräteverwaltungsskripts.</span><span class="sxs-lookup"><span data-stu-id="e9360-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="e9360-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="e9360-107">Methods</span></span>
|<span data-ttu-id="e9360-108">Methode</span><span class="sxs-lookup"><span data-stu-id="e9360-108">Method</span></span>|<span data-ttu-id="e9360-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e9360-109">Return Type</span></span>|<span data-ttu-id="e9360-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9360-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e9360-111">DeviceManagementScriptRunSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="e9360-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="e9360-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e9360-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="e9360-113">Lesen von Eigenschaften und Beziehungen des [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e9360-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="e9360-114">DeviceManagementScriptRunSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e9360-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="e9360-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e9360-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="e9360-116">Aktualisieren der Eigenschaften eines [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e9360-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e9360-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e9360-117">Properties</span></span>
|<span data-ttu-id="e9360-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9360-118">Property</span></span>|<span data-ttu-id="e9360-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e9360-119">Type</span></span>|<span data-ttu-id="e9360-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9360-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9360-121">id</span><span class="sxs-lookup"><span data-stu-id="e9360-121">id</span></span>|<span data-ttu-id="e9360-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e9360-122">String</span></span>|<span data-ttu-id="e9360-123">Der Schlüssel der Device Management-Skript Ausführungs Zusammenfassungs Entität.</span><span class="sxs-lookup"><span data-stu-id="e9360-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="e9360-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e9360-124">successDeviceCount</span></span>|<span data-ttu-id="e9360-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e9360-125">Int32</span></span>|<span data-ttu-id="e9360-126">Anzahl der erfolgreichen Geräte.</span><span class="sxs-lookup"><span data-stu-id="e9360-126">Success device count.</span></span>|
|<span data-ttu-id="e9360-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e9360-127">errorDeviceCount</span></span>|<span data-ttu-id="e9360-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e9360-128">Int32</span></span>|<span data-ttu-id="e9360-129">Fehlergeräte Anzahl.</span><span class="sxs-lookup"><span data-stu-id="e9360-129">Error device count.</span></span>|
|<span data-ttu-id="e9360-130">successUserCount</span><span class="sxs-lookup"><span data-stu-id="e9360-130">successUserCount</span></span>|<span data-ttu-id="e9360-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e9360-131">Int32</span></span>|<span data-ttu-id="e9360-132">Anzahl der erfolgreichen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="e9360-132">Success user count.</span></span>|
|<span data-ttu-id="e9360-133">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="e9360-133">errorUserCount</span></span>|<span data-ttu-id="e9360-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e9360-134">Int32</span></span>|<span data-ttu-id="e9360-135">Fehler Benutzeranzahl.</span><span class="sxs-lookup"><span data-stu-id="e9360-135">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9360-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e9360-136">Relationships</span></span>
<span data-ttu-id="e9360-137">Keine</span><span class="sxs-lookup"><span data-stu-id="e9360-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9360-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e9360-138">JSON Representation</span></span>
<span data-ttu-id="e9360-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e9360-139">Here is a JSON representation of the resource.</span></span>
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




