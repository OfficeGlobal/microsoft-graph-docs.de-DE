---
title: deviceConfigurationAssignment-Ressourcentyp
description: Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.
author: tfitzmac
ms.openlocfilehash: 26afc67312ab8544b395b5e20b89a01558fc75d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306244"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="25795-103">deviceConfigurationAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="25795-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="25795-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="25795-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25795-105">Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.</span><span class="sxs-lookup"><span data-stu-id="25795-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="25795-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="25795-106">Methods</span></span>
|<span data-ttu-id="25795-107">Methode</span><span class="sxs-lookup"><span data-stu-id="25795-107">Method</span></span>|<span data-ttu-id="25795-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="25795-108">Return Type</span></span>|<span data-ttu-id="25795-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25795-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="25795-110">deviceConfigurationAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="25795-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="25795-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="25795-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="25795-112">Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="25795-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="25795-113">deviceConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="25795-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="25795-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="25795-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="25795-115">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="25795-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="25795-116">deviceConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="25795-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="25795-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="25795-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="25795-118">Erstellen eines neuen [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="25795-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="25795-119">deviceConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="25795-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="25795-120">Keine</span><span class="sxs-lookup"><span data-stu-id="25795-120">None</span></span>|<span data-ttu-id="25795-121">Löscht ein [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="25795-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="25795-122">deviceConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="25795-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="25795-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="25795-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="25795-124">Aktualisieren der Eigenschaften eines [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="25795-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="25795-125">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="25795-125">Properties</span></span>
|<span data-ttu-id="25795-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="25795-126">Property</span></span>|<span data-ttu-id="25795-127">Typ</span><span class="sxs-lookup"><span data-stu-id="25795-127">Type</span></span>|<span data-ttu-id="25795-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25795-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25795-129">id</span><span class="sxs-lookup"><span data-stu-id="25795-129">id</span></span>|<span data-ttu-id="25795-130">String</span><span class="sxs-lookup"><span data-stu-id="25795-130">String</span></span>|<span data-ttu-id="25795-131">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="25795-131">The key of the assignment.</span></span>|
|<span data-ttu-id="25795-132">target</span><span class="sxs-lookup"><span data-stu-id="25795-132">target</span></span>|[<span data-ttu-id="25795-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="25795-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="25795-134">Das Zuweisungsziel für die Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="25795-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25795-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="25795-135">Relationships</span></span>
<span data-ttu-id="25795-136">Keine</span><span class="sxs-lookup"><span data-stu-id="25795-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="25795-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="25795-137">JSON Representation</span></span>
<span data-ttu-id="25795-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="25795-138">Here is a JSON representation of the resource.</span></span>
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



