---
title: subscribedSku-Ressourcentyp
description: " Erstellen, Update und Delete werden nicht unterstützt. Abfrageausdrücke Filter werden nicht unterstützt. Erbt von directoryObject."
ms.openlocfilehash: ab9b64d8de67379aa002ffeec78edd327b15b222
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064767"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="9fa67-105">subscribedSku-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9fa67-105">subscribedSku resource type</span></span>

> <span data-ttu-id="9fa67-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9fa67-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fa67-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9fa67-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9fa67-p103">Für abonnierte SKUs wird nur der Lesevorgang unterstützt. Erstellen, Aktualisieren und Löschen werden nicht unterstützt. Abfragefilterausdrücke werden nicht unterstützt. Erbt von [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="9fa67-p103">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="9fa67-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="9fa67-111">Methods</span></span>
| <span data-ttu-id="9fa67-112">Methode</span><span class="sxs-lookup"><span data-stu-id="9fa67-112">Method</span></span>           | <span data-ttu-id="9fa67-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9fa67-113">Return Type</span></span>    |<span data-ttu-id="9fa67-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fa67-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9fa67-115">subscribedSku abrufen</span><span class="sxs-lookup"><span data-stu-id="9fa67-115">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="9fa67-116">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="9fa67-116">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="9fa67-117">Dient zum Lesen der Eigenschaften und Beziehungen des subscribedSku-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9fa67-117">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="9fa67-118">Liste subscribedsku</span><span class="sxs-lookup"><span data-stu-id="9fa67-118">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="9fa67-119">[subscribedSku-Sammlung](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="9fa67-119">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="9fa67-120">Dienst zum Abrufen der Liste aller kommerziellen Abonnements, die eine Organisation erworben hat.</span><span class="sxs-lookup"><span data-stu-id="9fa67-120">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fa67-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9fa67-121">Properties</span></span>
| <span data-ttu-id="9fa67-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9fa67-122">Property</span></span>     | <span data-ttu-id="9fa67-123">Typ</span><span class="sxs-lookup"><span data-stu-id="9fa67-123">Type</span></span>   |<span data-ttu-id="9fa67-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fa67-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fa67-125">appliesTo</span><span class="sxs-lookup"><span data-stu-id="9fa67-125">appliesTo</span></span>|<span data-ttu-id="9fa67-126">String</span><span class="sxs-lookup"><span data-stu-id="9fa67-126">String</span></span>| <span data-ttu-id="9fa67-127">Beispiel: „Benutzer“ oder „Community“.</span><span class="sxs-lookup"><span data-stu-id="9fa67-127">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="9fa67-128">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="9fa67-128">capabilityStatus</span></span>|<span data-ttu-id="9fa67-129">String</span><span class="sxs-lookup"><span data-stu-id="9fa67-129">String</span></span>| <span data-ttu-id="9fa67-130">Beispiel: „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="9fa67-130">For example, "Enabled".</span></span> |
|<span data-ttu-id="9fa67-131">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="9fa67-131">consumedUnits</span></span>|<span data-ttu-id="9fa67-132">Int32</span><span class="sxs-lookup"><span data-stu-id="9fa67-132">Int32</span></span>| <span data-ttu-id="9fa67-133">Die Anzahl der Lizenzen, die zugewiesen wurden.</span><span class="sxs-lookup"><span data-stu-id="9fa67-133">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="9fa67-134">id</span><span class="sxs-lookup"><span data-stu-id="9fa67-134">id</span></span>|<span data-ttu-id="9fa67-135">String</span><span class="sxs-lookup"><span data-stu-id="9fa67-135">String</span></span>| <span data-ttu-id="9fa67-p104">Der eindeutige Bezeichner für das subscribedSku-Objekt. Schlüssel, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="9fa67-p104">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="9fa67-138">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="9fa67-138">prepaidUnits</span></span>|[<span data-ttu-id="9fa67-139">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="9fa67-139">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="9fa67-140">Informationen über die Anzahl und den Status der Prepaidlizenzen.</span><span class="sxs-lookup"><span data-stu-id="9fa67-140">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="9fa67-141">servicePlans</span><span class="sxs-lookup"><span data-stu-id="9fa67-141">servicePlans</span></span>|<span data-ttu-id="9fa67-142">[servicePlanInfo](serviceplaninfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9fa67-142">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="9fa67-p105">Informationen über die Servicepläne, die mit der SKU verfügbar sind. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="9fa67-p105">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="9fa67-145">skuId</span><span class="sxs-lookup"><span data-stu-id="9fa67-145">skuId</span></span>|<span data-ttu-id="9fa67-146">Guid</span><span class="sxs-lookup"><span data-stu-id="9fa67-146">Guid</span></span>| <span data-ttu-id="9fa67-147">Der eindeutige Bezeichner (GUID) für die Dienst-SKU.</span><span class="sxs-lookup"><span data-stu-id="9fa67-147">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="9fa67-148">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="9fa67-148">skuPartNumber</span></span>|<span data-ttu-id="9fa67-149">String</span><span class="sxs-lookup"><span data-stu-id="9fa67-149">String</span></span>| <span data-ttu-id="9fa67-150">Die SKU-Teilenummer, z. B.: „AAD_PREMIUM“ oder „RMSBASIC“.</span><span class="sxs-lookup"><span data-stu-id="9fa67-150">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="9fa67-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9fa67-151">Relationships</span></span>
<span data-ttu-id="9fa67-152">Keine</span><span class="sxs-lookup"><span data-stu-id="9fa67-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fa67-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9fa67-153">JSON representation</span></span>

<span data-ttu-id="9fa67-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9fa67-154">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
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
