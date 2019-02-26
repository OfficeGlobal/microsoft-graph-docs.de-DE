---
title: managementCondition-Ressourcentyp
description: Verwaltungsbedingungen sind Ereignisse, die dynamisch ausgelöst werden können, beispielsweise Geofences, Zeit Zäune und Netzwerk Zäune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 594716867cec1dcef9e0fee87af21fb63af99df0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163105"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="636b4-103">managementCondition-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="636b4-103">managementCondition resource type</span></span>

> <span data-ttu-id="636b4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="636b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="636b4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="636b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="636b4-106">Verwaltungsbedingungen sind Ereignisse, die dynamisch ausgelöst werden können, beispielsweise Geofences, Zeit Zäune und Netzwerk Zäune.</span><span class="sxs-lookup"><span data-stu-id="636b4-106">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="636b4-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="636b4-107">Methods</span></span>
|<span data-ttu-id="636b4-108">Methode</span><span class="sxs-lookup"><span data-stu-id="636b4-108">Method</span></span>|<span data-ttu-id="636b4-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="636b4-109">Return Type</span></span>|<span data-ttu-id="636b4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="636b4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="636b4-111">ManagementConditions aufListen</span><span class="sxs-lookup"><span data-stu-id="636b4-111">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="636b4-112">[managementCondition](../resources/intune-fencing-managementcondition.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="636b4-112">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="636b4-113">AufListen von Eigenschaften und Beziehungen der [managementCondition](../resources/intune-fencing-managementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="636b4-113">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="636b4-114">ManagementCondition abrufen</span><span class="sxs-lookup"><span data-stu-id="636b4-114">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="636b4-115">managementCondition</span><span class="sxs-lookup"><span data-stu-id="636b4-115">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="636b4-116">Lesen von Eigenschaften und Beziehungen des [managementCondition](../resources/intune-fencing-managementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="636b4-116">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="636b4-117">getManagementConditionsForPlatform-Funktion</span><span class="sxs-lookup"><span data-stu-id="636b4-117">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="636b4-118">[managementCondition](../resources/intune-fencing-managementcondition.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="636b4-118">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="636b4-119">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="636b4-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="636b4-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="636b4-120">Properties</span></span>
|<span data-ttu-id="636b4-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="636b4-121">Property</span></span>|<span data-ttu-id="636b4-122">Typ</span><span class="sxs-lookup"><span data-stu-id="636b4-122">Type</span></span>|<span data-ttu-id="636b4-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="636b4-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="636b4-124">id</span><span class="sxs-lookup"><span data-stu-id="636b4-124">id</span></span>|<span data-ttu-id="636b4-125">string</span><span class="sxs-lookup"><span data-stu-id="636b4-125">String</span></span>|<span data-ttu-id="636b4-126">Eindeutiger Bezeichner für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="636b4-126">Unique identifier for the management condition.</span></span> <span data-ttu-id="636b4-127">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="636b4-127">System generated value assigned when created.</span></span>|
|<span data-ttu-id="636b4-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="636b4-128">uniqueName</span></span>|<span data-ttu-id="636b4-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="636b4-129">String</span></span>|<span data-ttu-id="636b4-130">Eindeutiger Name für die Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="636b4-130">Unique name for the management condition.</span></span> <span data-ttu-id="636b4-131">Wird in Verwaltungs Bedingungsausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="636b4-131">Used in management condition expressions.</span></span>|
|<span data-ttu-id="636b4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="636b4-132">displayName</span></span>|<span data-ttu-id="636b4-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="636b4-133">String</span></span>|<span data-ttu-id="636b4-134">Der Administrator definierte Name der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="636b4-134">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="636b4-135">description</span><span class="sxs-lookup"><span data-stu-id="636b4-135">description</span></span>|<span data-ttu-id="636b4-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="636b4-136">String</span></span>|<span data-ttu-id="636b4-137">Die vom Administrator definierte Beschreibung der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="636b4-137">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="636b4-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="636b4-138">createdDateTime</span></span>|<span data-ttu-id="636b4-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="636b4-139">DateTimeOffset</span></span>|<span data-ttu-id="636b4-140">Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="636b4-140">The time the management condition was created.</span></span> <span data-ttu-id="636b4-141">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="636b4-141">Generated service side.</span></span>|
|<span data-ttu-id="636b4-142">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="636b4-142">modifiedDateTime</span></span>|<span data-ttu-id="636b4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="636b4-143">DateTimeOffset</span></span>|<span data-ttu-id="636b4-144">Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="636b4-144">The time the management condition was last modified.</span></span> <span data-ttu-id="636b4-145">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="636b4-145">Updated service side.</span></span>|
|<span data-ttu-id="636b4-146">eTag</span><span class="sxs-lookup"><span data-stu-id="636b4-146">eTag</span></span>|<span data-ttu-id="636b4-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="636b4-147">String</span></span>|<span data-ttu-id="636b4-148">ETag der Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="636b4-148">ETag of the management condition.</span></span> <span data-ttu-id="636b4-149">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="636b4-149">Updated service side.</span></span>|
|<span data-ttu-id="636b4-150">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="636b4-150">applicablePlatforms</span></span>|<span data-ttu-id="636b4-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="636b4-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="636b4-152">Die entsprechenden Plattformen für diese Verwaltungsbedingung.</span><span class="sxs-lookup"><span data-stu-id="636b4-152">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="636b4-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="636b4-153">Relationships</span></span>
|<span data-ttu-id="636b4-154">Beziehung</span><span class="sxs-lookup"><span data-stu-id="636b4-154">Relationship</span></span>|<span data-ttu-id="636b4-155">Typ</span><span class="sxs-lookup"><span data-stu-id="636b4-155">Type</span></span>|<span data-ttu-id="636b4-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="636b4-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="636b4-157">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="636b4-157">managementConditionStatements</span></span>|<span data-ttu-id="636b4-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="636b4-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="636b4-159">Die der Verwaltungsbedingung zugeordneten Verwaltungs Bedingungsanweisungen.</span><span class="sxs-lookup"><span data-stu-id="636b4-159">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="636b4-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="636b4-160">JSON Representation</span></span>
<span data-ttu-id="636b4-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="636b4-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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




