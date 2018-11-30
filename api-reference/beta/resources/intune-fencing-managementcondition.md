---
title: Ressourcentyp managementCondition
description: Management Bedingungen sind Ereignisse, die dynamisch wie Geo-Klammern, ausgelöst werden, können Zeit Klammern und Netzwerk Klammern.
ms.openlocfilehash: 3c2bc1d7594e61642b96398bfb55d6aa38f3283d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060175"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="57aeb-103">Ressourcentyp managementCondition</span><span class="sxs-lookup"><span data-stu-id="57aeb-103">managementCondition resource type</span></span>

> <span data-ttu-id="57aeb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="57aeb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57aeb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="57aeb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57aeb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="57aeb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57aeb-107">Management Bedingungen sind Ereignisse, die dynamisch wie Geo-Klammern, ausgelöst werden, können Zeit Klammern und Netzwerk Klammern.</span><span class="sxs-lookup"><span data-stu-id="57aeb-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>
## <a name="methods"></a><span data-ttu-id="57aeb-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="57aeb-108">Methods</span></span>
|<span data-ttu-id="57aeb-109">Methode</span><span class="sxs-lookup"><span data-stu-id="57aeb-109">Method</span></span>|<span data-ttu-id="57aeb-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="57aeb-110">Return Type</span></span>|<span data-ttu-id="57aeb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57aeb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="57aeb-112">Liste managementConditions</span><span class="sxs-lookup"><span data-stu-id="57aeb-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="57aeb-113">[ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="57aeb-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="57aeb-114">Listeneigenschaften und Beziehungen der [ManagementCondition](../resources/intune-fencing-managementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="57aeb-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="57aeb-115">Abrufen von managementCondition</span><span class="sxs-lookup"><span data-stu-id="57aeb-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="57aeb-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="57aeb-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="57aeb-117">Lesen Sie Eigenschaften und Beziehungen des [ManagementCondition](../resources/intune-fencing-managementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="57aeb-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="57aeb-118">GetManagementConditionsForPlatform-Funktion</span><span class="sxs-lookup"><span data-stu-id="57aeb-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="57aeb-119">[ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="57aeb-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="57aeb-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="57aeb-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="57aeb-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="57aeb-121">Properties</span></span>
|<span data-ttu-id="57aeb-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="57aeb-122">Property</span></span>|<span data-ttu-id="57aeb-123">Typ</span><span class="sxs-lookup"><span data-stu-id="57aeb-123">Type</span></span>|<span data-ttu-id="57aeb-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57aeb-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57aeb-125">id</span><span class="sxs-lookup"><span data-stu-id="57aeb-125">id</span></span>|<span data-ttu-id="57aeb-126">String</span><span class="sxs-lookup"><span data-stu-id="57aeb-126">String</span></span>|<span data-ttu-id="57aeb-127">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="57aeb-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="57aeb-128">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="57aeb-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="57aeb-129">uniqueName</span><span class="sxs-lookup"><span data-stu-id="57aeb-129">uniqueName</span></span>|<span data-ttu-id="57aeb-130">String</span><span class="sxs-lookup"><span data-stu-id="57aeb-130">String</span></span>|<span data-ttu-id="57aeb-131">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="57aeb-131">Unique name for the management condition.</span></span> <span data-ttu-id="57aeb-132">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="57aeb-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="57aeb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="57aeb-133">displayName</span></span>|<span data-ttu-id="57aeb-134">String</span><span class="sxs-lookup"><span data-stu-id="57aeb-134">String</span></span>|<span data-ttu-id="57aeb-135">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="57aeb-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="57aeb-136">description</span><span class="sxs-lookup"><span data-stu-id="57aeb-136">description</span></span>|<span data-ttu-id="57aeb-137">String</span><span class="sxs-lookup"><span data-stu-id="57aeb-137">String</span></span>|<span data-ttu-id="57aeb-138">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="57aeb-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="57aeb-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57aeb-139">createdDateTime</span></span>|<span data-ttu-id="57aeb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57aeb-140">DateTimeOffset</span></span>|<span data-ttu-id="57aeb-141">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="57aeb-141">The time the management condition was created.</span></span> <span data-ttu-id="57aeb-142">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="57aeb-142">Generated service side.</span></span>|
|<span data-ttu-id="57aeb-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57aeb-143">modifiedDateTime</span></span>|<span data-ttu-id="57aeb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57aeb-144">DateTimeOffset</span></span>|<span data-ttu-id="57aeb-145">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="57aeb-145">The time the management condition was last modified.</span></span> <span data-ttu-id="57aeb-146">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="57aeb-146">Updated service side.</span></span>|
|<span data-ttu-id="57aeb-147">eTag</span><span class="sxs-lookup"><span data-stu-id="57aeb-147">eTag</span></span>|<span data-ttu-id="57aeb-148">String</span><span class="sxs-lookup"><span data-stu-id="57aeb-148">String</span></span>|<span data-ttu-id="57aeb-149">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="57aeb-149">ETag of the management condition.</span></span> <span data-ttu-id="57aeb-150">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="57aeb-150">Updated service side.</span></span>|
|<span data-ttu-id="57aeb-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="57aeb-151">applicablePlatforms</span></span>|<span data-ttu-id="57aeb-152">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="57aeb-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="57aeb-153">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="57aeb-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57aeb-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="57aeb-154">Relationships</span></span>
|<span data-ttu-id="57aeb-155">Beziehung</span><span class="sxs-lookup"><span data-stu-id="57aeb-155">Relationship</span></span>|<span data-ttu-id="57aeb-156">Typ</span><span class="sxs-lookup"><span data-stu-id="57aeb-156">Type</span></span>|<span data-ttu-id="57aeb-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57aeb-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57aeb-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="57aeb-158">managementConditionStatements</span></span>|<span data-ttu-id="57aeb-159">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="57aeb-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="57aeb-160">Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="57aeb-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57aeb-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="57aeb-161">JSON Representation</span></span>
<span data-ttu-id="57aeb-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="57aeb-162">Here is a JSON representation of the resource.</span></span>
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





