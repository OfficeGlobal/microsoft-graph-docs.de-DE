---
title: licenseDetails-Ressourcentyp
description: Enthält Informationen über eine Lizenz, die einem Benutzer zugewiesen ist.
localization_priority: Normal
ms.openlocfilehash: 1f0992904a124931be239fd18ad2bf187e01c41c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885750"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="601fd-103">licenseDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="601fd-103">licenseDetails resource type</span></span>

> <span data-ttu-id="601fd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="601fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="601fd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="601fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="601fd-106">Enthält Informationen über eine Lizenz, die einem Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="601fd-106">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="601fd-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="601fd-107">Methods</span></span>

| <span data-ttu-id="601fd-108">Methode</span><span class="sxs-lookup"><span data-stu-id="601fd-108">Method</span></span>           | <span data-ttu-id="601fd-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="601fd-109">Return Type</span></span>    |<span data-ttu-id="601fd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="601fd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="601fd-111">licenseDetails auflisten</span><span class="sxs-lookup"><span data-stu-id="601fd-111">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="601fd-112">licenseDetails-Sammlung</span><span class="sxs-lookup"><span data-stu-id="601fd-112">licenseDetails collection</span></span> |<span data-ttu-id="601fd-113">Dient zum Abrufen einer Liste von licenseDetails-Objekten für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="601fd-113">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="601fd-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="601fd-114">Properties</span></span>
| <span data-ttu-id="601fd-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="601fd-115">Property</span></span>     | <span data-ttu-id="601fd-116">Typ</span><span class="sxs-lookup"><span data-stu-id="601fd-116">Type</span></span>   |<span data-ttu-id="601fd-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="601fd-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="601fd-118">id</span><span class="sxs-lookup"><span data-stu-id="601fd-118">id</span></span>|<span data-ttu-id="601fd-119">String</span><span class="sxs-lookup"><span data-stu-id="601fd-119">String</span></span>| <span data-ttu-id="601fd-p102">Der eindeutige Bezeichner für das licenseDetails-Objekt. Schreibgeschützt, Schlüssel, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="601fd-p102">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="601fd-122">servicePlans</span><span class="sxs-lookup"><span data-stu-id="601fd-122">servicePlans</span></span>|<span data-ttu-id="601fd-123">[servicePlanInfo](serviceplaninfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="601fd-123">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="601fd-p103">Informationen über die Servicepläne, die mit der Lizenz zugewiesen werden. Schreibgeschützt, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="601fd-p103">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="601fd-126">skuId</span><span class="sxs-lookup"><span data-stu-id="601fd-126">skuId</span></span>|<span data-ttu-id="601fd-127">Guid</span><span class="sxs-lookup"><span data-stu-id="601fd-127">Guid</span></span>| <span data-ttu-id="601fd-p104">Der eindeutige Bezeichner (GUID) für die Dienst-SKU. Entspricht der skuId-Eigenschaft des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="601fd-p104">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="601fd-131">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="601fd-131">skuPartNumber</span></span>|<span data-ttu-id="601fd-132">String</span><span class="sxs-lookup"><span data-stu-id="601fd-132">String</span></span>| <span data-ttu-id="601fd-p105">Eindeutiger SKU-Anzeigename. Entspricht der skuPartNumber des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts, z. B.: „AAD_Premium“. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="601fd-p105">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="601fd-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="601fd-136">Relationships</span></span>
<span data-ttu-id="601fd-137">Keine</span><span class="sxs-lookup"><span data-stu-id="601fd-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="601fd-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="601fd-138">JSON representation</span></span>
<span data-ttu-id="601fd-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="601fd-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
