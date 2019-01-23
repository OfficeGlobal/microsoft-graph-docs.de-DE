---
title: Ressourcentyp groupPolicyConfiguration
description: Die Gruppenrichtlinie Konfigurationsentität enthält die konfigurierten Werte für eine oder mehrere Group Policy-Definitionen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be3b43ab0e9e3f87f53ed0dae144f2b6f4dce7b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431575"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="693b4-103">Ressourcentyp groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="693b4-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="693b4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="693b4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="693b4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="693b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="693b4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="693b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="693b4-107">Die Gruppenrichtlinie Konfigurationsentität enthält die konfigurierten Werte für eine oder mehrere Group Policy-Definitionen.</span><span class="sxs-lookup"><span data-stu-id="693b4-107">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="693b4-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="693b4-108">Methods</span></span>
|<span data-ttu-id="693b4-109">Methode</span><span class="sxs-lookup"><span data-stu-id="693b4-109">Method</span></span>|<span data-ttu-id="693b4-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="693b4-110">Return Type</span></span>|<span data-ttu-id="693b4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="693b4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="693b4-112">Liste groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="693b4-112">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="693b4-113">[GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="693b4-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="693b4-114">Listeneigenschaften und Beziehungen der [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="693b4-114">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="693b4-115">Abrufen von groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="693b4-115">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="693b4-116">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="693b4-116">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="693b4-117">Lesen Sie Eigenschaften und Beziehungen des [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="693b4-117">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="693b4-118">Erstellen von groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="693b4-118">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="693b4-119">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="693b4-119">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="693b4-120">Erstellen eines neuen [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="693b4-120">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="693b4-121">GroupPolicyConfiguration löschen</span><span class="sxs-lookup"><span data-stu-id="693b4-121">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="693b4-122">Keine</span><span class="sxs-lookup"><span data-stu-id="693b4-122">None</span></span>|<span data-ttu-id="693b4-123">Löscht eine [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="693b4-123">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="693b4-124">GroupPolicyConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="693b4-124">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="693b4-125">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="693b4-125">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="693b4-126">Aktualisieren Sie die Eigenschaften eines [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="693b4-126">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="693b4-127">assign-Aktion</span><span class="sxs-lookup"><span data-stu-id="693b4-127">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="693b4-128">[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="693b4-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="693b4-129">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="693b4-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="693b4-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="693b4-130">Properties</span></span>
|<span data-ttu-id="693b4-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="693b4-131">Property</span></span>|<span data-ttu-id="693b4-132">Typ</span><span class="sxs-lookup"><span data-stu-id="693b4-132">Type</span></span>|<span data-ttu-id="693b4-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="693b4-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="693b4-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="693b4-134">createdDateTime</span></span>|<span data-ttu-id="693b4-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="693b4-135">DateTimeOffset</span></span>|<span data-ttu-id="693b4-136">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="693b4-136">The date and time the object was created.</span></span>|
|<span data-ttu-id="693b4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="693b4-137">displayName</span></span>|<span data-ttu-id="693b4-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="693b4-138">String</span></span>|<span data-ttu-id="693b4-139">Der vom Benutzer bereitgestellte Name für das Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="693b4-139">User provided name for the resource object.</span></span>|
|<span data-ttu-id="693b4-140">description</span><span class="sxs-lookup"><span data-stu-id="693b4-140">description</span></span>|<span data-ttu-id="693b4-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="693b4-141">String</span></span>|<span data-ttu-id="693b4-142">Vom Benutzer bereitgestellte Beschreibung für das Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="693b4-142">User provided description for the resource object.</span></span>|
|<span data-ttu-id="693b4-143">id</span><span class="sxs-lookup"><span data-stu-id="693b4-143">id</span></span>|<span data-ttu-id="693b4-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="693b4-144">String</span></span>|<span data-ttu-id="693b4-145">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="693b4-145">Key of the entity.</span></span>|
|<span data-ttu-id="693b4-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="693b4-146">lastModifiedDateTime</span></span>|<span data-ttu-id="693b4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="693b4-147">DateTimeOffset</span></span>|<span data-ttu-id="693b4-148">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="693b4-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="693b4-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="693b4-149">Relationships</span></span>
|<span data-ttu-id="693b4-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="693b4-150">Relationship</span></span>|<span data-ttu-id="693b4-151">Typ</span><span class="sxs-lookup"><span data-stu-id="693b4-151">Type</span></span>|<span data-ttu-id="693b4-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="693b4-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="693b4-153">definitionValues</span><span class="sxs-lookup"><span data-stu-id="693b4-153">definitionValues</span></span>|<span data-ttu-id="693b4-154">[GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="693b4-154">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="693b4-155">Die Liste der aktiviert oder deaktiviert Group Policy Definition Werte für die Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="693b4-155">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="693b4-156">assignments</span><span class="sxs-lookup"><span data-stu-id="693b4-156">assignments</span></span>|<span data-ttu-id="693b4-157">[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="693b4-157">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="693b4-158">Die Liste der Gruppe Aufgaben für die Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="693b4-158">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="693b4-159">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="693b4-159">JSON Representation</span></span>
<span data-ttu-id="693b4-160">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="693b4-160">Here is a JSON representation of the resource.</span></span>
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




