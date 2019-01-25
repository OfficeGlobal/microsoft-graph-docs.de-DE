---
title: subscribedSku-Ressourcentyp
description: " Erstellen, Update und Delete werden nicht unterstützt. Abfrageausdrücke Filter werden nicht unterstützt. Erbt von directoryObject."
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 090e6912ce2f337a8e30322c9b45161af73175cc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522700"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="b7ea8-105">subscribedSku-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b7ea8-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7ea8-p102">Für abonnierte SKUs wird nur der Lesevorgang unterstützt. Erstellen, Aktualisieren und Löschen werden nicht unterstützt. Abfragefilterausdrücke werden nicht unterstützt. Erbt von [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="b7ea8-p102">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="b7ea8-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="b7ea8-109">Methods</span></span>
| <span data-ttu-id="b7ea8-110">Methode</span><span class="sxs-lookup"><span data-stu-id="b7ea8-110">Method</span></span>           | <span data-ttu-id="b7ea8-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b7ea8-111">Return Type</span></span>    |<span data-ttu-id="b7ea8-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7ea8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7ea8-113">subscribedSku abrufen</span><span class="sxs-lookup"><span data-stu-id="b7ea8-113">[Get subscribedSku](../api/subscribedsku-get.md)</span></span> | [<span data-ttu-id="b7ea8-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="b7ea8-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="b7ea8-115">Dient zum Lesen der Eigenschaften und Beziehungen des subscribedSku-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-115">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="b7ea8-116">subscribedSku auflisten</span><span class="sxs-lookup"><span data-stu-id="b7ea8-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="b7ea8-117">[subscribedSku-Sammlung](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="b7ea8-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="b7ea8-118">Dienst zum Abrufen der Liste aller kommerziellen Abonnements, die eine Organisation erworben hat.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-118">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7ea8-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b7ea8-119">Properties</span></span>
| <span data-ttu-id="b7ea8-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b7ea8-120">Property</span></span>     | <span data-ttu-id="b7ea8-121">Typ</span><span class="sxs-lookup"><span data-stu-id="b7ea8-121">Type</span></span>   |<span data-ttu-id="b7ea8-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7ea8-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7ea8-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="b7ea8-123">appliesTo</span></span>|<span data-ttu-id="b7ea8-124">String</span><span class="sxs-lookup"><span data-stu-id="b7ea8-124">String</span></span>| <span data-ttu-id="b7ea8-125">Beispiel: „Benutzer“ oder „Community“.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="b7ea8-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="b7ea8-126">capabilityStatus</span></span>|<span data-ttu-id="b7ea8-127">String</span><span class="sxs-lookup"><span data-stu-id="b7ea8-127">String</span></span>| <span data-ttu-id="b7ea8-128">Beispiel: „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="b7ea8-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="b7ea8-129">consumedUnits</span></span>|<span data-ttu-id="b7ea8-130">Int32</span><span class="sxs-lookup"><span data-stu-id="b7ea8-130">Int32</span></span>| <span data-ttu-id="b7ea8-131">Die Anzahl der Lizenzen, die zugewiesen wurden.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="b7ea8-132">id</span><span class="sxs-lookup"><span data-stu-id="b7ea8-132">id</span></span>|<span data-ttu-id="b7ea8-133">String</span><span class="sxs-lookup"><span data-stu-id="b7ea8-133">String</span></span>| <span data-ttu-id="b7ea8-p103">Der eindeutige Bezeichner für das subscribedSku-Objekt. Schlüssel, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-p103">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="b7ea8-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="b7ea8-136">prepaidUnits</span></span>|[<span data-ttu-id="b7ea8-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="b7ea8-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="b7ea8-138">Informationen über die Anzahl und den Status der Prepaidlizenzen.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="b7ea8-139">servicePlans</span><span class="sxs-lookup"><span data-stu-id="b7ea8-139">servicePlans</span></span>|<span data-ttu-id="b7ea8-140">[servicePlanInfo](serviceplaninfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b7ea8-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="b7ea8-p104">Informationen über die Servicepläne, die mit der SKU verfügbar sind. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-p104">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="b7ea8-143">skuId</span><span class="sxs-lookup"><span data-stu-id="b7ea8-143">skuId</span></span>|<span data-ttu-id="b7ea8-144">Guid</span><span class="sxs-lookup"><span data-stu-id="b7ea8-144">Guid</span></span>| <span data-ttu-id="b7ea8-145">Der eindeutige Bezeichner (GUID) für die Dienst-SKU.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="b7ea8-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="b7ea8-146">skuPartNumber</span></span>|<span data-ttu-id="b7ea8-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b7ea8-147">String</span></span>| <span data-ttu-id="b7ea8-148">Die SKU-Teilenummer, z. B.: „AAD_PREMIUM“ oder „RMSBASIC“.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="b7ea8-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b7ea8-149">Relationships</span></span>
<span data-ttu-id="b7ea8-150">Keine</span><span class="sxs-lookup"><span data-stu-id="b7ea8-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7ea8-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b7ea8-151">JSON representation</span></span>

<span data-ttu-id="b7ea8-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b7ea8-152">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/subscribedsku.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
