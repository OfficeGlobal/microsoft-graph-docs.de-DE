---
title: groupPolicyConfiguration-Ressourcentyp
description: Die Gruppenrichtlinien-Konfigurationsentität enthält die konfigurierten Werte für eine oder mehrere Gruppenrichtlinien Definitionen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 540da94d92f3056a6699b7112f3589f6da4b7144
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160753"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="6c4fe-103">groupPolicyConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6c4fe-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="6c4fe-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c4fe-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c4fe-106">Die Gruppenrichtlinien-Konfigurationsentität enthält die konfigurierten Werte für eine oder mehrere Gruppenrichtlinien Definitionen.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="6c4fe-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="6c4fe-107">Methods</span></span>
|<span data-ttu-id="6c4fe-108">Methode</span><span class="sxs-lookup"><span data-stu-id="6c4fe-108">Method</span></span>|<span data-ttu-id="6c4fe-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6c4fe-109">Return Type</span></span>|<span data-ttu-id="6c4fe-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c4fe-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c4fe-111">GroupPolicyConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="6c4fe-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="6c4fe-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="6c4fe-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="6c4fe-113">AufListen von Eigenschaften und Beziehungen der [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6c4fe-114">GroupPolicyConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="6c4fe-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="6c4fe-115">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c4fe-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="6c4fe-116">Lesen von Eigenschaften und Beziehungen des [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6c4fe-117">GroupPolicyConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="6c4fe-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="6c4fe-118">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c4fe-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="6c4fe-119">Erstellen eines neuen [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6c4fe-120">GroupPolicyConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="6c4fe-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="6c4fe-121">Keine</span><span class="sxs-lookup"><span data-stu-id="6c4fe-121">None</span></span>|<span data-ttu-id="6c4fe-122">Löscht eine [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c4fe-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="6c4fe-123">GroupPolicyConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6c4fe-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="6c4fe-124">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c4fe-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="6c4fe-125">Aktualisieren der Eigenschaften eines [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6c4fe-126">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="6c4fe-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="6c4fe-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="6c4fe-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6c4fe-128">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6c4fe-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6c4fe-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6c4fe-129">Properties</span></span>
|<span data-ttu-id="6c4fe-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c4fe-130">Property</span></span>|<span data-ttu-id="6c4fe-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6c4fe-131">Type</span></span>|<span data-ttu-id="6c4fe-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c4fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c4fe-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c4fe-133">createdDateTime</span></span>|<span data-ttu-id="6c4fe-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c4fe-134">DateTimeOffset</span></span>|<span data-ttu-id="6c4fe-135">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="6c4fe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6c4fe-136">displayName</span></span>|<span data-ttu-id="6c4fe-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c4fe-137">String</span></span>|<span data-ttu-id="6c4fe-138">Vom Benutzer bereitgestellter Name für das Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="6c4fe-139">description</span><span class="sxs-lookup"><span data-stu-id="6c4fe-139">description</span></span>|<span data-ttu-id="6c4fe-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c4fe-140">String</span></span>|<span data-ttu-id="6c4fe-141">Vom Benutzer bereitgestellte Beschreibung für das Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="6c4fe-142">id</span><span class="sxs-lookup"><span data-stu-id="6c4fe-142">id</span></span>|<span data-ttu-id="6c4fe-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c4fe-143">String</span></span>|<span data-ttu-id="6c4fe-144">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6c4fe-144">Key of the entity.</span></span>|
|<span data-ttu-id="6c4fe-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c4fe-145">lastModifiedDateTime</span></span>|<span data-ttu-id="6c4fe-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c4fe-146">DateTimeOffset</span></span>|<span data-ttu-id="6c4fe-147">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c4fe-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6c4fe-148">Relationships</span></span>
|<span data-ttu-id="6c4fe-149">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6c4fe-149">Relationship</span></span>|<span data-ttu-id="6c4fe-150">Typ</span><span class="sxs-lookup"><span data-stu-id="6c4fe-150">Type</span></span>|<span data-ttu-id="6c4fe-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c4fe-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c4fe-152">definitionValues</span><span class="sxs-lookup"><span data-stu-id="6c4fe-152">definitionValues</span></span>|<span data-ttu-id="6c4fe-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="6c4fe-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="6c4fe-154">Die Liste der aktivierten oder deaktivierten Gruppenrichtlinien definitionswerte für die Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="6c4fe-155">assignments</span><span class="sxs-lookup"><span data-stu-id="6c4fe-155">assignments</span></span>|<span data-ttu-id="6c4fe-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="6c4fe-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6c4fe-157">Die Liste der Gruppenzuweisungen für die Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c4fe-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6c4fe-158">JSON Representation</span></span>
<span data-ttu-id="6c4fe-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6c4fe-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




