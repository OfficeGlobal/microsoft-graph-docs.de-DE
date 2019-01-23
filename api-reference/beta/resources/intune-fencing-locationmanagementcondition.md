---
title: Ressourcentyp locationManagementCondition
description: Enthält Informationen zum Definieren einer Speicherort Management Bedingung ein Interessenbereich zum Überwachen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c2eddf43696bd9300cc8dcd3408dbcd6fc5a9e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422796"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="9c128-103">Ressourcentyp locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="9c128-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="9c128-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9c128-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9c128-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9c128-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c128-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9c128-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c128-107">Enthält Informationen zum Definieren einer Speicherort Management Bedingung ein Interessenbereich zum Überwachen.</span><span class="sxs-lookup"><span data-stu-id="9c128-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="9c128-108">Erbt vom [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9c128-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9c128-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="9c128-109">Methods</span></span>
|<span data-ttu-id="9c128-110">Methode</span><span class="sxs-lookup"><span data-stu-id="9c128-110">Method</span></span>|<span data-ttu-id="9c128-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9c128-111">Return Type</span></span>|<span data-ttu-id="9c128-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c128-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9c128-113">Liste locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="9c128-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="9c128-114">[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9c128-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="9c128-115">Listeneigenschaften und Beziehungen der [LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9c128-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="9c128-116">Abrufen von locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="9c128-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="9c128-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="9c128-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="9c128-118">Lesen Sie Eigenschaften und Beziehungen des [LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9c128-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c128-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9c128-119">Properties</span></span>
|<span data-ttu-id="9c128-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c128-120">Property</span></span>|<span data-ttu-id="9c128-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9c128-121">Type</span></span>|<span data-ttu-id="9c128-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c128-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c128-123">id</span><span class="sxs-lookup"><span data-stu-id="9c128-123">id</span></span>|<span data-ttu-id="9c128-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c128-124">String</span></span>|<span data-ttu-id="9c128-125">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="9c128-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="9c128-126">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="9c128-126">System generated value assigned when created.</span></span> <span data-ttu-id="9c128-127">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9c128-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c128-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="9c128-128">uniqueName</span></span>|<span data-ttu-id="9c128-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c128-129">String</span></span>|<span data-ttu-id="9c128-130">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="9c128-130">Unique name for the management condition.</span></span> <span data-ttu-id="9c128-131">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="9c128-131">Used in management condition expressions.</span></span> <span data-ttu-id="9c128-132">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9c128-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c128-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9c128-133">displayName</span></span>|<span data-ttu-id="9c128-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c128-134">String</span></span>|<span data-ttu-id="9c128-135">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="9c128-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="9c128-136">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9c128-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c128-137">description</span><span class="sxs-lookup"><span data-stu-id="9c128-137">description</span></span>|<span data-ttu-id="9c128-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c128-138">String</span></span>|<span data-ttu-id="9c128-139">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="9c128-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="9c128-140">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9c128-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c128-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c128-141">createdDateTime</span></span>|<span data-ttu-id="9c128-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c128-142">DateTimeOffset</span></span>|<span data-ttu-id="9c128-143">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="9c128-143">The time the management condition was created.</span></span> <span data-ttu-id="9c128-144">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="9c128-144">Generated service side.</span></span> <span data-ttu-id="9c128-145">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9c128-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c128-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c128-146">modifiedDateTime</span></span>|<span data-ttu-id="9c128-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c128-147">DateTimeOffset</span></span>|<span data-ttu-id="9c128-148">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="9c128-148">The time the management condition was last modified.</span></span> <span data-ttu-id="9c128-149">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="9c128-149">Updated service side.</span></span> <span data-ttu-id="9c128-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9c128-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c128-151">eTag</span><span class="sxs-lookup"><span data-stu-id="9c128-151">eTag</span></span>|<span data-ttu-id="9c128-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c128-152">String</span></span>|<span data-ttu-id="9c128-153">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="9c128-153">ETag of the management condition.</span></span> <span data-ttu-id="9c128-154">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="9c128-154">Updated service side.</span></span> <span data-ttu-id="9c128-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9c128-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c128-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="9c128-156">applicablePlatforms</span></span>|<span data-ttu-id="9c128-157">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9c128-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="9c128-158">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="9c128-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="9c128-159">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9c128-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c128-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9c128-160">Relationships</span></span>
|<span data-ttu-id="9c128-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9c128-161">Relationship</span></span>|<span data-ttu-id="9c128-162">Typ</span><span class="sxs-lookup"><span data-stu-id="9c128-162">Type</span></span>|<span data-ttu-id="9c128-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c128-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c128-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="9c128-164">managementConditionStatements</span></span>|<span data-ttu-id="9c128-165">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9c128-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="9c128-166">Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="9c128-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="9c128-167">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="9c128-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c128-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9c128-168">JSON Representation</span></span>
<span data-ttu-id="9c128-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9c128-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```




