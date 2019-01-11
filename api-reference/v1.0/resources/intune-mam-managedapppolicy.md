---
title: managedAppPolicy-Ressourcentyp
description: Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5766e3a467a157bac0d876fd0178dc3ba1cb94e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888081"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="43a2e-103">managedAppPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="43a2e-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="43a2e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="43a2e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43a2e-105">Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.</span><span class="sxs-lookup"><span data-stu-id="43a2e-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="43a2e-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="43a2e-106">Methods</span></span>
|<span data-ttu-id="43a2e-107">Methode</span><span class="sxs-lookup"><span data-stu-id="43a2e-107">Method</span></span>|<span data-ttu-id="43a2e-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="43a2e-108">Return Type</span></span>|<span data-ttu-id="43a2e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43a2e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="43a2e-110">managedAppPolicies auflisten</span><span class="sxs-lookup"><span data-stu-id="43a2e-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="43a2e-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="43a2e-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="43a2e-112">Auflisten von Eigenschaften und Beziehungen der [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="43a2e-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="43a2e-113">managedAppPolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="43a2e-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="43a2e-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="43a2e-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="43a2e-115">Lesen von Eigenschaften und Beziehungen des [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="43a2e-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="43a2e-116">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="43a2e-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="43a2e-117">Keine</span><span class="sxs-lookup"><span data-stu-id="43a2e-117">None</span></span>|<span data-ttu-id="43a2e-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="43a2e-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="43a2e-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="43a2e-119">Properties</span></span>
|<span data-ttu-id="43a2e-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43a2e-120">Property</span></span>|<span data-ttu-id="43a2e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="43a2e-121">Type</span></span>|<span data-ttu-id="43a2e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43a2e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43a2e-123">displayName</span><span class="sxs-lookup"><span data-stu-id="43a2e-123">displayName</span></span>|<span data-ttu-id="43a2e-124">String</span><span class="sxs-lookup"><span data-stu-id="43a2e-124">String</span></span>|<span data-ttu-id="43a2e-125">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="43a2e-125">Policy display name.</span></span>|
|<span data-ttu-id="43a2e-126">description</span><span class="sxs-lookup"><span data-stu-id="43a2e-126">description</span></span>|<span data-ttu-id="43a2e-127">String</span><span class="sxs-lookup"><span data-stu-id="43a2e-127">String</span></span>|<span data-ttu-id="43a2e-128">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="43a2e-128">The policy's description.</span></span>|
|<span data-ttu-id="43a2e-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43a2e-129">createdDateTime</span></span>|<span data-ttu-id="43a2e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43a2e-130">DateTimeOffset</span></span>|<span data-ttu-id="43a2e-131">Das Datum und die Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="43a2e-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="43a2e-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43a2e-132">lastModifiedDateTime</span></span>|<span data-ttu-id="43a2e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43a2e-133">DateTimeOffset</span></span>|<span data-ttu-id="43a2e-134">Das Datum und die Uhrzeit der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="43a2e-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="43a2e-135">id</span><span class="sxs-lookup"><span data-stu-id="43a2e-135">id</span></span>|<span data-ttu-id="43a2e-136">String</span><span class="sxs-lookup"><span data-stu-id="43a2e-136">String</span></span>|<span data-ttu-id="43a2e-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="43a2e-137">Key of the entity.</span></span>|
|<span data-ttu-id="43a2e-138">Version</span><span class="sxs-lookup"><span data-stu-id="43a2e-138">version</span></span>|<span data-ttu-id="43a2e-139">String</span><span class="sxs-lookup"><span data-stu-id="43a2e-139">String</span></span>|<span data-ttu-id="43a2e-140">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="43a2e-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43a2e-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="43a2e-141">Relationships</span></span>
<span data-ttu-id="43a2e-142">Keine</span><span class="sxs-lookup"><span data-stu-id="43a2e-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="43a2e-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="43a2e-143">JSON Representation</span></span>
<span data-ttu-id="43a2e-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="43a2e-144">Here is a JSON representation of the resource.</span></span>
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



