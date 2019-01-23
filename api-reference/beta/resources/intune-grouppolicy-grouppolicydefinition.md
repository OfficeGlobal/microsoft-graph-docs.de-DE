---
title: Ressourcentyp groupPolicyDefinition
description: Die Entität beschreibt alle Informationen über eine einzelne Gruppenrichtlinie.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 502312f7a39dd5dc93fd8e39203f56d47a9ebf27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430167"
---
# <a name="grouppolicydefinition-resource-type"></a><span data-ttu-id="53bfa-103">Ressourcentyp groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="53bfa-103">groupPolicyDefinition resource type</span></span>

> <span data-ttu-id="53bfa-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="53bfa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="53bfa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53bfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53bfa-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53bfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53bfa-107">Die Entität beschreibt alle Informationen über eine einzelne Gruppenrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="53bfa-107">The entity describes all of the information about a single group policy.</span></span>

## <a name="methods"></a><span data-ttu-id="53bfa-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="53bfa-108">Methods</span></span>
|<span data-ttu-id="53bfa-109">Methode</span><span class="sxs-lookup"><span data-stu-id="53bfa-109">Method</span></span>|<span data-ttu-id="53bfa-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="53bfa-110">Return Type</span></span>|<span data-ttu-id="53bfa-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53bfa-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53bfa-112">Abrufen von groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="53bfa-112">Get groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[<span data-ttu-id="53bfa-113">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="53bfa-113">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="53bfa-114">Lesen Sie Eigenschaften und Beziehungen des [GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="53bfa-114">Read properties and relationships of the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|
|[<span data-ttu-id="53bfa-115">GroupPolicyDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="53bfa-115">Update groupPolicyDefinition</span></span>](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[<span data-ttu-id="53bfa-116">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="53bfa-116">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="53bfa-117">Aktualisieren Sie die Eigenschaften eines [GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="53bfa-117">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="53bfa-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="53bfa-118">Properties</span></span>
|<span data-ttu-id="53bfa-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="53bfa-119">Property</span></span>|<span data-ttu-id="53bfa-120">Typ</span><span class="sxs-lookup"><span data-stu-id="53bfa-120">Type</span></span>|<span data-ttu-id="53bfa-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53bfa-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53bfa-122">classType</span><span class="sxs-lookup"><span data-stu-id="53bfa-122">classType</span></span>|[<span data-ttu-id="53bfa-123">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="53bfa-123">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="53bfa-124">Identifiziert den Typ von Gruppen, denen auf die Richtlinie angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="53bfa-124">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="53bfa-125">Mögliche Werte sind: `user`, `machine` und `both`.</span><span class="sxs-lookup"><span data-stu-id="53bfa-125">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="53bfa-126">displayName</span><span class="sxs-lookup"><span data-stu-id="53bfa-126">displayName</span></span>|<span data-ttu-id="53bfa-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53bfa-127">String</span></span>|<span data-ttu-id="53bfa-128">Die lokalisierten Richtliniennamen.</span><span class="sxs-lookup"><span data-stu-id="53bfa-128">The localized policy name.</span></span>|
|<span data-ttu-id="53bfa-129">explainText</span><span class="sxs-lookup"><span data-stu-id="53bfa-129">explainText</span></span>|<span data-ttu-id="53bfa-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53bfa-130">String</span></span>|<span data-ttu-id="53bfa-131">Die lokalisierten Erläuterung oder Hilfe Text mit der Richtlinie verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="53bfa-131">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="53bfa-132">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="53bfa-132">The default value is empty.</span></span>|
|<span data-ttu-id="53bfa-133">categoryPath</span><span class="sxs-lookup"><span data-stu-id="53bfa-133">categoryPath</span></span>|<span data-ttu-id="53bfa-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53bfa-134">String</span></span>|<span data-ttu-id="53bfa-135">Der Pfad der lokalisierte vollständige Kategorie für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="53bfa-135">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="53bfa-136">supportedOn</span><span class="sxs-lookup"><span data-stu-id="53bfa-136">supportedOn</span></span>|<span data-ttu-id="53bfa-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53bfa-137">String</span></span>|<span data-ttu-id="53bfa-138">Lokalisierte Zeichenfolge verwendet, um anzugeben, welche Version der Anwendung oder das Betriebssystem durch die Richtlinie betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="53bfa-138">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="53bfa-139">policyType</span><span class="sxs-lookup"><span data-stu-id="53bfa-139">policyType</span></span>|[<span data-ttu-id="53bfa-140">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="53bfa-140">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="53bfa-141">Gibt den Typ von Gruppenrichtlinien.</span><span class="sxs-lookup"><span data-stu-id="53bfa-141">Specifies the type of group policy.</span></span> <span data-ttu-id="53bfa-142">Mögliche Werte sind: `admxBacked` und `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="53bfa-142">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="53bfa-143">id</span><span class="sxs-lookup"><span data-stu-id="53bfa-143">id</span></span>|<span data-ttu-id="53bfa-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53bfa-144">String</span></span>|<span data-ttu-id="53bfa-145">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="53bfa-145">Key of the entity.</span></span>|
|<span data-ttu-id="53bfa-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53bfa-146">lastModifiedDateTime</span></span>|<span data-ttu-id="53bfa-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53bfa-147">DateTimeOffset</span></span>|<span data-ttu-id="53bfa-148">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="53bfa-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53bfa-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="53bfa-149">Relationships</span></span>
|<span data-ttu-id="53bfa-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="53bfa-150">Relationship</span></span>|<span data-ttu-id="53bfa-151">Typ</span><span class="sxs-lookup"><span data-stu-id="53bfa-151">Type</span></span>|<span data-ttu-id="53bfa-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53bfa-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53bfa-153">­DefinitionFile</span><span class="sxs-lookup"><span data-stu-id="53bfa-153">definitionFile</span></span>|[<span data-ttu-id="53bfa-154">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="53bfa-154">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="53bfa-155">Die Gruppe Richtliniendatei für die Definition zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="53bfa-155">The group policy file associated with the definition.</span></span>|
|<span data-ttu-id="53bfa-156">Präsentationen</span><span class="sxs-lookup"><span data-stu-id="53bfa-156">presentations</span></span>|<span data-ttu-id="53bfa-157">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="53bfa-157">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) collection</span></span>|<span data-ttu-id="53bfa-158">Die Gruppenrichtlinie Präsentationen mit der Definition von verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="53bfa-158">The group policy presentations associated with the definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53bfa-159">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="53bfa-159">JSON Representation</span></span>
<span data-ttu-id="53bfa-160">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="53bfa-160">Here is a JSON representation of the resource.</span></span>
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




