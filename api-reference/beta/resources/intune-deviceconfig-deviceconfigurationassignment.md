---
title: deviceConfigurationAssignment-Ressourcentyp
description: Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.
ms.openlocfilehash: 447f02252eaa5b894d1cbe27f68242acf6b09a35
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061594"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="f3ea4-103">deviceConfigurationAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f3ea4-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="f3ea4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3ea4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3ea4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3ea4-107">Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="f3ea4-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="f3ea4-108">Methods</span></span>
|<span data-ttu-id="f3ea4-109">Methode</span><span class="sxs-lookup"><span data-stu-id="f3ea4-109">Method</span></span>|<span data-ttu-id="f3ea4-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f3ea4-110">Return Type</span></span>|<span data-ttu-id="f3ea4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3ea4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3ea4-112">deviceConfigurationAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="f3ea4-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="f3ea4-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f3ea4-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f3ea4-114">Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="f3ea4-115">deviceConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="f3ea4-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="f3ea4-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f3ea4-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="f3ea4-117">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="f3ea4-118">deviceConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="f3ea4-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="f3ea4-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f3ea4-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="f3ea4-120">Erstellen eines neuen [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="f3ea4-121">deviceConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="f3ea4-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="f3ea4-122">Keine</span><span class="sxs-lookup"><span data-stu-id="f3ea4-122">None</span></span>|<span data-ttu-id="f3ea4-123">Löscht ein [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="f3ea4-124">deviceConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f3ea4-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="f3ea4-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f3ea4-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="f3ea4-126">Aktualisieren der Eigenschaften eines [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3ea4-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f3ea4-127">Properties</span></span>
|<span data-ttu-id="f3ea4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f3ea4-128">Property</span></span>|<span data-ttu-id="f3ea4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="f3ea4-129">Type</span></span>|<span data-ttu-id="f3ea4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3ea4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3ea4-131">id</span><span class="sxs-lookup"><span data-stu-id="f3ea4-131">id</span></span>|<span data-ttu-id="f3ea4-132">String</span><span class="sxs-lookup"><span data-stu-id="f3ea4-132">String</span></span>|<span data-ttu-id="f3ea4-133">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="f3ea4-133">The key of the assignment.</span></span>|
|<span data-ttu-id="f3ea4-134">target</span><span class="sxs-lookup"><span data-stu-id="f3ea4-134">target</span></span>|[<span data-ttu-id="f3ea4-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f3ea4-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f3ea4-136">Das Zuweisungsziel für die Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3ea4-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f3ea4-137">Relationships</span></span>
<span data-ttu-id="f3ea4-138">Keine</span><span class="sxs-lookup"><span data-stu-id="f3ea4-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f3ea4-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f3ea4-139">JSON Representation</span></span>
<span data-ttu-id="f3ea4-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f3ea4-140">Here is a JSON representation of the resource.</span></span>
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





