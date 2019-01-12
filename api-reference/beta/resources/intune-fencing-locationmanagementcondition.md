---
title: Ressourcentyp locationManagementCondition
description: Enthält Informationen zum Definieren einer Speicherort Management Bedingung ein Interessenbereich zum Überwachen.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 541cf74decad641f6dc7751945e1d0ffceee1366
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922977"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="bb055-103">Ressourcentyp locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="bb055-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="bb055-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bb055-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb055-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bb055-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb055-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bb055-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb055-107">Enthält Informationen zum Definieren einer Speicherort Management Bedingung ein Interessenbereich zum Überwachen.</span><span class="sxs-lookup"><span data-stu-id="bb055-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>

<span data-ttu-id="bb055-108">Erbt vom [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bb055-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bb055-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="bb055-109">Methods</span></span>
|<span data-ttu-id="bb055-110">Methode</span><span class="sxs-lookup"><span data-stu-id="bb055-110">Method</span></span>|<span data-ttu-id="bb055-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bb055-111">Return Type</span></span>|<span data-ttu-id="bb055-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb055-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb055-113">Liste locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="bb055-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="bb055-114">[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bb055-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="bb055-115">Listeneigenschaften und Beziehungen der [LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="bb055-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="bb055-116">Abrufen von locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="bb055-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="bb055-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="bb055-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="bb055-118">Lesen Sie Eigenschaften und Beziehungen des [LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb055-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb055-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb055-119">Properties</span></span>
|<span data-ttu-id="bb055-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb055-120">Property</span></span>|<span data-ttu-id="bb055-121">Typ</span><span class="sxs-lookup"><span data-stu-id="bb055-121">Type</span></span>|<span data-ttu-id="bb055-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb055-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb055-123">id</span><span class="sxs-lookup"><span data-stu-id="bb055-123">id</span></span>|<span data-ttu-id="bb055-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb055-124">String</span></span>|<span data-ttu-id="bb055-125">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="bb055-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="bb055-126">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="bb055-126">System generated value assigned when created.</span></span> <span data-ttu-id="bb055-127">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bb055-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb055-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="bb055-128">uniqueName</span></span>|<span data-ttu-id="bb055-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb055-129">String</span></span>|<span data-ttu-id="bb055-130">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="bb055-130">Unique name for the management condition.</span></span> <span data-ttu-id="bb055-131">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="bb055-131">Used in management condition expressions.</span></span> <span data-ttu-id="bb055-132">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bb055-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb055-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bb055-133">displayName</span></span>|<span data-ttu-id="bb055-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb055-134">String</span></span>|<span data-ttu-id="bb055-135">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="bb055-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="bb055-136">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bb055-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb055-137">description</span><span class="sxs-lookup"><span data-stu-id="bb055-137">description</span></span>|<span data-ttu-id="bb055-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb055-138">String</span></span>|<span data-ttu-id="bb055-139">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="bb055-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="bb055-140">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bb055-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb055-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb055-141">createdDateTime</span></span>|<span data-ttu-id="bb055-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb055-142">DateTimeOffset</span></span>|<span data-ttu-id="bb055-143">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="bb055-143">The time the management condition was created.</span></span> <span data-ttu-id="bb055-144">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="bb055-144">Generated service side.</span></span> <span data-ttu-id="bb055-145">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bb055-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb055-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb055-146">modifiedDateTime</span></span>|<span data-ttu-id="bb055-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb055-147">DateTimeOffset</span></span>|<span data-ttu-id="bb055-148">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="bb055-148">The time the management condition was last modified.</span></span> <span data-ttu-id="bb055-149">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="bb055-149">Updated service side.</span></span> <span data-ttu-id="bb055-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bb055-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb055-151">eTag</span><span class="sxs-lookup"><span data-stu-id="bb055-151">eTag</span></span>|<span data-ttu-id="bb055-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb055-152">String</span></span>|<span data-ttu-id="bb055-153">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="bb055-153">ETag of the management condition.</span></span> <span data-ttu-id="bb055-154">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="bb055-154">Updated service side.</span></span> <span data-ttu-id="bb055-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bb055-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="bb055-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="bb055-156">applicablePlatforms</span></span>|<span data-ttu-id="bb055-157">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bb055-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="bb055-158">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="bb055-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="bb055-159">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bb055-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb055-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bb055-160">Relationships</span></span>
|<span data-ttu-id="bb055-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bb055-161">Relationship</span></span>|<span data-ttu-id="bb055-162">Typ</span><span class="sxs-lookup"><span data-stu-id="bb055-162">Type</span></span>|<span data-ttu-id="bb055-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb055-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb055-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="bb055-164">managementConditionStatements</span></span>|<span data-ttu-id="bb055-165">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bb055-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="bb055-166">Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="bb055-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="bb055-167">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="bb055-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb055-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bb055-168">JSON Representation</span></span>
<span data-ttu-id="bb055-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bb055-169">Here is a JSON representation of the resource.</span></span>
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





