---
title: Ressourcentyp networkManagementCondition
description: Enthält Informationen, die eine Network Management Bedingung zu definieren.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4eadaf4e67b7ffe5551fc82376c3a4bb58255f61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415761"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="f6d80-103">Ressourcentyp networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="f6d80-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="f6d80-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f6d80-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f6d80-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6d80-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6d80-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6d80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6d80-107">Enthält Informationen, die eine Network Management Bedingung zu definieren.</span><span class="sxs-lookup"><span data-stu-id="f6d80-107">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="f6d80-108">Erbt vom [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f6d80-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f6d80-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="f6d80-109">Methods</span></span>
|<span data-ttu-id="f6d80-110">Methode</span><span class="sxs-lookup"><span data-stu-id="f6d80-110">Method</span></span>|<span data-ttu-id="f6d80-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f6d80-111">Return Type</span></span>|<span data-ttu-id="f6d80-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6d80-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f6d80-113">Liste networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="f6d80-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="f6d80-114">[NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f6d80-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="f6d80-115">Listeneigenschaften und Beziehungen der [NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="f6d80-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="f6d80-116">Abrufen von networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="f6d80-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="f6d80-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="f6d80-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="f6d80-118">Lesen Sie Eigenschaften und Beziehungen des [NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f6d80-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6d80-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f6d80-119">Properties</span></span>
|<span data-ttu-id="f6d80-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6d80-120">Property</span></span>|<span data-ttu-id="f6d80-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f6d80-121">Type</span></span>|<span data-ttu-id="f6d80-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6d80-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d80-123">id</span><span class="sxs-lookup"><span data-stu-id="f6d80-123">id</span></span>|<span data-ttu-id="f6d80-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6d80-124">String</span></span>|<span data-ttu-id="f6d80-125">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f6d80-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="f6d80-126">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="f6d80-126">System generated value assigned when created.</span></span> <span data-ttu-id="f6d80-127">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f6d80-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f6d80-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="f6d80-128">uniqueName</span></span>|<span data-ttu-id="f6d80-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6d80-129">String</span></span>|<span data-ttu-id="f6d80-130">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f6d80-130">Unique name for the management condition.</span></span> <span data-ttu-id="f6d80-131">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="f6d80-131">Used in management condition expressions.</span></span> <span data-ttu-id="f6d80-132">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f6d80-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f6d80-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f6d80-133">displayName</span></span>|<span data-ttu-id="f6d80-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6d80-134">String</span></span>|<span data-ttu-id="f6d80-135">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f6d80-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="f6d80-136">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f6d80-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f6d80-137">description</span><span class="sxs-lookup"><span data-stu-id="f6d80-137">description</span></span>|<span data-ttu-id="f6d80-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6d80-138">String</span></span>|<span data-ttu-id="f6d80-139">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f6d80-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="f6d80-140">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f6d80-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f6d80-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6d80-141">createdDateTime</span></span>|<span data-ttu-id="f6d80-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6d80-142">DateTimeOffset</span></span>|<span data-ttu-id="f6d80-143">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f6d80-143">The time the management condition was created.</span></span> <span data-ttu-id="f6d80-144">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="f6d80-144">Generated service side.</span></span> <span data-ttu-id="f6d80-145">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f6d80-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f6d80-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6d80-146">modifiedDateTime</span></span>|<span data-ttu-id="f6d80-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6d80-147">DateTimeOffset</span></span>|<span data-ttu-id="f6d80-148">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="f6d80-148">The time the management condition was last modified.</span></span> <span data-ttu-id="f6d80-149">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="f6d80-149">Updated service side.</span></span> <span data-ttu-id="f6d80-150">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f6d80-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f6d80-151">eTag</span><span class="sxs-lookup"><span data-stu-id="f6d80-151">eTag</span></span>|<span data-ttu-id="f6d80-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6d80-152">String</span></span>|<span data-ttu-id="f6d80-153">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f6d80-153">ETag of the management condition.</span></span> <span data-ttu-id="f6d80-154">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="f6d80-154">Updated service side.</span></span> <span data-ttu-id="f6d80-155">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f6d80-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f6d80-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="f6d80-156">applicablePlatforms</span></span>|<span data-ttu-id="f6d80-157">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f6d80-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f6d80-158">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="f6d80-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="f6d80-159">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f6d80-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6d80-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f6d80-160">Relationships</span></span>
|<span data-ttu-id="f6d80-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f6d80-161">Relationship</span></span>|<span data-ttu-id="f6d80-162">Typ</span><span class="sxs-lookup"><span data-stu-id="f6d80-162">Type</span></span>|<span data-ttu-id="f6d80-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6d80-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d80-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="f6d80-164">managementConditionStatements</span></span>|<span data-ttu-id="f6d80-165">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f6d80-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="f6d80-166">Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="f6d80-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="f6d80-167">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f6d80-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6d80-168">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f6d80-168">JSON Representation</span></span>
<span data-ttu-id="f6d80-169">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f6d80-169">Here is a JSON representation of the resource.</span></span>
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




