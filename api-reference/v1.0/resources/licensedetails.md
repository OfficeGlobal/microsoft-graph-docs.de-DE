---
title: licenseDetails-Ressourcentyp
description: Enthält Informationen über eine Lizenz, die einem Benutzer zugewiesen ist.
localization_priority: Normal
ms.openlocfilehash: 4495e85b45f6fcfda4f37e467e9cdc5393787dc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843022"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="26080-103">licenseDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="26080-103">licenseDetails resource type</span></span>

<span data-ttu-id="26080-104">Enthält Informationen über eine Lizenz, die einem Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="26080-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="26080-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="26080-105">Methods</span></span>

| <span data-ttu-id="26080-106">Methode</span><span class="sxs-lookup"><span data-stu-id="26080-106">Method</span></span>           | <span data-ttu-id="26080-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="26080-107">Return Type</span></span>    |<span data-ttu-id="26080-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26080-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26080-109">licenseDetails auflisten</span><span class="sxs-lookup"><span data-stu-id="26080-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="26080-110">licenseDetails-Sammlung</span><span class="sxs-lookup"><span data-stu-id="26080-110">licenseDetails collection</span></span> |<span data-ttu-id="26080-111">Dient zum Abrufen einer Liste von licenseDetails-Objekten für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="26080-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="26080-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="26080-112">Properties</span></span>
| <span data-ttu-id="26080-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26080-113">Property</span></span>     | <span data-ttu-id="26080-114">Typ</span><span class="sxs-lookup"><span data-stu-id="26080-114">Type</span></span>   |<span data-ttu-id="26080-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26080-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26080-116">id</span><span class="sxs-lookup"><span data-stu-id="26080-116">id</span></span>|<span data-ttu-id="26080-117">String</span><span class="sxs-lookup"><span data-stu-id="26080-117">String</span></span>| <span data-ttu-id="26080-p101">Der eindeutige Bezeichner für das licenseDetails-Objekt. Schreibgeschützt, Schlüssel, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="26080-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="26080-120">servicePlans</span><span class="sxs-lookup"><span data-stu-id="26080-120">servicePlans</span></span>|<span data-ttu-id="26080-121">[servicePlanInfo](serviceplaninfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="26080-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="26080-p102">Informationen über die Servicepläne, die mit der Lizenz zugewiesen werden. Schreibgeschützt, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="26080-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="26080-124">skuId</span><span class="sxs-lookup"><span data-stu-id="26080-124">skuId</span></span>|<span data-ttu-id="26080-125">Guid</span><span class="sxs-lookup"><span data-stu-id="26080-125">Guid</span></span>| <span data-ttu-id="26080-p103">Der eindeutige Bezeichner (GUID) für die Dienst-SKU. Entspricht der skuId-Eigenschaft des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="26080-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="26080-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="26080-129">skuPartNumber</span></span>|<span data-ttu-id="26080-130">String</span><span class="sxs-lookup"><span data-stu-id="26080-130">String</span></span>| <span data-ttu-id="26080-p104">Eindeutiger SKU-Anzeigename. Entspricht der skuPartNumber des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts, z. B.: „AAD_Premium“. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="26080-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="26080-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="26080-134">Relationships</span></span>
<span data-ttu-id="26080-135">Keine</span><span class="sxs-lookup"><span data-stu-id="26080-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26080-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="26080-136">JSON representation</span></span>
<span data-ttu-id="26080-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="26080-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
