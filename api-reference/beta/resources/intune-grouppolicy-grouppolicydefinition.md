---
title: groupPolicyDefinition-Ressourcentyp
description: Die Entität beschreibt alle Informationen zu einer einzelnen Gruppenrichtlinie.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c5062fda984dbe1dda518e77ff271750d30adb8
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644286"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="9ef6e-103">groupPolicyDefinition-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9ef6e-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="9ef6e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ef6e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ef6e-106">Die Entität beschreibt alle Informationen zu einer einzelnen Gruppenrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-106">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="9ef6e-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="9ef6e-107">Methods</span></span>
|<span data-ttu-id="9ef6e-108">Methode</span><span class="sxs-lookup"><span data-stu-id="9ef6e-108">Method</span></span>|<span data-ttu-id="9ef6e-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9ef6e-109">Return Type</span></span>|<span data-ttu-id="9ef6e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ef6e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ef6e-111">GroupPolicyDefinition abrufen</span><span class="sxs-lookup"><span data-stu-id="9ef6e-111">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="9ef6e-112">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9ef6e-112">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9ef6e-113">Lesen von Eigenschaften und Beziehungen des [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-113">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="9ef6e-114">GroupPolicyDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9ef6e-114">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="9ef6e-115">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9ef6e-115">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9ef6e-116">Aktualisieren der Eigenschaften eines [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-116">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ef6e-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9ef6e-117">Properties</span></span>
|<span data-ttu-id="9ef6e-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ef6e-118">Property</span></span>|<span data-ttu-id="9ef6e-119">Typ</span><span class="sxs-lookup"><span data-stu-id="9ef6e-119">Type</span></span>|<span data-ttu-id="9ef6e-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ef6e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef6e-121">classType</span><span class="sxs-lookup"><span data-stu-id="9ef6e-121">classType</span></span>|[<span data-ttu-id="9ef6e-122">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="9ef6e-122">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="9ef6e-123">Gibt den Typ der Gruppen an, auf die die Richtlinie angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-123">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="9ef6e-124">Mögliche Werte sind: `user` und `machine`.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-124">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="9ef6e-125">displayName</span><span class="sxs-lookup"><span data-stu-id="9ef6e-125">displayName</span></span>|<span data-ttu-id="9ef6e-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ef6e-126">String</span></span>|<span data-ttu-id="9ef6e-127">Der Name der lokalisierten Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-127">The localized policy name.</span></span>|
|<span data-ttu-id="9ef6e-128">explainText</span><span class="sxs-lookup"><span data-stu-id="9ef6e-128">explainText</span></span>|<span data-ttu-id="9ef6e-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ef6e-129">String</span></span>|<span data-ttu-id="9ef6e-130">Die lokalisierte Erläuterung oder der Hilfe Text, der der Richtlinie zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-130">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="9ef6e-131">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-131">The default value is empty.</span></span>|
|<span data-ttu-id="9ef6e-132">categoryPath</span><span class="sxs-lookup"><span data-stu-id="9ef6e-132">categoryPath</span></span>|<span data-ttu-id="9ef6e-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ef6e-133">String</span></span>|<span data-ttu-id="9ef6e-134">Der lokalisierte vollständige Kategorie-Pfad für die Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-134">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="9ef6e-135">supportedOn</span><span class="sxs-lookup"><span data-stu-id="9ef6e-135">supportedOn</span></span>|<span data-ttu-id="9ef6e-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ef6e-136">String</span></span>|<span data-ttu-id="9ef6e-137">Lokalisierte Zeichenfolge, die verwendet wird, um anzugeben, welche Betriebssystem-oder Anwendungsversion von der Richtlinie betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-137">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="9ef6e-138">policyType</span><span class="sxs-lookup"><span data-stu-id="9ef6e-138">policyType</span></span>|[<span data-ttu-id="9ef6e-139">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="9ef6e-139">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="9ef6e-140">Gibt den Typ der Gruppenrichtlinie an.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-140">Specifies the type of group policy.</span></span> <span data-ttu-id="9ef6e-141">Mögliche Werte: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-141">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="9ef6e-142">id</span><span class="sxs-lookup"><span data-stu-id="9ef6e-142">id</span></span>|<span data-ttu-id="9ef6e-143">String</span><span class="sxs-lookup"><span data-stu-id="9ef6e-143">String</span></span>|<span data-ttu-id="9ef6e-144">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9ef6e-144">Key of the entity.</span></span>|
|<span data-ttu-id="9ef6e-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ef6e-145">lastModifiedDateTime</span></span>|<span data-ttu-id="9ef6e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ef6e-146">DateTimeOffset</span></span>|<span data-ttu-id="9ef6e-147">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ef6e-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9ef6e-148">Relationships</span></span>
|<span data-ttu-id="9ef6e-149">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9ef6e-149">Relationship</span></span>|<span data-ttu-id="9ef6e-150">Typ</span><span class="sxs-lookup"><span data-stu-id="9ef6e-150">Type</span></span>|<span data-ttu-id="9ef6e-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ef6e-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef6e-152">definitionFile</span><span class="sxs-lookup"><span data-stu-id="9ef6e-152">definitionFile</span></span>|[<span data-ttu-id="9ef6e-153">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="9ef6e-153">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="9ef6e-154">Die der Definition zugeordnete Gruppenrichtliniendatei.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-154">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="9ef6e-155">Präsentationen</span><span class="sxs-lookup"><span data-stu-id="9ef6e-155">presentations</span></span>|<span data-ttu-id="9ef6e-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="9ef6e-156">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="9ef6e-157">Die der Definition zugeordneten Gruppenrichtlinien Präsentationen.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-157">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ef6e-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9ef6e-158">JSON Representation</span></span>
<span data-ttu-id="9ef6e-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9ef6e-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




