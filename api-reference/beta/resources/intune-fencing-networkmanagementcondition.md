---
title: Ressourcentyp networkManagementCondition
description: Enthält Informationen, die eine Network Management Bedingung zu definieren.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7d91ac60ae52f3317e8148e8bb4adcaf82afac53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806510"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="a560b-103">Ressourcentyp networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="a560b-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="a560b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a560b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a560b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a560b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a560b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a560b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a560b-107">Enthält Informationen, die eine Network Management Bedingung zu definieren.</span><span class="sxs-lookup"><span data-stu-id="a560b-107">Contains the information to define a network management condition.</span></span>

<span data-ttu-id="a560b-108">Erbt vom [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a560b-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a560b-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="a560b-109">Methods</span></span>
|<span data-ttu-id="a560b-110">Methode</span><span class="sxs-lookup"><span data-stu-id="a560b-110">Method</span></span>|<span data-ttu-id="a560b-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a560b-111">Return Type</span></span>|<span data-ttu-id="a560b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a560b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a560b-113">Liste networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="a560b-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="a560b-114">[NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a560b-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="a560b-115">Listeneigenschaften und Beziehungen der [NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="a560b-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="a560b-116">Abrufen von networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="a560b-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="a560b-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="a560b-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="a560b-118">Lesen Sie Eigenschaften und Beziehungen des [NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a560b-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a560b-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a560b-119">Properties</span></span>
|<span data-ttu-id="a560b-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a560b-120">Property</span></span>|<span data-ttu-id="a560b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a560b-121">Type</span></span>|<span data-ttu-id="a560b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a560b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a560b-123">id</span><span class="sxs-lookup"><span data-stu-id="a560b-123">id</span></span>|<span data-ttu-id="a560b-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a560b-124">String</span></span>|<span data-ttu-id="a560b-125">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a560b-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="a560b-126">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="a560b-126">System generated value assigned when created.</span></span> <span data-ttu-id="a560b-127">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a560b-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a560b-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="a560b-128">uniqueName</span></span>|<span data-ttu-id="a560b-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a560b-129">String</span></span>|<span data-ttu-id="a560b-130">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a560b-130">Unique name for the management condition.</span></span> <span data-ttu-id="a560b-131">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="a560b-131">Used in management condition expressions.</span></span> <span data-ttu-id="a560b-132">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a560b-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a560b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a560b-133">displayName</span></span>|<span data-ttu-id="a560b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a560b-134">String</span></span>|<span data-ttu-id="a560b-135">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a560b-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="a560b-136">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a560b-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a560b-137">description</span><span class="sxs-lookup"><span data-stu-id="a560b-137">description</span></span>|<span data-ttu-id="a560b-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a560b-138">String</span></span>|<span data-ttu-id="a560b-139">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a560b-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="a560b-140">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a560b-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a560b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a560b-141">createdDateTime</span></span>|<span data-ttu-id="a560b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a560b-142">DateTimeOffset</span></span>|<span data-ttu-id="a560b-143">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="a560b-143">The time the management condition was created.</span></span> <span data-ttu-id="a560b-144">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="a560b-144">Generated service side.</span></span> <span data-ttu-id="a560b-145">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a560b-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a560b-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a560b-146">modifiedDateTime</span></span>|<span data-ttu-id="a560b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a560b-147">DateTimeOffset</span></span>|<span data-ttu-id="a560b-148">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="a560b-148">The time the management condition was last modified.</span></span> <span data-ttu-id="a560b-149">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="a560b-149">Updated service side.</span></span> <span data-ttu-id="a560b-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a560b-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a560b-151">eTag</span><span class="sxs-lookup"><span data-stu-id="a560b-151">eTag</span></span>|<span data-ttu-id="a560b-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a560b-152">String</span></span>|<span data-ttu-id="a560b-153">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a560b-153">ETag of the management condition.</span></span> <span data-ttu-id="a560b-154">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="a560b-154">Updated service side.</span></span> <span data-ttu-id="a560b-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a560b-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="a560b-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="a560b-156">applicablePlatforms</span></span>|<span data-ttu-id="a560b-157">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a560b-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="a560b-158">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="a560b-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="a560b-159">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a560b-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a560b-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a560b-160">Relationships</span></span>
|<span data-ttu-id="a560b-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="a560b-161">Relationship</span></span>|<span data-ttu-id="a560b-162">Typ</span><span class="sxs-lookup"><span data-stu-id="a560b-162">Type</span></span>|<span data-ttu-id="a560b-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a560b-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a560b-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="a560b-164">managementConditionStatements</span></span>|<span data-ttu-id="a560b-165">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a560b-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="a560b-166">Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="a560b-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="a560b-167">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="a560b-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a560b-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a560b-168">JSON Representation</span></span>
<span data-ttu-id="a560b-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a560b-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
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





