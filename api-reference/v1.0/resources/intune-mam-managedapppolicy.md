---
title: managedAppPolicy-Ressourcentyp
description: Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5054566f0ee80940165ba19f8f0da197b5e4f3c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981105"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="2ff86-103">managedAppPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2ff86-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="2ff86-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2ff86-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ff86-105">Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.</span><span class="sxs-lookup"><span data-stu-id="2ff86-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="2ff86-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="2ff86-106">Methods</span></span>
|<span data-ttu-id="2ff86-107">Methode</span><span class="sxs-lookup"><span data-stu-id="2ff86-107">Method</span></span>|<span data-ttu-id="2ff86-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2ff86-108">Return Type</span></span>|<span data-ttu-id="2ff86-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ff86-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ff86-110">managedAppPolicies auflisten</span><span class="sxs-lookup"><span data-stu-id="2ff86-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="2ff86-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2ff86-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2ff86-112">Auflisten von Eigenschaften und Beziehungen der [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="2ff86-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="2ff86-113">managedAppPolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="2ff86-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="2ff86-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2ff86-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="2ff86-115">Lesen von Eigenschaften und Beziehungen des [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2ff86-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="2ff86-116">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="2ff86-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="2ff86-117">Keine</span><span class="sxs-lookup"><span data-stu-id="2ff86-117">None</span></span>|<span data-ttu-id="2ff86-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2ff86-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2ff86-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2ff86-119">Properties</span></span>
|<span data-ttu-id="2ff86-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ff86-120">Property</span></span>|<span data-ttu-id="2ff86-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2ff86-121">Type</span></span>|<span data-ttu-id="2ff86-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ff86-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ff86-123">displayName</span><span class="sxs-lookup"><span data-stu-id="2ff86-123">displayName</span></span>|<span data-ttu-id="2ff86-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ff86-124">String</span></span>|<span data-ttu-id="2ff86-125">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2ff86-125">Policy display name.</span></span>|
|<span data-ttu-id="2ff86-126">description</span><span class="sxs-lookup"><span data-stu-id="2ff86-126">description</span></span>|<span data-ttu-id="2ff86-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ff86-127">String</span></span>|<span data-ttu-id="2ff86-128">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="2ff86-128">The policy's description.</span></span>|
|<span data-ttu-id="2ff86-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ff86-129">createdDateTime</span></span>|<span data-ttu-id="2ff86-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ff86-130">DateTimeOffset</span></span>|<span data-ttu-id="2ff86-131">Das Datum und die Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="2ff86-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="2ff86-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ff86-132">lastModifiedDateTime</span></span>|<span data-ttu-id="2ff86-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ff86-133">DateTimeOffset</span></span>|<span data-ttu-id="2ff86-134">Das Datum und die Uhrzeit der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="2ff86-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="2ff86-135">id</span><span class="sxs-lookup"><span data-stu-id="2ff86-135">id</span></span>|<span data-ttu-id="2ff86-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ff86-136">String</span></span>|<span data-ttu-id="2ff86-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2ff86-137">Key of the entity.</span></span>|
|<span data-ttu-id="2ff86-138">Version</span><span class="sxs-lookup"><span data-stu-id="2ff86-138">version</span></span>|<span data-ttu-id="2ff86-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ff86-139">String</span></span>|<span data-ttu-id="2ff86-140">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="2ff86-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ff86-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2ff86-141">Relationships</span></span>
<span data-ttu-id="2ff86-142">Keine</span><span class="sxs-lookup"><span data-stu-id="2ff86-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ff86-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2ff86-143">JSON Representation</span></span>
<span data-ttu-id="2ff86-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2ff86-144">Here is a JSON representation of the resource.</span></span>
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



