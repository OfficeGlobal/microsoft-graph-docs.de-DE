---
title: managedAppPolicy-Ressourcentyp
description: Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2615d1331c024c1a04bc7db618e36966cc5bcdff
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251167"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="7e1c6-103">managedAppPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7e1c6-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="7e1c6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7e1c6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e1c6-105">Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.</span><span class="sxs-lookup"><span data-stu-id="7e1c6-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="7e1c6-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="7e1c6-106">Methods</span></span>
|<span data-ttu-id="7e1c6-107">Methode</span><span class="sxs-lookup"><span data-stu-id="7e1c6-107">Method</span></span>|<span data-ttu-id="7e1c6-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7e1c6-108">Return Type</span></span>|<span data-ttu-id="7e1c6-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e1c6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e1c6-110">managedAppPolicies auflisten</span><span class="sxs-lookup"><span data-stu-id="7e1c6-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="7e1c6-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7e1c6-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="7e1c6-112">Auflisten von Eigenschaften und Beziehungen der [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="7e1c6-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="7e1c6-113">managedAppPolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="7e1c6-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="7e1c6-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="7e1c6-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="7e1c6-115">Lesen von Eigenschaften und Beziehungen des [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7e1c6-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="7e1c6-116">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="7e1c6-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="7e1c6-117">Keine</span><span class="sxs-lookup"><span data-stu-id="7e1c6-117">None</span></span>|<span data-ttu-id="7e1c6-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7e1c6-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7e1c6-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7e1c6-119">Properties</span></span>
|<span data-ttu-id="7e1c6-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e1c6-120">Property</span></span>|<span data-ttu-id="7e1c6-121">Typ</span><span class="sxs-lookup"><span data-stu-id="7e1c6-121">Type</span></span>|<span data-ttu-id="7e1c6-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e1c6-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e1c6-123">displayName</span><span class="sxs-lookup"><span data-stu-id="7e1c6-123">displayName</span></span>|<span data-ttu-id="7e1c6-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e1c6-124">String</span></span>|<span data-ttu-id="7e1c6-125">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="7e1c6-125">Policy display name.</span></span>|
|<span data-ttu-id="7e1c6-126">description</span><span class="sxs-lookup"><span data-stu-id="7e1c6-126">description</span></span>|<span data-ttu-id="7e1c6-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e1c6-127">String</span></span>|<span data-ttu-id="7e1c6-128">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="7e1c6-128">The policy's description.</span></span>|
|<span data-ttu-id="7e1c6-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e1c6-129">createdDateTime</span></span>|<span data-ttu-id="7e1c6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e1c6-130">DateTimeOffset</span></span>|<span data-ttu-id="7e1c6-131">Das Datum und die Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="7e1c6-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="7e1c6-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e1c6-132">lastModifiedDateTime</span></span>|<span data-ttu-id="7e1c6-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e1c6-133">DateTimeOffset</span></span>|<span data-ttu-id="7e1c6-134">Das Datum und die Uhrzeit der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="7e1c6-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="7e1c6-135">id</span><span class="sxs-lookup"><span data-stu-id="7e1c6-135">id</span></span>|<span data-ttu-id="7e1c6-136">string</span><span class="sxs-lookup"><span data-stu-id="7e1c6-136">String</span></span>|<span data-ttu-id="7e1c6-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7e1c6-137">Key of the entity.</span></span>|
|<span data-ttu-id="7e1c6-138">Version</span><span class="sxs-lookup"><span data-stu-id="7e1c6-138">version</span></span>|<span data-ttu-id="7e1c6-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e1c6-139">String</span></span>|<span data-ttu-id="7e1c6-140">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="7e1c6-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e1c6-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7e1c6-141">Relationships</span></span>
<span data-ttu-id="7e1c6-142">Keine</span><span class="sxs-lookup"><span data-stu-id="7e1c6-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e1c6-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7e1c6-143">JSON Representation</span></span>
<span data-ttu-id="7e1c6-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7e1c6-144">Here is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "version": "String"
}
```



