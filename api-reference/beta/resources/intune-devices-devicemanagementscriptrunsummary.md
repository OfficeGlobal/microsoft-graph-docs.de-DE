---
title: Ressourcentyp deviceManagementScriptRunSummary
description: Enthält Eigenschaften für die Laufzeit Zusammenfassung für ein Gerät Management-Skript.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9676fc7f6792c3bd9771ab7ed1ccbeaa67826d3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962037"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="731ad-103">Ressourcentyp deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="731ad-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="731ad-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="731ad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="731ad-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="731ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="731ad-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="731ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="731ad-107">Enthält Eigenschaften für die Laufzeit Zusammenfassung für ein Gerät Management-Skript.</span><span class="sxs-lookup"><span data-stu-id="731ad-107">Contains properties for the run summary of a device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="731ad-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="731ad-108">Methods</span></span>
|<span data-ttu-id="731ad-109">Methode</span><span class="sxs-lookup"><span data-stu-id="731ad-109">Method</span></span>|<span data-ttu-id="731ad-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="731ad-110">Return Type</span></span>|<span data-ttu-id="731ad-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="731ad-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="731ad-112">Abrufen von deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="731ad-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="731ad-113">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="731ad-113">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="731ad-114">Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="731ad-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="731ad-115">DeviceManagementScriptRunSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="731ad-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="731ad-116">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="731ad-116">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="731ad-117">Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="731ad-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="731ad-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="731ad-118">Properties</span></span>
|<span data-ttu-id="731ad-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="731ad-119">Property</span></span>|<span data-ttu-id="731ad-120">Typ</span><span class="sxs-lookup"><span data-stu-id="731ad-120">Type</span></span>|<span data-ttu-id="731ad-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="731ad-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="731ad-122">id</span><span class="sxs-lookup"><span data-stu-id="731ad-122">id</span></span>|<span data-ttu-id="731ad-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="731ad-123">String</span></span>|<span data-ttu-id="731ad-124">Das Gerät Management-Skript ausführen Zusammenfassung Entität-Taste.</span><span class="sxs-lookup"><span data-stu-id="731ad-124">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="731ad-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="731ad-125">successDeviceCount</span></span>|<span data-ttu-id="731ad-126">Int32</span><span class="sxs-lookup"><span data-stu-id="731ad-126">Int32</span></span>|<span data-ttu-id="731ad-127">Anzahl der Geräte Erfolg.</span><span class="sxs-lookup"><span data-stu-id="731ad-127">Success device count.</span></span>|
|<span data-ttu-id="731ad-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="731ad-128">errorDeviceCount</span></span>|<span data-ttu-id="731ad-129">Int32</span><span class="sxs-lookup"><span data-stu-id="731ad-129">Int32</span></span>|<span data-ttu-id="731ad-130">Anzahl der Fehler Geräte.</span><span class="sxs-lookup"><span data-stu-id="731ad-130">Error device count.</span></span>|
|<span data-ttu-id="731ad-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="731ad-131">successUserCount</span></span>|<span data-ttu-id="731ad-132">Int32</span><span class="sxs-lookup"><span data-stu-id="731ad-132">Int32</span></span>|<span data-ttu-id="731ad-133">Benutzeranzahl Erfolg.</span><span class="sxs-lookup"><span data-stu-id="731ad-133">Success user count.</span></span>|
|<span data-ttu-id="731ad-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="731ad-134">errorUserCount</span></span>|<span data-ttu-id="731ad-135">Int32</span><span class="sxs-lookup"><span data-stu-id="731ad-135">Int32</span></span>|<span data-ttu-id="731ad-136">Anzahl der Fehler Benutzer.</span><span class="sxs-lookup"><span data-stu-id="731ad-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="731ad-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="731ad-137">Relationships</span></span>
<span data-ttu-id="731ad-138">Keine</span><span class="sxs-lookup"><span data-stu-id="731ad-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="731ad-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="731ad-139">JSON Representation</span></span>
<span data-ttu-id="731ad-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="731ad-140">Here is a JSON representation of the resource.</span></span>
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





