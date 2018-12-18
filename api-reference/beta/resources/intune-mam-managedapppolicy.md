---
title: managedAppPolicy-Ressourcentyp
description: Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.
author: tfitzmac
ms.openlocfilehash: d971f99c4f081d5b40179d406f6a50acf5812e4f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313461"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="9f4db-103">managedAppPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9f4db-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="9f4db-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9f4db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f4db-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f4db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f4db-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9f4db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f4db-107">Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.</span><span class="sxs-lookup"><span data-stu-id="9f4db-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="9f4db-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="9f4db-108">Methods</span></span>
|<span data-ttu-id="9f4db-109">Methode</span><span class="sxs-lookup"><span data-stu-id="9f4db-109">Method</span></span>|<span data-ttu-id="9f4db-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9f4db-110">Return Type</span></span>|<span data-ttu-id="9f4db-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f4db-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9f4db-112">managedAppPolicies auflisten</span><span class="sxs-lookup"><span data-stu-id="9f4db-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="9f4db-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9f4db-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="9f4db-114">Auflisten von Eigenschaften und Beziehungen der [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="9f4db-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="9f4db-115">managedAppPolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="9f4db-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="9f4db-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="9f4db-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="9f4db-117">Lesen von Eigenschaften und Beziehungen des [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9f4db-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="9f4db-118">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="9f4db-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="9f4db-119">Keine</span><span class="sxs-lookup"><span data-stu-id="9f4db-119">None</span></span>|<span data-ttu-id="9f4db-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9f4db-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9f4db-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9f4db-121">Properties</span></span>
|<span data-ttu-id="9f4db-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f4db-122">Property</span></span>|<span data-ttu-id="9f4db-123">Typ</span><span class="sxs-lookup"><span data-stu-id="9f4db-123">Type</span></span>|<span data-ttu-id="9f4db-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f4db-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f4db-125">displayName</span><span class="sxs-lookup"><span data-stu-id="9f4db-125">displayName</span></span>|<span data-ttu-id="9f4db-126">String</span><span class="sxs-lookup"><span data-stu-id="9f4db-126">String</span></span>|<span data-ttu-id="9f4db-127">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="9f4db-127">Policy display name.</span></span>|
|<span data-ttu-id="9f4db-128">description</span><span class="sxs-lookup"><span data-stu-id="9f4db-128">description</span></span>|<span data-ttu-id="9f4db-129">String</span><span class="sxs-lookup"><span data-stu-id="9f4db-129">String</span></span>|<span data-ttu-id="9f4db-130">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="9f4db-130">The policy's description.</span></span>|
|<span data-ttu-id="9f4db-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f4db-131">createdDateTime</span></span>|<span data-ttu-id="9f4db-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f4db-132">DateTimeOffset</span></span>|<span data-ttu-id="9f4db-133">Das Datum und die Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="9f4db-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="9f4db-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f4db-134">lastModifiedDateTime</span></span>|<span data-ttu-id="9f4db-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f4db-135">DateTimeOffset</span></span>|<span data-ttu-id="9f4db-136">Das Datum und die Uhrzeit der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="9f4db-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="9f4db-137">id</span><span class="sxs-lookup"><span data-stu-id="9f4db-137">id</span></span>|<span data-ttu-id="9f4db-138">String</span><span class="sxs-lookup"><span data-stu-id="9f4db-138">String</span></span>|<span data-ttu-id="9f4db-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9f4db-139">Key of the entity.</span></span>|
|<span data-ttu-id="9f4db-140">Version</span><span class="sxs-lookup"><span data-stu-id="9f4db-140">version</span></span>|<span data-ttu-id="9f4db-141">String</span><span class="sxs-lookup"><span data-stu-id="9f4db-141">String</span></span>|<span data-ttu-id="9f4db-142">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="9f4db-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f4db-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9f4db-143">Relationships</span></span>
<span data-ttu-id="9f4db-144">Keine</span><span class="sxs-lookup"><span data-stu-id="9f4db-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f4db-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9f4db-145">JSON Representation</span></span>
<span data-ttu-id="9f4db-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9f4db-146">Here is a JSON representation of the resource.</span></span>
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





