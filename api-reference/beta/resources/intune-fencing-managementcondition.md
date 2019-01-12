---
title: Ressourcentyp managementCondition
description: Management Bedingungen sind Ereignisse, die dynamisch wie Geo-Klammern, ausgelöst werden, können Zeit Klammern und Netzwerk Klammern.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: e0aeb73a93cd4c61b6d4680f73c2a9b8cee830c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986741"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="91497-103">Ressourcentyp managementCondition</span><span class="sxs-lookup"><span data-stu-id="91497-103">managementCondition resource type</span></span>

> <span data-ttu-id="91497-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91497-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91497-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91497-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91497-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="91497-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91497-107">Management Bedingungen sind Ereignisse, die dynamisch wie Geo-Klammern, ausgelöst werden, können Zeit Klammern und Netzwerk Klammern.</span><span class="sxs-lookup"><span data-stu-id="91497-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>
## <a name="methods"></a><span data-ttu-id="91497-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="91497-108">Methods</span></span>
|<span data-ttu-id="91497-109">Methode</span><span class="sxs-lookup"><span data-stu-id="91497-109">Method</span></span>|<span data-ttu-id="91497-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="91497-110">Return Type</span></span>|<span data-ttu-id="91497-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91497-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91497-112">Liste managementConditions</span><span class="sxs-lookup"><span data-stu-id="91497-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="91497-113">[ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="91497-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="91497-114">Listeneigenschaften und Beziehungen der [ManagementCondition](../resources/intune-fencing-managementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="91497-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="91497-115">Abrufen von managementCondition</span><span class="sxs-lookup"><span data-stu-id="91497-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="91497-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="91497-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="91497-117">Lesen Sie Eigenschaften und Beziehungen des [ManagementCondition](../resources/intune-fencing-managementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="91497-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="91497-118">GetManagementConditionsForPlatform-Funktion</span><span class="sxs-lookup"><span data-stu-id="91497-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="91497-119">[ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="91497-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="91497-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="91497-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="91497-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91497-121">Properties</span></span>
|<span data-ttu-id="91497-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91497-122">Property</span></span>|<span data-ttu-id="91497-123">Typ</span><span class="sxs-lookup"><span data-stu-id="91497-123">Type</span></span>|<span data-ttu-id="91497-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91497-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91497-125">id</span><span class="sxs-lookup"><span data-stu-id="91497-125">id</span></span>|<span data-ttu-id="91497-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91497-126">String</span></span>|<span data-ttu-id="91497-127">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="91497-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="91497-128">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="91497-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="91497-129">uniqueName</span><span class="sxs-lookup"><span data-stu-id="91497-129">uniqueName</span></span>|<span data-ttu-id="91497-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91497-130">String</span></span>|<span data-ttu-id="91497-131">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="91497-131">Unique name for the management condition.</span></span> <span data-ttu-id="91497-132">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="91497-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="91497-133">displayName</span><span class="sxs-lookup"><span data-stu-id="91497-133">displayName</span></span>|<span data-ttu-id="91497-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91497-134">String</span></span>|<span data-ttu-id="91497-135">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="91497-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="91497-136">description</span><span class="sxs-lookup"><span data-stu-id="91497-136">description</span></span>|<span data-ttu-id="91497-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91497-137">String</span></span>|<span data-ttu-id="91497-138">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="91497-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="91497-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91497-139">createdDateTime</span></span>|<span data-ttu-id="91497-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91497-140">DateTimeOffset</span></span>|<span data-ttu-id="91497-141">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="91497-141">The time the management condition was created.</span></span> <span data-ttu-id="91497-142">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="91497-142">Generated service side.</span></span>|
|<span data-ttu-id="91497-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91497-143">modifiedDateTime</span></span>|<span data-ttu-id="91497-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91497-144">DateTimeOffset</span></span>|<span data-ttu-id="91497-145">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="91497-145">The time the management condition was last modified.</span></span> <span data-ttu-id="91497-146">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="91497-146">Updated service side.</span></span>|
|<span data-ttu-id="91497-147">eTag</span><span class="sxs-lookup"><span data-stu-id="91497-147">eTag</span></span>|<span data-ttu-id="91497-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91497-148">String</span></span>|<span data-ttu-id="91497-149">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="91497-149">ETag of the management condition.</span></span> <span data-ttu-id="91497-150">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="91497-150">Updated service side.</span></span>|
|<span data-ttu-id="91497-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="91497-151">applicablePlatforms</span></span>|<span data-ttu-id="91497-152">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="91497-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="91497-153">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="91497-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91497-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="91497-154">Relationships</span></span>
|<span data-ttu-id="91497-155">Beziehung</span><span class="sxs-lookup"><span data-stu-id="91497-155">Relationship</span></span>|<span data-ttu-id="91497-156">Typ</span><span class="sxs-lookup"><span data-stu-id="91497-156">Type</span></span>|<span data-ttu-id="91497-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91497-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91497-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="91497-158">managementConditionStatements</span></span>|<span data-ttu-id="91497-159">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="91497-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="91497-160">Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="91497-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91497-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91497-161">JSON Representation</span></span>
<span data-ttu-id="91497-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91497-162">Here is a JSON representation of the resource.</span></span>
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





