---
title: deviceConfigurationAssignment-Ressourcentyp
description: Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a4a527f8b9da9f11d521311c54697fd04c4f019
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940911"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="2a0f8-103">deviceConfigurationAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2a0f8-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="2a0f8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2a0f8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a0f8-105">Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.</span><span class="sxs-lookup"><span data-stu-id="2a0f8-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="2a0f8-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="2a0f8-106">Methods</span></span>
|<span data-ttu-id="2a0f8-107">Methode</span><span class="sxs-lookup"><span data-stu-id="2a0f8-107">Method</span></span>|<span data-ttu-id="2a0f8-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2a0f8-108">Return Type</span></span>|<span data-ttu-id="2a0f8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a0f8-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2a0f8-110">deviceConfigurationAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="2a0f8-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="2a0f8-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2a0f8-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2a0f8-112">Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="2a0f8-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="2a0f8-113">deviceConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="2a0f8-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="2a0f8-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a0f8-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2a0f8-115">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a0f8-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2a0f8-116">deviceConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="2a0f8-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="2a0f8-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a0f8-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2a0f8-118">Erstellen eines neuen [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a0f8-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2a0f8-119">deviceConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="2a0f8-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="2a0f8-120">Keine</span><span class="sxs-lookup"><span data-stu-id="2a0f8-120">None</span></span>|<span data-ttu-id="2a0f8-121">Löscht ein [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2a0f8-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="2a0f8-122">deviceConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2a0f8-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="2a0f8-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a0f8-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2a0f8-124">Aktualisieren der Eigenschaften eines [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a0f8-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a0f8-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2a0f8-125">Properties</span></span>
|<span data-ttu-id="2a0f8-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a0f8-126">Property</span></span>|<span data-ttu-id="2a0f8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="2a0f8-127">Type</span></span>|<span data-ttu-id="2a0f8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a0f8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a0f8-129">id</span><span class="sxs-lookup"><span data-stu-id="2a0f8-129">id</span></span>|<span data-ttu-id="2a0f8-130">String</span><span class="sxs-lookup"><span data-stu-id="2a0f8-130">String</span></span>|<span data-ttu-id="2a0f8-131">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="2a0f8-131">The key of the assignment.</span></span>|
|<span data-ttu-id="2a0f8-132">target</span><span class="sxs-lookup"><span data-stu-id="2a0f8-132">target</span></span>|[<span data-ttu-id="2a0f8-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2a0f8-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2a0f8-134">Das Zuweisungsziel für die Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="2a0f8-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a0f8-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2a0f8-135">Relationships</span></span>
<span data-ttu-id="2a0f8-136">Keine</span><span class="sxs-lookup"><span data-stu-id="2a0f8-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a0f8-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2a0f8-137">JSON Representation</span></span>
<span data-ttu-id="2a0f8-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a0f8-138">Here is a JSON representation of the resource.</span></span>
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



