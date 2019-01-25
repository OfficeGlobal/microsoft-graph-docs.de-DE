---
title: Ressourcentyp bookingPerson
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: be00e59e2378c454cd9c939f992376dd9c54c3b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508405"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="68547-104">Ressourcentyp bookingPerson</span><span class="sxs-lookup"><span data-stu-id="68547-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="68547-105">Dies ist ein Basistyp für eine Person in einem Unternehmen Microsoft Bookings, der ein [BookingCustomer](bookingcustomer.md) oder [BookingStaffMember](bookingstaffmember.md)sein kann.</span><span class="sxs-lookup"><span data-stu-id="68547-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="68547-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="68547-106">Properties</span></span>
| <span data-ttu-id="68547-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="68547-107">Property</span></span>     | <span data-ttu-id="68547-108">Typ</span><span class="sxs-lookup"><span data-stu-id="68547-108">Type</span></span>   |<span data-ttu-id="68547-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68547-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68547-110">displayName</span><span class="sxs-lookup"><span data-stu-id="68547-110">displayName</span></span>|<span data-ttu-id="68547-111">String</span><span class="sxs-lookup"><span data-stu-id="68547-111">String</span></span>|<span data-ttu-id="68547-112">Ein Name für die abgeleitete Entität, welche mit Kunden Schnittstellen.</span><span class="sxs-lookup"><span data-stu-id="68547-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="68547-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="68547-113">emailAddress</span></span>|<span data-ttu-id="68547-114">String</span><span class="sxs-lookup"><span data-stu-id="68547-114">String</span></span>|<span data-ttu-id="68547-115">Die e-Mail-Adresse der Person ein.</span><span class="sxs-lookup"><span data-stu-id="68547-115">The email address of the person.</span></span>|
|<span data-ttu-id="68547-116">id</span><span class="sxs-lookup"><span data-stu-id="68547-116">id</span></span>|<span data-ttu-id="68547-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68547-117">String</span></span>| <span data-ttu-id="68547-118">Die ID für die abgeleitete Entität.</span><span class="sxs-lookup"><span data-stu-id="68547-118">The ID for the derived entity.</span></span> <span data-ttu-id="68547-119">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="68547-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68547-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="68547-120">Relationships</span></span>
<span data-ttu-id="68547-121">Keine</span><span class="sxs-lookup"><span data-stu-id="68547-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="68547-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="68547-122">JSON representation</span></span>

<span data-ttu-id="68547-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68547-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingperson.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
