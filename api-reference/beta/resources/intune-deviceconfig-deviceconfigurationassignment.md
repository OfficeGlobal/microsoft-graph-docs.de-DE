---
title: deviceConfigurationAssignment-Ressourcentyp
description: Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.
author: tfitzmac
ms.openlocfilehash: ef5a9156b98eb8915471dbc042f6e028542be768
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343295"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="91b66-103">deviceConfigurationAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="91b66-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="91b66-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91b66-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91b66-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91b66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91b66-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="91b66-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91b66-107">Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.</span><span class="sxs-lookup"><span data-stu-id="91b66-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="91b66-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="91b66-108">Methods</span></span>
|<span data-ttu-id="91b66-109">Methode</span><span class="sxs-lookup"><span data-stu-id="91b66-109">Method</span></span>|<span data-ttu-id="91b66-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="91b66-110">Return Type</span></span>|<span data-ttu-id="91b66-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91b66-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91b66-112">deviceConfigurationAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="91b66-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="91b66-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="91b66-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="91b66-114">Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="91b66-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="91b66-115">deviceConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="91b66-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="91b66-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="91b66-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="91b66-117">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="91b66-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="91b66-118">deviceConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="91b66-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="91b66-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="91b66-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="91b66-120">Erstellen eines neuen [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="91b66-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="91b66-121">deviceConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="91b66-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="91b66-122">Keine</span><span class="sxs-lookup"><span data-stu-id="91b66-122">None</span></span>|<span data-ttu-id="91b66-123">Löscht ein [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="91b66-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="91b66-124">deviceConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="91b66-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="91b66-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="91b66-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="91b66-126">Aktualisieren der Eigenschaften eines [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="91b66-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="91b66-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91b66-127">Properties</span></span>
|<span data-ttu-id="91b66-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91b66-128">Property</span></span>|<span data-ttu-id="91b66-129">Typ</span><span class="sxs-lookup"><span data-stu-id="91b66-129">Type</span></span>|<span data-ttu-id="91b66-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91b66-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91b66-131">id</span><span class="sxs-lookup"><span data-stu-id="91b66-131">id</span></span>|<span data-ttu-id="91b66-132">String</span><span class="sxs-lookup"><span data-stu-id="91b66-132">String</span></span>|<span data-ttu-id="91b66-133">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="91b66-133">The key of the assignment.</span></span>|
|<span data-ttu-id="91b66-134">target</span><span class="sxs-lookup"><span data-stu-id="91b66-134">target</span></span>|[<span data-ttu-id="91b66-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="91b66-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="91b66-136">Das Zuweisungsziel für die Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="91b66-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91b66-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="91b66-137">Relationships</span></span>
<span data-ttu-id="91b66-138">Keine</span><span class="sxs-lookup"><span data-stu-id="91b66-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91b66-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91b66-139">JSON Representation</span></span>
<span data-ttu-id="91b66-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91b66-140">Here is a JSON representation of the resource.</span></span>
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





