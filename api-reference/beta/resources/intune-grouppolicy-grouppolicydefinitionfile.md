---
title: groupPolicyDefinitionFile-Ressourcentyp
description: Die Entität stellt eine ADMX-XML-Datei (administrative Vorlage) dar. Die ADMX-Datei enthält eine Sammlung von Gruppenrichtlinien Definitionen und ihre Standorte nach Kategorie-Pfad. Die Gruppenrichtlinien-Definitionsdatei enthält auch die unterstützten Sprachen, die von den sprachabhängigen Sprachdateien der ADML (administrative Template) bestimmt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 494a2f8ff80b3a7f8ee9db9fea4d795494c19a92
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161334"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="e8c43-105">groupPolicyDefinitionFile-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e8c43-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="e8c43-106">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e8c43-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8c43-107">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e8c43-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8c43-108">Die Entität stellt eine ADMX-XML-Datei (administrative Vorlage) dar.</span><span class="sxs-lookup"><span data-stu-id="e8c43-108">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="e8c43-109">Die ADMX-Datei enthält eine Sammlung von Gruppenrichtlinien Definitionen und ihre Standorte nach Kategorie-Pfad.</span><span class="sxs-lookup"><span data-stu-id="e8c43-109">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="e8c43-110">Die Gruppenrichtlinien-Definitionsdatei enthält auch die unterstützten Sprachen, die von den sprachabhängigen Sprachdateien der ADML (administrative Template) bestimmt werden.</span><span class="sxs-lookup"><span data-stu-id="e8c43-110">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="e8c43-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="e8c43-111">Methods</span></span>
|<span data-ttu-id="e8c43-112">Methode</span><span class="sxs-lookup"><span data-stu-id="e8c43-112">Method</span></span>|<span data-ttu-id="e8c43-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e8c43-113">Return Type</span></span>|<span data-ttu-id="e8c43-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8c43-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e8c43-115">GroupPolicyDefinitionFile abrufen</span><span class="sxs-lookup"><span data-stu-id="e8c43-115">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="e8c43-116">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="e8c43-116">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="e8c43-117">Lesen von Eigenschaften und Beziehungen des [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8c43-117">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="e8c43-118">GroupPolicyDefinitionFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e8c43-118">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="e8c43-119">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="e8c43-119">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="e8c43-120">Aktualisieren der Eigenschaften eines [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8c43-120">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8c43-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e8c43-121">Properties</span></span>
|<span data-ttu-id="e8c43-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e8c43-122">Property</span></span>|<span data-ttu-id="e8c43-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e8c43-123">Type</span></span>|<span data-ttu-id="e8c43-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8c43-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8c43-125">displayName</span><span class="sxs-lookup"><span data-stu-id="e8c43-125">displayName</span></span>|<span data-ttu-id="e8c43-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8c43-126">String</span></span>|<span data-ttu-id="e8c43-127">Der lokalisierte Anzeigename der ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="e8c43-127">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="e8c43-128">description</span><span class="sxs-lookup"><span data-stu-id="e8c43-128">description</span></span>|<span data-ttu-id="e8c43-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8c43-129">String</span></span>|<span data-ttu-id="e8c43-130">Die lokalisierte Beschreibung der Richtlinieneinstellungen in der ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="e8c43-130">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="e8c43-131">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="e8c43-131">The default value is empty.</span></span>|
|<span data-ttu-id="e8c43-132">languageCodes</span><span class="sxs-lookup"><span data-stu-id="e8c43-132">languageCodes</span></span>|<span data-ttu-id="e8c43-133">String collection</span><span class="sxs-lookup"><span data-stu-id="e8c43-133">String collection</span></span>|<span data-ttu-id="e8c43-134">Die unterstützten Sprachcodes für die ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="e8c43-134">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="e8c43-135">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="e8c43-135">targetPrefix</span></span>|<span data-ttu-id="e8c43-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8c43-136">String</span></span>|<span data-ttu-id="e8c43-137">Gibt den logischen Namen an, der auf den Namespace innerhalb der ADMX-Datei verweist.</span><span class="sxs-lookup"><span data-stu-id="e8c43-137">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="e8c43-138">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="e8c43-138">targetNamespace</span></span>|<span data-ttu-id="e8c43-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8c43-139">String</span></span>|<span data-ttu-id="e8c43-140">Gibt den URI an, der zum Identifizieren des Namespaces innerhalb der ADMX-Datei verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e8c43-140">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="e8c43-141">policyType</span><span class="sxs-lookup"><span data-stu-id="e8c43-141">policyType</span></span>|[<span data-ttu-id="e8c43-142">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="e8c43-142">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="e8c43-143">Gibt den Typ der Gruppenrichtlinie an.</span><span class="sxs-lookup"><span data-stu-id="e8c43-143">Specifies the type of group policy.</span></span> <span data-ttu-id="e8c43-144">Mögliche Werte sind: `admxBacked` und `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="e8c43-144">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="e8c43-145">id</span><span class="sxs-lookup"><span data-stu-id="e8c43-145">id</span></span>|<span data-ttu-id="e8c43-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8c43-146">String</span></span>|<span data-ttu-id="e8c43-147">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e8c43-147">Key of the entity.</span></span>|
|<span data-ttu-id="e8c43-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8c43-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e8c43-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8c43-149">DateTimeOffset</span></span>|<span data-ttu-id="e8c43-150">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="e8c43-150">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8c43-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e8c43-151">Relationships</span></span>
|<span data-ttu-id="e8c43-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e8c43-152">Relationship</span></span>|<span data-ttu-id="e8c43-153">Typ</span><span class="sxs-lookup"><span data-stu-id="e8c43-153">Type</span></span>|<span data-ttu-id="e8c43-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8c43-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8c43-155">Definitionen</span><span class="sxs-lookup"><span data-stu-id="e8c43-155">definitions</span></span>|<span data-ttu-id="e8c43-156">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="e8c43-156">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="e8c43-157">Die der Datei zugeordneten Gruppenrichtlinien Definitionen.</span><span class="sxs-lookup"><span data-stu-id="e8c43-157">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8c43-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e8c43-158">JSON Representation</span></span>
<span data-ttu-id="e8c43-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e8c43-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




