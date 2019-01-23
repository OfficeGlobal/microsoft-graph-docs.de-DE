---
title: managedAppPolicy-Ressourcentyp
description: Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6bc4a7bbc4bc0dc85da8759ad95162712b1deb13
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422978"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="662f9-103">managedAppPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="662f9-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="662f9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="662f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="662f9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="662f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="662f9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="662f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="662f9-107">Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.</span><span class="sxs-lookup"><span data-stu-id="662f9-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="662f9-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="662f9-108">Methods</span></span>
|<span data-ttu-id="662f9-109">Methode</span><span class="sxs-lookup"><span data-stu-id="662f9-109">Method</span></span>|<span data-ttu-id="662f9-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="662f9-110">Return Type</span></span>|<span data-ttu-id="662f9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="662f9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="662f9-112">managedAppPolicies auflisten</span><span class="sxs-lookup"><span data-stu-id="662f9-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="662f9-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="662f9-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="662f9-114">Auflisten von Eigenschaften und Beziehungen der [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="662f9-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="662f9-115">managedAppPolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="662f9-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="662f9-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="662f9-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="662f9-117">Lesen von Eigenschaften und Beziehungen des [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="662f9-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="662f9-118">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="662f9-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="662f9-119">Keine</span><span class="sxs-lookup"><span data-stu-id="662f9-119">None</span></span>|<span data-ttu-id="662f9-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="662f9-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="662f9-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="662f9-121">Properties</span></span>
|<span data-ttu-id="662f9-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="662f9-122">Property</span></span>|<span data-ttu-id="662f9-123">Typ</span><span class="sxs-lookup"><span data-stu-id="662f9-123">Type</span></span>|<span data-ttu-id="662f9-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="662f9-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="662f9-125">displayName</span><span class="sxs-lookup"><span data-stu-id="662f9-125">displayName</span></span>|<span data-ttu-id="662f9-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="662f9-126">String</span></span>|<span data-ttu-id="662f9-127">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="662f9-127">Policy display name.</span></span>|
|<span data-ttu-id="662f9-128">description</span><span class="sxs-lookup"><span data-stu-id="662f9-128">description</span></span>|<span data-ttu-id="662f9-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="662f9-129">String</span></span>|<span data-ttu-id="662f9-130">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="662f9-130">The policy's description.</span></span>|
|<span data-ttu-id="662f9-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="662f9-131">createdDateTime</span></span>|<span data-ttu-id="662f9-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="662f9-132">DateTimeOffset</span></span>|<span data-ttu-id="662f9-133">Das Datum und die Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="662f9-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="662f9-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="662f9-134">lastModifiedDateTime</span></span>|<span data-ttu-id="662f9-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="662f9-135">DateTimeOffset</span></span>|<span data-ttu-id="662f9-136">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="662f9-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="662f9-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="662f9-137">roleScopeTagIds</span></span>|<span data-ttu-id="662f9-138">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="662f9-138">String collection</span></span>|<span data-ttu-id="662f9-139">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="662f9-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="662f9-140">id</span><span class="sxs-lookup"><span data-stu-id="662f9-140">id</span></span>|<span data-ttu-id="662f9-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="662f9-141">String</span></span>|<span data-ttu-id="662f9-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="662f9-142">Key of the entity.</span></span>|
|<span data-ttu-id="662f9-143">Version</span><span class="sxs-lookup"><span data-stu-id="662f9-143">version</span></span>|<span data-ttu-id="662f9-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="662f9-144">String</span></span>|<span data-ttu-id="662f9-145">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="662f9-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="662f9-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="662f9-146">Relationships</span></span>
<span data-ttu-id="662f9-147">Keine</span><span class="sxs-lookup"><span data-stu-id="662f9-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="662f9-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="662f9-148">JSON Representation</span></span>
<span data-ttu-id="662f9-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="662f9-149">Here is a JSON representation of the resource.</span></span>
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




