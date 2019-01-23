---
title: deviceConfigurationAssignment-Ressourcentyp
description: Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 115cbd779e53f303bdbf95dc28916879726676ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402601"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="803bf-103">deviceConfigurationAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="803bf-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="803bf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="803bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="803bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="803bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="803bf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="803bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="803bf-107">Die Zuweisungsentität für die Gerätekonfiguration weist eine AAD-Gruppe einer bestimmten Gerätekonfiguration zu.</span><span class="sxs-lookup"><span data-stu-id="803bf-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="803bf-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="803bf-108">Methods</span></span>
|<span data-ttu-id="803bf-109">Methode</span><span class="sxs-lookup"><span data-stu-id="803bf-109">Method</span></span>|<span data-ttu-id="803bf-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="803bf-110">Return Type</span></span>|<span data-ttu-id="803bf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="803bf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="803bf-112">deviceConfigurationAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="803bf-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="803bf-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="803bf-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="803bf-114">Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="803bf-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="803bf-115">deviceConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="803bf-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="803bf-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="803bf-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="803bf-117">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="803bf-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="803bf-118">deviceConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="803bf-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="803bf-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="803bf-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="803bf-120">Erstellen eines neuen [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="803bf-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="803bf-121">deviceConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="803bf-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="803bf-122">Keine</span><span class="sxs-lookup"><span data-stu-id="803bf-122">None</span></span>|<span data-ttu-id="803bf-123">Löscht ein [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="803bf-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="803bf-124">deviceConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="803bf-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="803bf-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="803bf-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="803bf-126">Aktualisieren der Eigenschaften eines [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="803bf-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="803bf-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="803bf-127">Properties</span></span>
|<span data-ttu-id="803bf-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="803bf-128">Property</span></span>|<span data-ttu-id="803bf-129">Typ</span><span class="sxs-lookup"><span data-stu-id="803bf-129">Type</span></span>|<span data-ttu-id="803bf-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="803bf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="803bf-131">id</span><span class="sxs-lookup"><span data-stu-id="803bf-131">id</span></span>|<span data-ttu-id="803bf-132">String</span><span class="sxs-lookup"><span data-stu-id="803bf-132">String</span></span>|<span data-ttu-id="803bf-133">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="803bf-133">The key of the assignment.</span></span>|
|<span data-ttu-id="803bf-134">target</span><span class="sxs-lookup"><span data-stu-id="803bf-134">target</span></span>|[<span data-ttu-id="803bf-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="803bf-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="803bf-136">Das Zuweisungsziel für die Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="803bf-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="803bf-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="803bf-137">Relationships</span></span>
<span data-ttu-id="803bf-138">Keine</span><span class="sxs-lookup"><span data-stu-id="803bf-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="803bf-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="803bf-139">JSON Representation</span></span>
<span data-ttu-id="803bf-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="803bf-140">Here is a JSON representation of the resource.</span></span>
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




