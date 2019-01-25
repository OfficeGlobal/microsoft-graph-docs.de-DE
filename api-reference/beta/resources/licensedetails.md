---
title: licenseDetails-Ressourcentyp
description: Enthält Informationen über eine Lizenz, die einem Benutzer zugewiesen ist.
localization_priority: Normal
ms.openlocfilehash: 7036904e20173f8fefb6f4f02bd2473289de96c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522777"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="346c7-103">licenseDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="346c7-103">licenseDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="346c7-104">Enthält Informationen über eine Lizenz, die einem Benutzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="346c7-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="346c7-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="346c7-105">Methods</span></span>

| <span data-ttu-id="346c7-106">Methode</span><span class="sxs-lookup"><span data-stu-id="346c7-106">Method</span></span>           | <span data-ttu-id="346c7-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="346c7-107">Return Type</span></span>    |<span data-ttu-id="346c7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="346c7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="346c7-109">licenseDetails auflisten</span><span class="sxs-lookup"><span data-stu-id="346c7-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="346c7-110">licenseDetails-Sammlung</span><span class="sxs-lookup"><span data-stu-id="346c7-110">licenseDetails collection</span></span> |<span data-ttu-id="346c7-111">Dient zum Abrufen einer Liste von licenseDetails-Objekten für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="346c7-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="346c7-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="346c7-112">Properties</span></span>
| <span data-ttu-id="346c7-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="346c7-113">Property</span></span>     | <span data-ttu-id="346c7-114">Typ</span><span class="sxs-lookup"><span data-stu-id="346c7-114">Type</span></span>   |<span data-ttu-id="346c7-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="346c7-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="346c7-116">id</span><span class="sxs-lookup"><span data-stu-id="346c7-116">id</span></span>|<span data-ttu-id="346c7-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="346c7-117">String</span></span>| <span data-ttu-id="346c7-p101">Der eindeutige Bezeichner für das licenseDetails-Objekt. Schreibgeschützt, Schlüssel, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="346c7-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="346c7-120">servicePlans</span><span class="sxs-lookup"><span data-stu-id="346c7-120">servicePlans</span></span>|<span data-ttu-id="346c7-121">[servicePlanInfo](serviceplaninfo.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="346c7-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="346c7-p102">Informationen über die Servicepläne, die mit der Lizenz zugewiesen werden. Schreibgeschützt, lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="346c7-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="346c7-124">skuId</span><span class="sxs-lookup"><span data-stu-id="346c7-124">skuId</span></span>|<span data-ttu-id="346c7-125">Guid</span><span class="sxs-lookup"><span data-stu-id="346c7-125">Guid</span></span>| <span data-ttu-id="346c7-p103">Der eindeutige Bezeichner (GUID) für die Dienst-SKU. Entspricht der skuId-Eigenschaft des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="346c7-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="346c7-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="346c7-129">skuPartNumber</span></span>|<span data-ttu-id="346c7-130">String</span><span class="sxs-lookup"><span data-stu-id="346c7-130">String</span></span>| <span data-ttu-id="346c7-p104">Eindeutiger SKU-Anzeigename. Entspricht der skuPartNumber des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts, z. B.: „AAD_Premium“. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="346c7-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="346c7-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="346c7-134">Relationships</span></span>
<span data-ttu-id="346c7-135">Keine</span><span class="sxs-lookup"><span data-stu-id="346c7-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="346c7-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="346c7-136">JSON representation</span></span>
<span data-ttu-id="346c7-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="346c7-137">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/licensedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
