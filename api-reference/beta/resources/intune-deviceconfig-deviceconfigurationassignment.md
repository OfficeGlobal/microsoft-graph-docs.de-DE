---
title: deviceConfigurationAssignment-Ressourcentyp
description: Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80645a7b6724a71620eeebf4dfb4ba8a1b440db2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172632"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="8dc3d-103">deviceConfigurationAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8dc3d-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="8dc3d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8dc3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dc3d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8dc3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dc3d-106">Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.</span><span class="sxs-lookup"><span data-stu-id="8dc3d-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="8dc3d-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="8dc3d-107">Methods</span></span>
|<span data-ttu-id="8dc3d-108">Methode</span><span class="sxs-lookup"><span data-stu-id="8dc3d-108">Method</span></span>|<span data-ttu-id="8dc3d-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8dc3d-109">Return Type</span></span>|<span data-ttu-id="8dc3d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dc3d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8dc3d-111">deviceConfigurationAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="8dc3d-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="8dc3d-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8dc3d-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8dc3d-113">Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="8dc3d-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="8dc3d-114">deviceConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="8dc3d-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="8dc3d-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8dc3d-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8dc3d-116">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8dc3d-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="8dc3d-117">deviceConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="8dc3d-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="8dc3d-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8dc3d-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8dc3d-119">Erstellen eines neuen [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8dc3d-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="8dc3d-120">deviceConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="8dc3d-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="8dc3d-121">Keine</span><span class="sxs-lookup"><span data-stu-id="8dc3d-121">None</span></span>|<span data-ttu-id="8dc3d-122">Löscht ein [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="8dc3d-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="8dc3d-123">deviceConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8dc3d-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="8dc3d-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8dc3d-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="8dc3d-125">Aktualisieren der Eigenschaften eines [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8dc3d-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8dc3d-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8dc3d-126">Properties</span></span>
|<span data-ttu-id="8dc3d-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8dc3d-127">Property</span></span>|<span data-ttu-id="8dc3d-128">Typ</span><span class="sxs-lookup"><span data-stu-id="8dc3d-128">Type</span></span>|<span data-ttu-id="8dc3d-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dc3d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dc3d-130">id</span><span class="sxs-lookup"><span data-stu-id="8dc3d-130">id</span></span>|<span data-ttu-id="8dc3d-131">String</span><span class="sxs-lookup"><span data-stu-id="8dc3d-131">String</span></span>|<span data-ttu-id="8dc3d-132">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="8dc3d-132">The key of the assignment.</span></span>|
|<span data-ttu-id="8dc3d-133">target</span><span class="sxs-lookup"><span data-stu-id="8dc3d-133">target</span></span>|[<span data-ttu-id="8dc3d-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8dc3d-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8dc3d-135">Das Zuweisungsziel für die Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8dc3d-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dc3d-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8dc3d-136">Relationships</span></span>
<span data-ttu-id="8dc3d-137">Keine</span><span class="sxs-lookup"><span data-stu-id="8dc3d-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8dc3d-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8dc3d-138">JSON Representation</span></span>
<span data-ttu-id="8dc3d-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8dc3d-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




