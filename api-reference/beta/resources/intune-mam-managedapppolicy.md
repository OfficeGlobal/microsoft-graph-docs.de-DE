---
title: managedAppPolicy-Ressourcentyp
description: Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 45a8365bb7a1ea97c156921cfbd923ba9b52dd1b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937502"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="e8b0e-103">managedAppPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e8b0e-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="e8b0e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e8b0e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8b0e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e8b0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8b0e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e8b0e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8b0e-107">Die ManagedAppPolicy-Ressource stellt einen Basistyp für plattformspezifische Richtlinien dar.</span><span class="sxs-lookup"><span data-stu-id="e8b0e-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="e8b0e-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="e8b0e-108">Methods</span></span>
|<span data-ttu-id="e8b0e-109">Methode</span><span class="sxs-lookup"><span data-stu-id="e8b0e-109">Method</span></span>|<span data-ttu-id="e8b0e-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e8b0e-110">Return Type</span></span>|<span data-ttu-id="e8b0e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8b0e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e8b0e-112">managedAppPolicies auflisten</span><span class="sxs-lookup"><span data-stu-id="e8b0e-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="e8b0e-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e8b0e-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e8b0e-114">Auflisten von Eigenschaften und Beziehungen der [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="e8b0e-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="e8b0e-115">managedAppPolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="e8b0e-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="e8b0e-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="e8b0e-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="e8b0e-117">Lesen von Eigenschaften und Beziehungen des [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e8b0e-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="e8b0e-118">targetApps-Aktion</span><span class="sxs-lookup"><span data-stu-id="e8b0e-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="e8b0e-119">Keine</span><span class="sxs-lookup"><span data-stu-id="e8b0e-119">None</span></span>|<span data-ttu-id="e8b0e-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e8b0e-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e8b0e-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e8b0e-121">Properties</span></span>
|<span data-ttu-id="e8b0e-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e8b0e-122">Property</span></span>|<span data-ttu-id="e8b0e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e8b0e-123">Type</span></span>|<span data-ttu-id="e8b0e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8b0e-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8b0e-125">displayName</span><span class="sxs-lookup"><span data-stu-id="e8b0e-125">displayName</span></span>|<span data-ttu-id="e8b0e-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8b0e-126">String</span></span>|<span data-ttu-id="e8b0e-127">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="e8b0e-127">Policy display name.</span></span>|
|<span data-ttu-id="e8b0e-128">description</span><span class="sxs-lookup"><span data-stu-id="e8b0e-128">description</span></span>|<span data-ttu-id="e8b0e-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8b0e-129">String</span></span>|<span data-ttu-id="e8b0e-130">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="e8b0e-130">The policy's description.</span></span>|
|<span data-ttu-id="e8b0e-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8b0e-131">createdDateTime</span></span>|<span data-ttu-id="e8b0e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8b0e-132">DateTimeOffset</span></span>|<span data-ttu-id="e8b0e-133">Das Datum und die Uhrzeit der Erstellung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="e8b0e-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="e8b0e-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8b0e-134">lastModifiedDateTime</span></span>|<span data-ttu-id="e8b0e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8b0e-135">DateTimeOffset</span></span>|<span data-ttu-id="e8b0e-136">Das Datum und die Uhrzeit der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="e8b0e-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="e8b0e-137">id</span><span class="sxs-lookup"><span data-stu-id="e8b0e-137">id</span></span>|<span data-ttu-id="e8b0e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8b0e-138">String</span></span>|<span data-ttu-id="e8b0e-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e8b0e-139">Key of the entity.</span></span>|
|<span data-ttu-id="e8b0e-140">Version</span><span class="sxs-lookup"><span data-stu-id="e8b0e-140">version</span></span>|<span data-ttu-id="e8b0e-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e8b0e-141">String</span></span>|<span data-ttu-id="e8b0e-142">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="e8b0e-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8b0e-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e8b0e-143">Relationships</span></span>
<span data-ttu-id="e8b0e-144">Keine</span><span class="sxs-lookup"><span data-stu-id="e8b0e-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e8b0e-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e8b0e-145">JSON Representation</span></span>
<span data-ttu-id="e8b0e-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e8b0e-146">Here is a JSON representation of the resource.</span></span>
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





