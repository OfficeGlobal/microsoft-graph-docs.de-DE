---
title: deviceConfigurationAssignment-Ressourcentyp
description: Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60fb4f0a782d9502f9e3da3f0a7da2389e937a7d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251426"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="87cd5-103">deviceConfigurationAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="87cd5-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="87cd5-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="87cd5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87cd5-105">Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.</span><span class="sxs-lookup"><span data-stu-id="87cd5-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="87cd5-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="87cd5-106">Methods</span></span>
|<span data-ttu-id="87cd5-107">Methode</span><span class="sxs-lookup"><span data-stu-id="87cd5-107">Method</span></span>|<span data-ttu-id="87cd5-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="87cd5-108">Return Type</span></span>|<span data-ttu-id="87cd5-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87cd5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87cd5-110">deviceConfigurationAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="87cd5-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="87cd5-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="87cd5-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="87cd5-112">Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="87cd5-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="87cd5-113">deviceConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="87cd5-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="87cd5-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="87cd5-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="87cd5-115">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="87cd5-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="87cd5-116">deviceConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="87cd5-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="87cd5-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="87cd5-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="87cd5-118">Erstellen eines neuen [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="87cd5-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="87cd5-119">deviceConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="87cd5-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="87cd5-120">Keine</span><span class="sxs-lookup"><span data-stu-id="87cd5-120">None</span></span>|<span data-ttu-id="87cd5-121">Löscht ein [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="87cd5-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="87cd5-122">deviceConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="87cd5-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="87cd5-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="87cd5-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="87cd5-124">Aktualisieren der Eigenschaften eines [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="87cd5-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="87cd5-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="87cd5-125">Properties</span></span>
|<span data-ttu-id="87cd5-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87cd5-126">Property</span></span>|<span data-ttu-id="87cd5-127">Typ</span><span class="sxs-lookup"><span data-stu-id="87cd5-127">Type</span></span>|<span data-ttu-id="87cd5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87cd5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87cd5-129">id</span><span class="sxs-lookup"><span data-stu-id="87cd5-129">id</span></span>|<span data-ttu-id="87cd5-130">String</span><span class="sxs-lookup"><span data-stu-id="87cd5-130">String</span></span>|<span data-ttu-id="87cd5-131">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="87cd5-131">The key of the assignment.</span></span>|
|<span data-ttu-id="87cd5-132">target</span><span class="sxs-lookup"><span data-stu-id="87cd5-132">target</span></span>|[<span data-ttu-id="87cd5-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="87cd5-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="87cd5-134">Das Zuweisungsziel für die Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="87cd5-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87cd5-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="87cd5-135">Relationships</span></span>
<span data-ttu-id="87cd5-136">Keine</span><span class="sxs-lookup"><span data-stu-id="87cd5-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87cd5-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="87cd5-137">JSON Representation</span></span>
<span data-ttu-id="87cd5-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="87cd5-138">Here is a JSON representation of the resource.</span></span>
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



