---
title: Ressourcentyp targetResource
description: Gibt eine Auflistung von Ziel Ressourcentypen mit der Aktivität Audit verknüpfte an. Jede Ressource Zieltyp erbt die Eigenschaften dieser Ressource unten beschriebenen.
ms.openlocfilehash: ba3bee7ce89f73ed97610d62676c22d14488ed9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058561"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="05478-104">Ressourcentyp targetResource</span><span class="sxs-lookup"><span data-stu-id="05478-104">targetResource resource type</span></span>
<span data-ttu-id="05478-105">Gibt eine Auflistung von Ziel Ressourcentypen mit der Aktivität Audit verknüpfte an.</span><span class="sxs-lookup"><span data-stu-id="05478-105">Indicates a collection of  target resource types associated with the audit activity.</span></span> <span data-ttu-id="05478-106">Jede Ressource Zieltyp erbt die Eigenschaften dieser Ressource unten beschriebenen.</span><span class="sxs-lookup"><span data-stu-id="05478-106">Each target resource type will inherit the properties outlined below from this resource.</span></span>


## <a name="properties"></a><span data-ttu-id="05478-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="05478-107">Properties</span></span>
| <span data-ttu-id="05478-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="05478-108">Property</span></span>     | <span data-ttu-id="05478-109">Typ</span><span class="sxs-lookup"><span data-stu-id="05478-109">Type</span></span>   |<span data-ttu-id="05478-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="05478-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05478-111">displayName</span><span class="sxs-lookup"><span data-stu-id="05478-111">displayName</span></span>|<span data-ttu-id="05478-112">String</span><span class="sxs-lookup"><span data-stu-id="05478-112">String</span></span>|<span data-ttu-id="05478-113">Gibt den Anzeigenamen der unter Ziel Ressourcentypen unten aufgeführten Ressourcen an.</span><span class="sxs-lookup"><span data-stu-id="05478-113">Indicates the display name of the resources outlined under Target Resource Types below.</span></span>|
|<span data-ttu-id="05478-114">id</span><span class="sxs-lookup"><span data-stu-id="05478-114">id</span></span>|<span data-ttu-id="05478-115">String</span><span class="sxs-lookup"><span data-stu-id="05478-115">String</span></span>|<span data-ttu-id="05478-116">Gibt die eindeutige Id der Ressource (zum Beispiel: UserId, AppId, RoleId.).</span><span class="sxs-lookup"><span data-stu-id="05478-116">Indicates the Unique Id of the resource (For example: UserId, AppId, RoleId.).</span></span>|
|<span data-ttu-id="05478-117">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="05478-117">modifiedProperties</span></span>|<span data-ttu-id="05478-118">[ModifiedProperty](modifiedproperty.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="05478-118">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="05478-119">Gibt an, Name, alten und neuen Wert der einzelnen Attribute, die geändert.</span><span class="sxs-lookup"><span data-stu-id="05478-119">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="05478-120">Dies gilt für alle Aktivitäten "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="05478-120">This is applicable for any "Update" activities</span></span>|

### <a name="target-resource-types"></a><span data-ttu-id="05478-121">Ziel-Ressourcentypen</span><span class="sxs-lookup"><span data-stu-id="05478-121">Target Resource Types</span></span>

<span data-ttu-id="05478-122">Der Ressourcentyp Ziel variiert entsprechend der zugrunde liegenden Ressource:</span><span class="sxs-lookup"><span data-stu-id="05478-122">The target resource type varies according to the underlying resource:</span></span>

|<span data-ttu-id="05478-123">Ressourcenname</span><span class="sxs-lookup"><span data-stu-id="05478-123">Resource Name</span></span>| <span data-ttu-id="05478-124">Referenz</span><span class="sxs-lookup"><span data-stu-id="05478-124">Reference</span></span>|
|-------------|----------|
<span data-ttu-id="05478-125">Ger?t</span><span class="sxs-lookup"><span data-stu-id="05478-125">Device</span></span>|[<span data-ttu-id="05478-126">targetResourceDevice</span><span class="sxs-lookup"><span data-stu-id="05478-126">targetResourceDevice</span></span>](targetresourcedevice.md)
<span data-ttu-id="05478-127">Verzeichnis</span><span class="sxs-lookup"><span data-stu-id="05478-127">Directory</span></span>|<span data-ttu-id="05478-128">[TargetResourceDirectory] (targetresourcedirectory.md]</span><span class="sxs-lookup"><span data-stu-id="05478-128">[targetResourceDirectory](targetresourcedirectory.md]</span></span>
<span data-ttu-id="05478-129">Gruppe</span><span class="sxs-lookup"><span data-stu-id="05478-129">Group</span></span>|[<span data-ttu-id="05478-130">targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="05478-130">targetResourceGroup</span></span>](targetresourcegroup.md)
<span data-ttu-id="05478-131">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="05478-131">Policy</span></span>|[<span data-ttu-id="05478-132">targetResourcePolicy</span><span class="sxs-lookup"><span data-stu-id="05478-132">targetResourcePolicy</span></span>](targetresourcepolicy.md)
<span data-ttu-id="05478-133">Rolle</span><span class="sxs-lookup"><span data-stu-id="05478-133">Role</span></span>|[<span data-ttu-id="05478-134">targetResourceRole</span><span class="sxs-lookup"><span data-stu-id="05478-134">targetResourceRole</span></span>](targetresourcerole.md)
<span data-ttu-id="05478-135">Dienstprinzipalnamen</span><span class="sxs-lookup"><span data-stu-id="05478-135">Service Principal</span></span>|[<span data-ttu-id="05478-136">targetResourceServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="05478-136">targetResourceServicePrincipal</span></span>](targetresourceserviceprincipal.md)
<span data-ttu-id="05478-137">Benutzer</span><span class="sxs-lookup"><span data-stu-id="05478-137">User</span></span>|[<span data-ttu-id="05478-138">targetResourceUser</span><span class="sxs-lookup"><span data-stu-id="05478-138">targetResourceUser</span></span>](targetresourceuser.md)
<span data-ttu-id="05478-139">Andere</span><span class="sxs-lookup"><span data-stu-id="05478-139">Other</span></span>|[<span data-ttu-id="05478-140">targetResourceOther</span><span class="sxs-lookup"><span data-stu-id="05478-140">targetResourceOther</span></span>](targetresourceother.md)

## <a name="json-representation"></a><span data-ttu-id="05478-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="05478-141">JSON representation</span></span>

<span data-ttu-id="05478-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="05478-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->