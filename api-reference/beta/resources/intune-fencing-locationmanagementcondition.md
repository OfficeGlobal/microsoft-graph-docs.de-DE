---
title: locationManagementCondition-Ressourcentyp
description: Enthält die Informationen zum Definieren einer Standort Verwaltungsbedingung für die Überwachung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07bf05fa8ab6f7f7f1ce6e1978645f289ea57a2f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143309"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="0e349-103">locationManagementCondition-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0e349-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="0e349-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e349-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e349-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0e349-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e349-106">Enthält die Informationen zum Definieren einer Standort Verwaltungsbedingung für die Überwachung.</span><span class="sxs-lookup"><span data-stu-id="0e349-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="0e349-107">Erbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e349-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0e349-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="0e349-108">Methods</span></span>
|<span data-ttu-id="0e349-109">Methode</span><span class="sxs-lookup"><span data-stu-id="0e349-109">Method</span></span>|<span data-ttu-id="0e349-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0e349-110">Return Type</span></span>|<span data-ttu-id="0e349-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e349-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e349-112">LocationManagementConditions aufListen</span><span class="sxs-lookup"><span data-stu-id="0e349-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="0e349-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0e349-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="0e349-114">AufListen von Eigenschaften und Beziehungen der [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="0e349-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="0e349-115">LocationManagementCondition abrufen</span><span class="sxs-lookup"><span data-stu-id="0e349-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="0e349-116">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="0e349-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="0e349-117">Lesen von Eigenschaften und Beziehungen des [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e349-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e349-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0e349-118">Properties</span></span>
|<span data-ttu-id="0e349-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e349-119">Property</span></span>|<span data-ttu-id="0e349-120">Typ</span><span class="sxs-lookup"><span data-stu-id="0e349-120">Type</span></span>|<span data-ttu-id="0e349-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e349-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e349-122">id</span><span class="sxs-lookup"><span data-stu-id="0e349-122">id</span></span>|<span data-ttu-id="0e349-123">string</span><span class="sxs-lookup"><span data-stu-id="0e349-123">String</span></span>|<span data-ttu-id="0e349-124">Eindeutiger Bezeichner für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0e349-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="0e349-125">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="0e349-125">System generated value assigned when created.</span></span> <span data-ttu-id="0e349-126">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e349-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e349-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="0e349-127">uniqueName</span></span>|<span data-ttu-id="0e349-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e349-128">String</span></span>|<span data-ttu-id="0e349-129">Eindeutiger Name für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0e349-129">Unique name for the management condition.</span></span> <span data-ttu-id="0e349-130">Wird in Verwaltungs Bedingungsausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="0e349-130">Used in management condition expressions.</span></span> <span data-ttu-id="0e349-131">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e349-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e349-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0e349-132">displayName</span></span>|<span data-ttu-id="0e349-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e349-133">String</span></span>|<span data-ttu-id="0e349-134">Der Administrator definierte Name der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0e349-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="0e349-135">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e349-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e349-136">description</span><span class="sxs-lookup"><span data-stu-id="0e349-136">description</span></span>|<span data-ttu-id="0e349-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e349-137">String</span></span>|<span data-ttu-id="0e349-138">Die vom Administrator definierte Beschreibung der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0e349-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="0e349-139">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e349-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e349-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e349-140">createdDateTime</span></span>|<span data-ttu-id="0e349-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e349-141">DateTimeOffset</span></span>|<span data-ttu-id="0e349-142">Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="0e349-142">The time the management condition was created.</span></span> <span data-ttu-id="0e349-143">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="0e349-143">Generated service side.</span></span> <span data-ttu-id="0e349-144">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e349-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e349-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e349-145">modifiedDateTime</span></span>|<span data-ttu-id="0e349-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e349-146">DateTimeOffset</span></span>|<span data-ttu-id="0e349-147">Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="0e349-147">The time the management condition was last modified.</span></span> <span data-ttu-id="0e349-148">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="0e349-148">Updated service side.</span></span> <span data-ttu-id="0e349-149">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e349-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e349-150">eTag</span><span class="sxs-lookup"><span data-stu-id="0e349-150">eTag</span></span>|<span data-ttu-id="0e349-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e349-151">String</span></span>|<span data-ttu-id="0e349-152">ETag der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0e349-152">ETag of the management condition.</span></span> <span data-ttu-id="0e349-153">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="0e349-153">Updated service side.</span></span> <span data-ttu-id="0e349-154">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e349-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e349-155">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0e349-155">applicablePlatforms</span></span>|<span data-ttu-id="0e349-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0e349-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0e349-157">Die entsprechenden Plattformen für diese Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="0e349-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="0e349-158">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e349-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e349-159">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0e349-159">Relationships</span></span>
|<span data-ttu-id="0e349-160">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0e349-160">Relationship</span></span>|<span data-ttu-id="0e349-161">Typ</span><span class="sxs-lookup"><span data-stu-id="0e349-161">Type</span></span>|<span data-ttu-id="0e349-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e349-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e349-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="0e349-163">managementConditionStatements</span></span>|<span data-ttu-id="0e349-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0e349-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="0e349-165">Die der Verwaltungsbedingung zugeordneten Verwaltungs Bedingungsanweisungen.</span><span class="sxs-lookup"><span data-stu-id="0e349-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="0e349-166">Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e349-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e349-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0e349-167">JSON Representation</span></span>
<span data-ttu-id="0e349-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0e349-168">Here is a JSON representation of the resource.</span></span>
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




