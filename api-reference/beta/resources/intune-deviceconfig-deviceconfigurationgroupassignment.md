---
title: Ressourcentyp deviceConfigurationGroupAssignment
description: Gerät Konfiguration Gruppe zuweisen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ed94f08fb33fe4a999e71b85808f58853d40cad4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406822"
---
# <a name="deviceconfigurationgroupassignment-resource-type"></a><span data-ttu-id="06ddc-103">Ressourcentyp deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="06ddc-103">deviceConfigurationGroupAssignment resource type</span></span>

> <span data-ttu-id="06ddc-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="06ddc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="06ddc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06ddc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06ddc-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06ddc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06ddc-107">Gerät Konfiguration Gruppe zuweisen.</span><span class="sxs-lookup"><span data-stu-id="06ddc-107">Device configuration group assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="06ddc-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="06ddc-108">Methods</span></span>
|<span data-ttu-id="06ddc-109">Methode</span><span class="sxs-lookup"><span data-stu-id="06ddc-109">Method</span></span>|<span data-ttu-id="06ddc-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="06ddc-110">Return Type</span></span>|<span data-ttu-id="06ddc-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06ddc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06ddc-112">Liste deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="06ddc-112">List deviceConfigurationGroupAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-list.md)|<span data-ttu-id="06ddc-113">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="06ddc-113">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="06ddc-114">Listeneigenschaften und Beziehungen der [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="06ddc-114">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="06ddc-115">Abrufen von deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="06ddc-115">Get deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-get.md)|[<span data-ttu-id="06ddc-116">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="06ddc-116">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="06ddc-117">Lesen Sie Eigenschaften und Beziehungen des [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="06ddc-117">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="06ddc-118">Erstellen von deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="06ddc-118">Create deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-create.md)|[<span data-ttu-id="06ddc-119">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="06ddc-119">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="06ddc-120">Erstellen eines neuen [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="06ddc-120">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="06ddc-121">DeviceConfigurationGroupAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="06ddc-121">Delete deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-delete.md)|<span data-ttu-id="06ddc-122">Keine</span><span class="sxs-lookup"><span data-stu-id="06ddc-122">None</span></span>|<span data-ttu-id="06ddc-123">Löscht eine [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06ddc-123">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>|
|[<span data-ttu-id="06ddc-124">DeviceConfigurationGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="06ddc-124">Update deviceConfigurationGroupAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationgroupassignment-update.md)|[<span data-ttu-id="06ddc-125">deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="06ddc-125">deviceConfigurationGroupAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|<span data-ttu-id="06ddc-126">Aktualisieren Sie die Eigenschaften eines [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="06ddc-126">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06ddc-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06ddc-127">Properties</span></span>
|<span data-ttu-id="06ddc-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06ddc-128">Property</span></span>|<span data-ttu-id="06ddc-129">Typ</span><span class="sxs-lookup"><span data-stu-id="06ddc-129">Type</span></span>|<span data-ttu-id="06ddc-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06ddc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06ddc-131">id</span><span class="sxs-lookup"><span data-stu-id="06ddc-131">id</span></span>|<span data-ttu-id="06ddc-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06ddc-132">String</span></span>|<span data-ttu-id="06ddc-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="06ddc-133">Key of the entity.</span></span>|
|<span data-ttu-id="06ddc-134">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="06ddc-134">targetGroupId</span></span>|<span data-ttu-id="06ddc-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06ddc-135">String</span></span>|<span data-ttu-id="06ddc-136">Die Id der Gruppe AAD sind wir Gerätekonfiguration zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="06ddc-136">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="06ddc-137">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="06ddc-137">excludeGroup</span></span>|<span data-ttu-id="06ddc-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="06ddc-138">Boolean</span></span>|<span data-ttu-id="06ddc-139">Gibt an, ob diese Gruppe ist ausgeschlossen werden soll.</span><span class="sxs-lookup"><span data-stu-id="06ddc-139">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="06ddc-140">Die Standardeinstellungen, dass die Gruppe eingeschlossen werden sollen</span><span class="sxs-lookup"><span data-stu-id="06ddc-140">Defaults that the group should be included</span></span>|

## <a name="relationships"></a><span data-ttu-id="06ddc-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="06ddc-141">Relationships</span></span>
|<span data-ttu-id="06ddc-142">Beziehung</span><span class="sxs-lookup"><span data-stu-id="06ddc-142">Relationship</span></span>|<span data-ttu-id="06ddc-143">Typ</span><span class="sxs-lookup"><span data-stu-id="06ddc-143">Type</span></span>|<span data-ttu-id="06ddc-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06ddc-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06ddc-145">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="06ddc-145">deviceConfiguration</span></span>|[<span data-ttu-id="06ddc-146">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="06ddc-146">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="06ddc-147">Der Navigationslink zur Gerätekonfiguration geplant wird.</span><span class="sxs-lookup"><span data-stu-id="06ddc-147">The navigation link to the Device Configuration being targeted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06ddc-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06ddc-148">JSON Representation</span></span>
<span data-ttu-id="06ddc-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06ddc-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String",
  "excludeGroup": true
}
```




