---
title: networkManagementCondition-Ressourcentyp
description: Enthält die Informationen zum Definieren einer Netzwerk Verwaltungsbedingung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 909eaa89a8303948cd97ba47299146b575e32c9f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164834"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="0aca8-103">networkManagementCondition-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0aca8-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="0aca8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0aca8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0aca8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0aca8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aca8-106">Enthält die Informationen zum Definieren einer Netzwerk Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0aca8-106">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="0aca8-107">Erbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0aca8-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0aca8-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="0aca8-108">Methods</span></span>
|<span data-ttu-id="0aca8-109">Methode</span><span class="sxs-lookup"><span data-stu-id="0aca8-109">Method</span></span>|<span data-ttu-id="0aca8-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0aca8-110">Return Type</span></span>|<span data-ttu-id="0aca8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aca8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0aca8-112">NetworkManagementConditions aufListen</span><span class="sxs-lookup"><span data-stu-id="0aca8-112">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="0aca8-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0aca8-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="0aca8-114">AufListen von Eigenschaften und Beziehungen der [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="0aca8-114">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="0aca8-115">NetworkManagementCondition abrufen</span><span class="sxs-lookup"><span data-stu-id="0aca8-115">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="0aca8-116">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="0aca8-116">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="0aca8-117">Lesen von Eigenschaften und Beziehungen des [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0aca8-117">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0aca8-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0aca8-118">Properties</span></span>
|<span data-ttu-id="0aca8-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0aca8-119">Property</span></span>|<span data-ttu-id="0aca8-120">Typ</span><span class="sxs-lookup"><span data-stu-id="0aca8-120">Type</span></span>|<span data-ttu-id="0aca8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aca8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aca8-122">id</span><span class="sxs-lookup"><span data-stu-id="0aca8-122">id</span></span>|<span data-ttu-id="0aca8-123">string</span><span class="sxs-lookup"><span data-stu-id="0aca8-123">String</span></span>|<span data-ttu-id="0aca8-124">Eindeutiger Bezeichner für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0aca8-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="0aca8-125">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="0aca8-125">System generated value assigned when created.</span></span> <span data-ttu-id="0aca8-126">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0aca8-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0aca8-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="0aca8-127">uniqueName</span></span>|<span data-ttu-id="0aca8-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aca8-128">String</span></span>|<span data-ttu-id="0aca8-129">Eindeutiger Name für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0aca8-129">Unique name for the management condition.</span></span> <span data-ttu-id="0aca8-130">Wird in Verwaltungs Bedingungsausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="0aca8-130">Used in management condition expressions.</span></span> <span data-ttu-id="0aca8-131">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0aca8-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0aca8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0aca8-132">displayName</span></span>|<span data-ttu-id="0aca8-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aca8-133">String</span></span>|<span data-ttu-id="0aca8-134">Der Administrator definierte Name der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0aca8-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="0aca8-135">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0aca8-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0aca8-136">description</span><span class="sxs-lookup"><span data-stu-id="0aca8-136">description</span></span>|<span data-ttu-id="0aca8-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aca8-137">String</span></span>|<span data-ttu-id="0aca8-138">Die vom Administrator definierte Beschreibung der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0aca8-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="0aca8-139">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0aca8-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0aca8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0aca8-140">createdDateTime</span></span>|<span data-ttu-id="0aca8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0aca8-141">DateTimeOffset</span></span>|<span data-ttu-id="0aca8-142">Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="0aca8-142">The time the management condition was created.</span></span> <span data-ttu-id="0aca8-143">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="0aca8-143">Generated service side.</span></span> <span data-ttu-id="0aca8-144">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0aca8-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0aca8-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0aca8-145">modifiedDateTime</span></span>|<span data-ttu-id="0aca8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0aca8-146">DateTimeOffset</span></span>|<span data-ttu-id="0aca8-147">Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="0aca8-147">The time the management condition was last modified.</span></span> <span data-ttu-id="0aca8-148">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="0aca8-148">Updated service side.</span></span> <span data-ttu-id="0aca8-149">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0aca8-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0aca8-150">eTag</span><span class="sxs-lookup"><span data-stu-id="0aca8-150">eTag</span></span>|<span data-ttu-id="0aca8-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aca8-151">String</span></span>|<span data-ttu-id="0aca8-152">ETag der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0aca8-152">ETag of the management condition.</span></span> <span data-ttu-id="0aca8-153">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="0aca8-153">Updated service side.</span></span> <span data-ttu-id="0aca8-154">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0aca8-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0aca8-155">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0aca8-155">applicablePlatforms</span></span>|<span data-ttu-id="0aca8-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0aca8-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0aca8-157">Die entsprechenden Plattformen für diese Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0aca8-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="0aca8-158">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0aca8-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0aca8-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0aca8-159">Relationships</span></span>
|<span data-ttu-id="0aca8-160">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0aca8-160">Relationship</span></span>|<span data-ttu-id="0aca8-161">Typ</span><span class="sxs-lookup"><span data-stu-id="0aca8-161">Type</span></span>|<span data-ttu-id="0aca8-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aca8-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aca8-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="0aca8-163">managementConditionStatements</span></span>|<span data-ttu-id="0aca8-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0aca8-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="0aca8-165">Die der Verwaltungsbedingung zugeordneten Verwaltungs Bedingungsanweisungen.</span><span class="sxs-lookup"><span data-stu-id="0aca8-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="0aca8-166">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0aca8-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0aca8-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0aca8-167">JSON Representation</span></span>
<span data-ttu-id="0aca8-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0aca8-168">Here is a JSON representation of the resource.</span></span>
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




