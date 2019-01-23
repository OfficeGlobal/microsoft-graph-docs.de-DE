---
title: Ressourcentyp groupPolicyDefinitionFile
description: Die Entität stellt eine ADMX (ADM) XML-Datei. Die ADMX-Datei enthält eine Auflistung von Group Policy-Definitionen und deren Speicherorte nach Kategoriepfad. Die Gruppenrichtlinie-Definitionsdatei enthält auch die Sprachen unterstützt, wie durch die Sprachdateien abhängigen ADML (ADM) Sprache bestimmt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac5206321047dd4cd54732103e4adb70221e860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431531"
---
# <a name="grouppolicydefinitionfile-resource-type"></a><span data-ttu-id="da889-105">Ressourcentyp groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="da889-105">groupPolicyDefinitionFile resource type</span></span>

> <span data-ttu-id="da889-106">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="da889-106">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da889-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da889-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da889-108">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="da889-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da889-109">Die Entität stellt eine ADMX (ADM) XML-Datei.</span><span class="sxs-lookup"><span data-stu-id="da889-109">The entity represents an ADMX (Administrative Template) XML file.</span></span> <span data-ttu-id="da889-110">Die ADMX-Datei enthält eine Auflistung von Group Policy-Definitionen und deren Speicherorte nach Kategoriepfad.</span><span class="sxs-lookup"><span data-stu-id="da889-110">The ADMX file contains a collection of group policy definitions and their locations by category path.</span></span> <span data-ttu-id="da889-111">Die Gruppenrichtlinie-Definitionsdatei enthält auch die Sprachen unterstützt, wie durch die Sprachdateien abhängigen ADML (ADM) Sprache bestimmt.</span><span class="sxs-lookup"><span data-stu-id="da889-111">The group policy definition file also contains the languages supported as determined by the language dependent ADML (Administrative Template) language files.</span></span>

## <a name="methods"></a><span data-ttu-id="da889-112">Methoden</span><span class="sxs-lookup"><span data-stu-id="da889-112">Methods</span></span>
|<span data-ttu-id="da889-113">Methode</span><span class="sxs-lookup"><span data-stu-id="da889-113">Method</span></span>|<span data-ttu-id="da889-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="da889-114">Return Type</span></span>|<span data-ttu-id="da889-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da889-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="da889-116">Abrufen von groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="da889-116">Get groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[<span data-ttu-id="da889-117">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="da889-117">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="da889-118">Lesen Sie Eigenschaften und Beziehungen des [GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="da889-118">Read properties and relationships of the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|
|[<span data-ttu-id="da889-119">GroupPolicyDefinitionFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="da889-119">Update groupPolicyDefinitionFile</span></span>](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[<span data-ttu-id="da889-120">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="da889-120">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="da889-121">Aktualisieren Sie die Eigenschaften eines [GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="da889-121">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="da889-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="da889-122">Properties</span></span>
|<span data-ttu-id="da889-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da889-123">Property</span></span>|<span data-ttu-id="da889-124">Typ</span><span class="sxs-lookup"><span data-stu-id="da889-124">Type</span></span>|<span data-ttu-id="da889-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da889-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da889-126">displayName</span><span class="sxs-lookup"><span data-stu-id="da889-126">displayName</span></span>|<span data-ttu-id="da889-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da889-127">String</span></span>|<span data-ttu-id="da889-128">Die lokalisierten Anzeigenamen der ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="da889-128">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="da889-129">description</span><span class="sxs-lookup"><span data-stu-id="da889-129">description</span></span>|<span data-ttu-id="da889-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da889-130">String</span></span>|<span data-ttu-id="da889-131">Die lokalisierte Beschreibung der Richtlinieneinstellungen in der ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="da889-131">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="da889-132">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="da889-132">The default value is empty.</span></span>|
|<span data-ttu-id="da889-133">languageCodes</span><span class="sxs-lookup"><span data-stu-id="da889-133">languageCodes</span></span>|<span data-ttu-id="da889-134">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="da889-134">String collection</span></span>|<span data-ttu-id="da889-135">Die unterstützten Sprachcodes für die ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="da889-135">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="da889-136">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="da889-136">targetPrefix</span></span>|<span data-ttu-id="da889-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da889-137">String</span></span>|<span data-ttu-id="da889-138">Gibt den logischen Namen, der auf den Namespace innerhalb der ADMX-Datei verweist.</span><span class="sxs-lookup"><span data-stu-id="da889-138">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="da889-139">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="da889-139">targetNamespace</span></span>|<span data-ttu-id="da889-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da889-140">String</span></span>|<span data-ttu-id="da889-141">Gibt den URI verwendet, um den Namespace innerhalb der ADMX-Datei zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="da889-141">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="da889-142">policyType</span><span class="sxs-lookup"><span data-stu-id="da889-142">policyType</span></span>|[<span data-ttu-id="da889-143">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="da889-143">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="da889-144">Gibt den Typ von Gruppenrichtlinien.</span><span class="sxs-lookup"><span data-stu-id="da889-144">Specifies the type of group policy.</span></span> <span data-ttu-id="da889-145">Mögliche Werte sind: `admxBacked` und `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="da889-145">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="da889-146">id</span><span class="sxs-lookup"><span data-stu-id="da889-146">id</span></span>|<span data-ttu-id="da889-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da889-147">String</span></span>|<span data-ttu-id="da889-148">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="da889-148">Key of the entity.</span></span>|
|<span data-ttu-id="da889-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da889-149">lastModifiedDateTime</span></span>|<span data-ttu-id="da889-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da889-150">DateTimeOffset</span></span>|<span data-ttu-id="da889-151">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="da889-151">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da889-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="da889-152">Relationships</span></span>
|<span data-ttu-id="da889-153">Beziehung</span><span class="sxs-lookup"><span data-stu-id="da889-153">Relationship</span></span>|<span data-ttu-id="da889-154">Typ</span><span class="sxs-lookup"><span data-stu-id="da889-154">Type</span></span>|<span data-ttu-id="da889-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da889-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da889-156">Definitionen</span><span class="sxs-lookup"><span data-stu-id="da889-156">definitions</span></span>|<span data-ttu-id="da889-157">[GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="da889-157">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="da889-158">Der Gruppenrichtlinie Definitionen im Zusammenhang mit der Datei.</span><span class="sxs-lookup"><span data-stu-id="da889-158">The group policy definitions associated with the file.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da889-159">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="da889-159">JSON Representation</span></span>
<span data-ttu-id="da889-160">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="da889-160">Here is a JSON representation of the resource.</span></span>
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




