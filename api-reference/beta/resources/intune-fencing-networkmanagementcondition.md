---
title: Ressourcentyp networkManagementCondition
description: Enthält Informationen, die eine Network Management Bedingung zu definieren.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 00ccc045892290ff03e68a109ccc01c4d5dbf8a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927044"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="505ee-103">Ressourcentyp networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="505ee-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="505ee-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="505ee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="505ee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="505ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="505ee-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="505ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="505ee-107">Enthält Informationen, die eine Network Management Bedingung zu definieren.</span><span class="sxs-lookup"><span data-stu-id="505ee-107">Contains the information to define a network management condition.</span></span>

<span data-ttu-id="505ee-108">Erbt vom [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="505ee-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="505ee-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="505ee-109">Methods</span></span>
|<span data-ttu-id="505ee-110">Methode</span><span class="sxs-lookup"><span data-stu-id="505ee-110">Method</span></span>|<span data-ttu-id="505ee-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="505ee-111">Return Type</span></span>|<span data-ttu-id="505ee-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="505ee-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="505ee-113">Liste networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="505ee-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="505ee-114">[NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="505ee-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="505ee-115">Listeneigenschaften und Beziehungen der [NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="505ee-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="505ee-116">Abrufen von networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="505ee-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="505ee-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="505ee-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="505ee-118">Lesen Sie Eigenschaften und Beziehungen des [NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="505ee-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="505ee-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="505ee-119">Properties</span></span>
|<span data-ttu-id="505ee-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="505ee-120">Property</span></span>|<span data-ttu-id="505ee-121">Typ</span><span class="sxs-lookup"><span data-stu-id="505ee-121">Type</span></span>|<span data-ttu-id="505ee-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="505ee-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="505ee-123">id</span><span class="sxs-lookup"><span data-stu-id="505ee-123">id</span></span>|<span data-ttu-id="505ee-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="505ee-124">String</span></span>|<span data-ttu-id="505ee-125">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="505ee-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="505ee-126">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="505ee-126">System generated value assigned when created.</span></span> <span data-ttu-id="505ee-127">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="505ee-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="505ee-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="505ee-128">uniqueName</span></span>|<span data-ttu-id="505ee-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="505ee-129">String</span></span>|<span data-ttu-id="505ee-130">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="505ee-130">Unique name for the management condition.</span></span> <span data-ttu-id="505ee-131">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="505ee-131">Used in management condition expressions.</span></span> <span data-ttu-id="505ee-132">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="505ee-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="505ee-133">displayName</span><span class="sxs-lookup"><span data-stu-id="505ee-133">displayName</span></span>|<span data-ttu-id="505ee-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="505ee-134">String</span></span>|<span data-ttu-id="505ee-135">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="505ee-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="505ee-136">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="505ee-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="505ee-137">description</span><span class="sxs-lookup"><span data-stu-id="505ee-137">description</span></span>|<span data-ttu-id="505ee-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="505ee-138">String</span></span>|<span data-ttu-id="505ee-139">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="505ee-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="505ee-140">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="505ee-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="505ee-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="505ee-141">createdDateTime</span></span>|<span data-ttu-id="505ee-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="505ee-142">DateTimeOffset</span></span>|<span data-ttu-id="505ee-143">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="505ee-143">The time the management condition was created.</span></span> <span data-ttu-id="505ee-144">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="505ee-144">Generated service side.</span></span> <span data-ttu-id="505ee-145">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="505ee-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="505ee-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="505ee-146">modifiedDateTime</span></span>|<span data-ttu-id="505ee-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="505ee-147">DateTimeOffset</span></span>|<span data-ttu-id="505ee-148">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="505ee-148">The time the management condition was last modified.</span></span> <span data-ttu-id="505ee-149">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="505ee-149">Updated service side.</span></span> <span data-ttu-id="505ee-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="505ee-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="505ee-151">eTag</span><span class="sxs-lookup"><span data-stu-id="505ee-151">eTag</span></span>|<span data-ttu-id="505ee-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="505ee-152">String</span></span>|<span data-ttu-id="505ee-153">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="505ee-153">ETag of the management condition.</span></span> <span data-ttu-id="505ee-154">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="505ee-154">Updated service side.</span></span> <span data-ttu-id="505ee-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="505ee-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="505ee-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="505ee-156">applicablePlatforms</span></span>|<span data-ttu-id="505ee-157">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="505ee-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="505ee-158">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="505ee-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="505ee-159">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="505ee-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="505ee-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="505ee-160">Relationships</span></span>
|<span data-ttu-id="505ee-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="505ee-161">Relationship</span></span>|<span data-ttu-id="505ee-162">Typ</span><span class="sxs-lookup"><span data-stu-id="505ee-162">Type</span></span>|<span data-ttu-id="505ee-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="505ee-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="505ee-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="505ee-164">managementConditionStatements</span></span>|<span data-ttu-id="505ee-165">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="505ee-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="505ee-166">Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="505ee-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="505ee-167">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="505ee-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="505ee-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="505ee-168">JSON Representation</span></span>
<span data-ttu-id="505ee-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="505ee-169">Here is a JSON representation of the resource.</span></span>
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





