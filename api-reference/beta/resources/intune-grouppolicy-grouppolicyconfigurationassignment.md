---
title: groupPolicyConfigurationAssignment-Ressourcentyp
description: Die Gruppenrichtlinien-Konfigurations Zuweisungs Entität weist einer bestimmten Gruppenrichtlinienkonfiguration eine oder mehrere AAD-Gruppen zu.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d928ff8d65eaf2fb766e579828e2ec7d9b56f05
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160837"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="b0f02-103">groupPolicyConfigurationAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b0f02-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="b0f02-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b0f02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0f02-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b0f02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0f02-106">Die Gruppenrichtlinien-Konfigurations Zuweisungs Entität weist einer bestimmten Gruppenrichtlinienkonfiguration eine oder mehrere AAD-Gruppen zu.</span><span class="sxs-lookup"><span data-stu-id="b0f02-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="b0f02-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="b0f02-107">Methods</span></span>
|<span data-ttu-id="b0f02-108">Methode</span><span class="sxs-lookup"><span data-stu-id="b0f02-108">Method</span></span>|<span data-ttu-id="b0f02-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b0f02-109">Return Type</span></span>|<span data-ttu-id="b0f02-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0f02-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0f02-111">GroupPolicyConfigurationAssignments aufListen</span><span class="sxs-lookup"><span data-stu-id="b0f02-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="b0f02-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="b0f02-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b0f02-113">AufListen von Eigenschaften und Beziehungen der [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b0f02-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="b0f02-114">GroupPolicyConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="b0f02-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="b0f02-115">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f02-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="b0f02-116">Lesen von Eigenschaften und Beziehungen des [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b0f02-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="b0f02-117">GroupPolicyConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="b0f02-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="b0f02-118">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f02-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="b0f02-119">Erstellen eines neuen [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b0f02-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="b0f02-120">GroupPolicyConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="b0f02-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="b0f02-121">Keine</span><span class="sxs-lookup"><span data-stu-id="b0f02-121">None</span></span>|<span data-ttu-id="b0f02-122">Löscht eine [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b0f02-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="b0f02-123">GroupPolicyConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b0f02-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="b0f02-124">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b0f02-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="b0f02-125">Aktualisieren der Eigenschaften eines [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b0f02-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0f02-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b0f02-126">Properties</span></span>
|<span data-ttu-id="b0f02-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b0f02-127">Property</span></span>|<span data-ttu-id="b0f02-128">Typ</span><span class="sxs-lookup"><span data-stu-id="b0f02-128">Type</span></span>|<span data-ttu-id="b0f02-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0f02-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0f02-130">id</span><span class="sxs-lookup"><span data-stu-id="b0f02-130">id</span></span>|<span data-ttu-id="b0f02-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0f02-131">String</span></span>|<span data-ttu-id="b0f02-132">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b0f02-132">Key of the entity.</span></span>|
|<span data-ttu-id="b0f02-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0f02-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b0f02-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0f02-134">DateTimeOffset</span></span>|<span data-ttu-id="b0f02-135">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="b0f02-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="b0f02-136">target</span><span class="sxs-lookup"><span data-stu-id="b0f02-136">target</span></span>|[<span data-ttu-id="b0f02-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b0f02-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b0f02-138">Der Typ der Gruppen, die für die Gruppenrichtlinienkonfiguration vorgesehen sind.</span><span class="sxs-lookup"><span data-stu-id="b0f02-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0f02-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b0f02-139">Relationships</span></span>
<span data-ttu-id="b0f02-140">Keine</span><span class="sxs-lookup"><span data-stu-id="b0f02-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0f02-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b0f02-141">JSON Representation</span></span>
<span data-ttu-id="b0f02-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b0f02-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




