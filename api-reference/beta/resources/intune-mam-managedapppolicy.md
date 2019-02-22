---
title: managedAppPolicy-Ressourcentyp
description: Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e98735a03583fef25fc460c6f989a5a7edf9b44
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144023"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="2c0d6-103">managedAppPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2c0d6-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="2c0d6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2c0d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c0d6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2c0d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c0d6-106">Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.</span><span class="sxs-lookup"><span data-stu-id="2c0d6-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="2c0d6-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="2c0d6-107">Methods</span></span>
|<span data-ttu-id="2c0d6-108">Methode</span><span class="sxs-lookup"><span data-stu-id="2c0d6-108">Method</span></span>|<span data-ttu-id="2c0d6-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2c0d6-109">Return Type</span></span>|<span data-ttu-id="2c0d6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c0d6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2c0d6-111">managedAppPolicies auflisten</span><span class="sxs-lookup"><span data-stu-id="2c0d6-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="2c0d6-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2c0d6-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2c0d6-113">Auflisten von Eigenschaften und Beziehungen der [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="2c0d6-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="2c0d6-114">managedAppPolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="2c0d6-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="2c0d6-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2c0d6-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="2c0d6-116">Lesen von Eigenschaften und Beziehungen des [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2c0d6-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="2c0d6-117">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="2c0d6-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="2c0d6-118">Keine</span><span class="sxs-lookup"><span data-stu-id="2c0d6-118">None</span></span>|<span data-ttu-id="2c0d6-119">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2c0d6-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2c0d6-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2c0d6-120">Properties</span></span>
|<span data-ttu-id="2c0d6-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c0d6-121">Property</span></span>|<span data-ttu-id="2c0d6-122">Typ</span><span class="sxs-lookup"><span data-stu-id="2c0d6-122">Type</span></span>|<span data-ttu-id="2c0d6-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c0d6-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c0d6-124">displayName</span><span class="sxs-lookup"><span data-stu-id="2c0d6-124">displayName</span></span>|<span data-ttu-id="2c0d6-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2c0d6-125">String</span></span>|<span data-ttu-id="2c0d6-126">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2c0d6-126">Policy display name.</span></span>|
|<span data-ttu-id="2c0d6-127">description</span><span class="sxs-lookup"><span data-stu-id="2c0d6-127">description</span></span>|<span data-ttu-id="2c0d6-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2c0d6-128">String</span></span>|<span data-ttu-id="2c0d6-129">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2c0d6-129">The policy's description.</span></span>|
|<span data-ttu-id="2c0d6-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c0d6-130">createdDateTime</span></span>|<span data-ttu-id="2c0d6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c0d6-131">DateTimeOffset</span></span>|<span data-ttu-id="2c0d6-132">Das Datum und die Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="2c0d6-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="2c0d6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c0d6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2c0d6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c0d6-134">DateTimeOffset</span></span>|<span data-ttu-id="2c0d6-135">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2c0d6-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="2c0d6-136">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="2c0d6-136">roleScopeTagIds</span></span>|<span data-ttu-id="2c0d6-137">String collection</span><span class="sxs-lookup"><span data-stu-id="2c0d6-137">String collection</span></span>|<span data-ttu-id="2c0d6-138">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="2c0d6-138">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="2c0d6-139">id</span><span class="sxs-lookup"><span data-stu-id="2c0d6-139">id</span></span>|<span data-ttu-id="2c0d6-140">string</span><span class="sxs-lookup"><span data-stu-id="2c0d6-140">String</span></span>|<span data-ttu-id="2c0d6-141">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2c0d6-141">Key of the entity.</span></span>|
|<span data-ttu-id="2c0d6-142">Version</span><span class="sxs-lookup"><span data-stu-id="2c0d6-142">version</span></span>|<span data-ttu-id="2c0d6-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2c0d6-143">String</span></span>|<span data-ttu-id="2c0d6-144">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="2c0d6-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c0d6-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2c0d6-145">Relationships</span></span>
<span data-ttu-id="2c0d6-146">Keine</span><span class="sxs-lookup"><span data-stu-id="2c0d6-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c0d6-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2c0d6-147">JSON Representation</span></span>
<span data-ttu-id="2c0d6-148">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2c0d6-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String"
}
```




