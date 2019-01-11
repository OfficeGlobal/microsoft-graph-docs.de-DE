---
title: managedAppPolicy-Ressourcentyp
description: Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3cea81d492e708c1d21039c6286fe01e70a590b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840733"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="09304-103">managedAppPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="09304-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="09304-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="09304-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09304-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09304-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09304-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="09304-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09304-107">Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.</span><span class="sxs-lookup"><span data-stu-id="09304-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="09304-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="09304-108">Methods</span></span>
|<span data-ttu-id="09304-109">Methode</span><span class="sxs-lookup"><span data-stu-id="09304-109">Method</span></span>|<span data-ttu-id="09304-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="09304-110">Return Type</span></span>|<span data-ttu-id="09304-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09304-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="09304-112">managedAppPolicies auflisten</span><span class="sxs-lookup"><span data-stu-id="09304-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="09304-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="09304-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="09304-114">Auflisten von Eigenschaften und Beziehungen der [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="09304-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="09304-115">managedAppPolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="09304-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="09304-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="09304-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="09304-117">Lesen von Eigenschaften und Beziehungen des [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="09304-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="09304-118">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="09304-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="09304-119">Keine</span><span class="sxs-lookup"><span data-stu-id="09304-119">None</span></span>|<span data-ttu-id="09304-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="09304-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="09304-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="09304-121">Properties</span></span>
|<span data-ttu-id="09304-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="09304-122">Property</span></span>|<span data-ttu-id="09304-123">Typ</span><span class="sxs-lookup"><span data-stu-id="09304-123">Type</span></span>|<span data-ttu-id="09304-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09304-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09304-125">displayName</span><span class="sxs-lookup"><span data-stu-id="09304-125">displayName</span></span>|<span data-ttu-id="09304-126">String</span><span class="sxs-lookup"><span data-stu-id="09304-126">String</span></span>|<span data-ttu-id="09304-127">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="09304-127">Policy display name.</span></span>|
|<span data-ttu-id="09304-128">description</span><span class="sxs-lookup"><span data-stu-id="09304-128">description</span></span>|<span data-ttu-id="09304-129">String</span><span class="sxs-lookup"><span data-stu-id="09304-129">String</span></span>|<span data-ttu-id="09304-130">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="09304-130">The policy's description.</span></span>|
|<span data-ttu-id="09304-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09304-131">createdDateTime</span></span>|<span data-ttu-id="09304-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09304-132">DateTimeOffset</span></span>|<span data-ttu-id="09304-133">Das Datum und die Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="09304-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="09304-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09304-134">lastModifiedDateTime</span></span>|<span data-ttu-id="09304-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09304-135">DateTimeOffset</span></span>|<span data-ttu-id="09304-136">Das Datum und die Uhrzeit der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="09304-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="09304-137">id</span><span class="sxs-lookup"><span data-stu-id="09304-137">id</span></span>|<span data-ttu-id="09304-138">String</span><span class="sxs-lookup"><span data-stu-id="09304-138">String</span></span>|<span data-ttu-id="09304-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="09304-139">Key of the entity.</span></span>|
|<span data-ttu-id="09304-140">Version</span><span class="sxs-lookup"><span data-stu-id="09304-140">version</span></span>|<span data-ttu-id="09304-141">String</span><span class="sxs-lookup"><span data-stu-id="09304-141">String</span></span>|<span data-ttu-id="09304-142">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="09304-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09304-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="09304-143">Relationships</span></span>
<span data-ttu-id="09304-144">Keine</span><span class="sxs-lookup"><span data-stu-id="09304-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09304-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="09304-145">JSON Representation</span></span>
<span data-ttu-id="09304-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="09304-146">Here is a JSON representation of the resource.</span></span>
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





