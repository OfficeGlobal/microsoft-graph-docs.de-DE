---
title: subscribedSku-Ressourcentyp
description: Enthält Informationen zu einer Dienst-SKU, die ein Unternehmen abonniert hat.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9e61fba199d6d3e509700fe61e75bde240c7f16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937439"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="24231-103">subscribedSku-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="24231-103">subscribedSku resource type</span></span>

<span data-ttu-id="24231-104">Enthält Informationen zu einer Dienst-SKU, die ein Unternehmen abonniert hat.</span><span class="sxs-lookup"><span data-stu-id="24231-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="24231-p101">Für abonnierte SKUs wird nur der Lesevorgang unterstützt. Erstellen, Aktualisieren und Löschen werden nicht unterstützt. Abfragefilterausdrücke werden nicht unterstützt. Erbt von [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="24231-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="24231-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="24231-108">Methods</span></span>
| <span data-ttu-id="24231-109">Methode</span><span class="sxs-lookup"><span data-stu-id="24231-109">Method</span></span>           | <span data-ttu-id="24231-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="24231-110">Return Type</span></span>    |<span data-ttu-id="24231-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24231-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="24231-112">subscribedSku abrufen</span><span class="sxs-lookup"><span data-stu-id="24231-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="24231-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="24231-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="24231-114">Dient zum Lesen der Eigenschaften und Beziehungen des subscribedSku-Objekts.</span><span class="sxs-lookup"><span data-stu-id="24231-114">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="24231-115">Liste subscribedsku</span><span class="sxs-lookup"><span data-stu-id="24231-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="24231-116">[subscribedSku-Sammlung](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="24231-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="24231-117">Dienst zum Abrufen der Liste aller kommerziellen Abonnements, die eine Organisation erworben hat.</span><span class="sxs-lookup"><span data-stu-id="24231-117">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="24231-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="24231-118">Properties</span></span>
| <span data-ttu-id="24231-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="24231-119">Property</span></span>     | <span data-ttu-id="24231-120">Typ</span><span class="sxs-lookup"><span data-stu-id="24231-120">Type</span></span>   |<span data-ttu-id="24231-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24231-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24231-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="24231-122">appliesTo</span></span>|<span data-ttu-id="24231-123">String</span><span class="sxs-lookup"><span data-stu-id="24231-123">String</span></span>| <span data-ttu-id="24231-124">Beispiel: „Benutzer“ oder „Community“.</span><span class="sxs-lookup"><span data-stu-id="24231-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="24231-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="24231-125">capabilityStatus</span></span>|<span data-ttu-id="24231-126">String</span><span class="sxs-lookup"><span data-stu-id="24231-126">String</span></span>| <span data-ttu-id="24231-127">Beispiel: „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="24231-127">For example, "Enabled".</span></span> |
|<span data-ttu-id="24231-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="24231-128">consumedUnits</span></span>|<span data-ttu-id="24231-129">Int32</span><span class="sxs-lookup"><span data-stu-id="24231-129">Int32</span></span>| <span data-ttu-id="24231-130">Die Anzahl der Lizenzen, die zugewiesen wurden.</span><span class="sxs-lookup"><span data-stu-id="24231-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="24231-131">id</span><span class="sxs-lookup"><span data-stu-id="24231-131">id</span></span>|<span data-ttu-id="24231-132">String</span><span class="sxs-lookup"><span data-stu-id="24231-132">String</span></span>| <span data-ttu-id="24231-p102">Der eindeutige Bezeichner für das subscribedSku-Objekt. Schlüssel, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="24231-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="24231-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="24231-135">prepaidUnits</span></span>|[<span data-ttu-id="24231-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="24231-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="24231-137">Informationen über die Anzahl und den Status der Prepaidlizenzen.</span><span class="sxs-lookup"><span data-stu-id="24231-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="24231-138">servicePlans</span><span class="sxs-lookup"><span data-stu-id="24231-138">servicePlans</span></span>|<span data-ttu-id="24231-139">[servicePlanInfo](serviceplaninfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="24231-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="24231-p103">Informationen über die Servicepläne, die mit der SKU verfügbar sind. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="24231-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="24231-142">skuId</span><span class="sxs-lookup"><span data-stu-id="24231-142">skuId</span></span>|<span data-ttu-id="24231-143">Guid</span><span class="sxs-lookup"><span data-stu-id="24231-143">Guid</span></span>| <span data-ttu-id="24231-144">Der eindeutige Bezeichner (GUID) für die Dienst-SKU.</span><span class="sxs-lookup"><span data-stu-id="24231-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="24231-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="24231-145">skuPartNumber</span></span>|<span data-ttu-id="24231-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24231-146">String</span></span>| <span data-ttu-id="24231-147">Die SKU-Teilenummer, z. B.: „AAD_PREMIUM“ oder „RMSBASIC“.</span><span class="sxs-lookup"><span data-stu-id="24231-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="24231-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="24231-148">Relationships</span></span>
<span data-ttu-id="24231-149">Keine</span><span class="sxs-lookup"><span data-stu-id="24231-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24231-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="24231-150">JSON representation</span></span>

<span data-ttu-id="24231-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="24231-151">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
