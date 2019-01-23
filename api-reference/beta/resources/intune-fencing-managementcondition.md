---
title: Ressourcentyp managementCondition
description: Management Bedingungen sind Ereignisse, die dynamisch wie Geo-Klammern, ausgelöst werden, können Zeit Klammern und Netzwerk Klammern.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c41b4cb3143349ba0fdd97633a70ec7b38e266ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405856"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="70006-103">Ressourcentyp managementCondition</span><span class="sxs-lookup"><span data-stu-id="70006-103">managementCondition resource type</span></span>

> <span data-ttu-id="70006-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="70006-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="70006-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70006-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70006-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="70006-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70006-107">Management Bedingungen sind Ereignisse, die dynamisch wie Geo-Klammern, ausgelöst werden, können Zeit Klammern und Netzwerk Klammern.</span><span class="sxs-lookup"><span data-stu-id="70006-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="70006-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="70006-108">Methods</span></span>
|<span data-ttu-id="70006-109">Methode</span><span class="sxs-lookup"><span data-stu-id="70006-109">Method</span></span>|<span data-ttu-id="70006-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="70006-110">Return Type</span></span>|<span data-ttu-id="70006-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70006-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="70006-112">Liste managementConditions</span><span class="sxs-lookup"><span data-stu-id="70006-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="70006-113">[ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70006-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="70006-114">Listeneigenschaften und Beziehungen der [ManagementCondition](../resources/intune-fencing-managementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="70006-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="70006-115">Abrufen von managementCondition</span><span class="sxs-lookup"><span data-stu-id="70006-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="70006-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="70006-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="70006-117">Lesen Sie Eigenschaften und Beziehungen des [ManagementCondition](../resources/intune-fencing-managementcondition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="70006-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="70006-118">GetManagementConditionsForPlatform-Funktion</span><span class="sxs-lookup"><span data-stu-id="70006-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="70006-119">[ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70006-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="70006-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="70006-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="70006-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="70006-121">Properties</span></span>
|<span data-ttu-id="70006-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70006-122">Property</span></span>|<span data-ttu-id="70006-123">Typ</span><span class="sxs-lookup"><span data-stu-id="70006-123">Type</span></span>|<span data-ttu-id="70006-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70006-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70006-125">id</span><span class="sxs-lookup"><span data-stu-id="70006-125">id</span></span>|<span data-ttu-id="70006-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70006-126">String</span></span>|<span data-ttu-id="70006-127">Eindeutiger Bezeichner für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="70006-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="70006-128">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="70006-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="70006-129">uniqueName</span><span class="sxs-lookup"><span data-stu-id="70006-129">uniqueName</span></span>|<span data-ttu-id="70006-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70006-130">String</span></span>|<span data-ttu-id="70006-131">Eindeutiger Name für die Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="70006-131">Unique name for the management condition.</span></span> <span data-ttu-id="70006-132">In Management Bedingung Ausdrücken verwendet.</span><span class="sxs-lookup"><span data-stu-id="70006-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="70006-133">displayName</span><span class="sxs-lookup"><span data-stu-id="70006-133">displayName</span></span>|<span data-ttu-id="70006-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70006-134">String</span></span>|<span data-ttu-id="70006-135">Der Administrator definierter Name der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="70006-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="70006-136">description</span><span class="sxs-lookup"><span data-stu-id="70006-136">description</span></span>|<span data-ttu-id="70006-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70006-137">String</span></span>|<span data-ttu-id="70006-138">Der Administrator definiert die Beschreibung der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="70006-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="70006-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70006-139">createdDateTime</span></span>|<span data-ttu-id="70006-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70006-140">DateTimeOffset</span></span>|<span data-ttu-id="70006-141">Der Zeitpunkt, an die Bedingung Management erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="70006-141">The time the management condition was created.</span></span> <span data-ttu-id="70006-142">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="70006-142">Generated service side.</span></span>|
|<span data-ttu-id="70006-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70006-143">modifiedDateTime</span></span>|<span data-ttu-id="70006-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70006-144">DateTimeOffset</span></span>|<span data-ttu-id="70006-145">Die Zeit, die die Bedingung Management zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="70006-145">The time the management condition was last modified.</span></span> <span data-ttu-id="70006-146">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="70006-146">Updated service side.</span></span>|
|<span data-ttu-id="70006-147">eTag</span><span class="sxs-lookup"><span data-stu-id="70006-147">eTag</span></span>|<span data-ttu-id="70006-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70006-148">String</span></span>|<span data-ttu-id="70006-149">ETag der Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="70006-149">ETag of the management condition.</span></span> <span data-ttu-id="70006-150">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="70006-150">Updated service side.</span></span>|
|<span data-ttu-id="70006-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="70006-151">applicablePlatforms</span></span>|<span data-ttu-id="70006-152">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70006-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="70006-153">Die entsprechenden Plattformen für diese Bedingung Management.</span><span class="sxs-lookup"><span data-stu-id="70006-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70006-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="70006-154">Relationships</span></span>
|<span data-ttu-id="70006-155">Beziehung</span><span class="sxs-lookup"><span data-stu-id="70006-155">Relationship</span></span>|<span data-ttu-id="70006-156">Typ</span><span class="sxs-lookup"><span data-stu-id="70006-156">Type</span></span>|<span data-ttu-id="70006-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70006-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70006-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="70006-158">managementConditionStatements</span></span>|<span data-ttu-id="70006-159">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="70006-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="70006-160">Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="70006-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70006-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="70006-161">JSON Representation</span></span>
<span data-ttu-id="70006-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="70006-162">Here is a JSON representation of the resource.</span></span>
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




