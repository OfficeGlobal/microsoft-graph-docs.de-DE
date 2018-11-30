---
title: managedAppPolicy-Ressourcentyp
description: Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.
ms.openlocfilehash: 0cd886e594e58dec3486af6d447969f1610c84fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018671"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="d648f-103">managedAppPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d648f-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="d648f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d648f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d648f-105">Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.</span><span class="sxs-lookup"><span data-stu-id="d648f-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="d648f-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="d648f-106">Methods</span></span>
|<span data-ttu-id="d648f-107">Methode</span><span class="sxs-lookup"><span data-stu-id="d648f-107">Method</span></span>|<span data-ttu-id="d648f-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d648f-108">Return Type</span></span>|<span data-ttu-id="d648f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d648f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d648f-110">managedAppPolicies auflisten</span><span class="sxs-lookup"><span data-stu-id="d648f-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="d648f-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d648f-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d648f-112">Auflisten von Eigenschaften und Beziehungen der [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="d648f-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="d648f-113">managedAppPolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="d648f-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="d648f-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="d648f-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="d648f-115">Lesen von Eigenschaften und Beziehungen des [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d648f-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="d648f-116">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="d648f-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="d648f-117">Keine</span><span class="sxs-lookup"><span data-stu-id="d648f-117">None</span></span>|<span data-ttu-id="d648f-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d648f-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d648f-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d648f-119">Properties</span></span>
|<span data-ttu-id="d648f-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d648f-120">Property</span></span>|<span data-ttu-id="d648f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d648f-121">Type</span></span>|<span data-ttu-id="d648f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d648f-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d648f-123">displayName</span><span class="sxs-lookup"><span data-stu-id="d648f-123">displayName</span></span>|<span data-ttu-id="d648f-124">String</span><span class="sxs-lookup"><span data-stu-id="d648f-124">String</span></span>|<span data-ttu-id="d648f-125">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d648f-125">Policy display name.</span></span>|
|<span data-ttu-id="d648f-126">description</span><span class="sxs-lookup"><span data-stu-id="d648f-126">description</span></span>|<span data-ttu-id="d648f-127">String</span><span class="sxs-lookup"><span data-stu-id="d648f-127">String</span></span>|<span data-ttu-id="d648f-128">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="d648f-128">The policy's description.</span></span>|
|<span data-ttu-id="d648f-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d648f-129">createdDateTime</span></span>|<span data-ttu-id="d648f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d648f-130">DateTimeOffset</span></span>|<span data-ttu-id="d648f-131">Das Datum und die Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="d648f-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="d648f-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d648f-132">lastModifiedDateTime</span></span>|<span data-ttu-id="d648f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d648f-133">DateTimeOffset</span></span>|<span data-ttu-id="d648f-134">Das Datum und die Uhrzeit der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="d648f-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="d648f-135">id</span><span class="sxs-lookup"><span data-stu-id="d648f-135">id</span></span>|<span data-ttu-id="d648f-136">String</span><span class="sxs-lookup"><span data-stu-id="d648f-136">String</span></span>|<span data-ttu-id="d648f-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d648f-137">Key of the entity.</span></span>|
|<span data-ttu-id="d648f-138">Version</span><span class="sxs-lookup"><span data-stu-id="d648f-138">version</span></span>|<span data-ttu-id="d648f-139">String</span><span class="sxs-lookup"><span data-stu-id="d648f-139">String</span></span>|<span data-ttu-id="d648f-140">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="d648f-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d648f-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d648f-141">Relationships</span></span>
<span data-ttu-id="d648f-142">Keine</span><span class="sxs-lookup"><span data-stu-id="d648f-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d648f-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d648f-143">JSON Representation</span></span>
<span data-ttu-id="d648f-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d648f-144">Here is a JSON representation of the resource.</span></span>
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



