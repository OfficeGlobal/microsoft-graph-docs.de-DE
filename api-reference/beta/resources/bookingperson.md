---
title: Ressourcentyp bookingPerson
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: d20f6ee9e14723a80f012cfffb1e4b8214f89739
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063102"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="e1819-104">Ressourcentyp bookingPerson</span><span class="sxs-lookup"><span data-stu-id="e1819-104">bookingPerson resource type</span></span>

 > <span data-ttu-id="e1819-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e1819-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1819-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1819-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e1819-107">Dies ist ein Basistyp für eine Person in einem Unternehmen Microsoft Bookings, der ein [BookingCustomer](bookingcustomer.md) oder [BookingStaffMember](bookingstaffmember.md)sein kann.</span><span class="sxs-lookup"><span data-stu-id="e1819-107">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e1819-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e1819-108">Properties</span></span>
| <span data-ttu-id="e1819-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1819-109">Property</span></span>     | <span data-ttu-id="e1819-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e1819-110">Type</span></span>   |<span data-ttu-id="e1819-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1819-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1819-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e1819-112">displayName</span></span>|<span data-ttu-id="e1819-113">String</span><span class="sxs-lookup"><span data-stu-id="e1819-113">String</span></span>|<span data-ttu-id="e1819-114">Ein Name für die abgeleitete Entität, welche mit Kunden Schnittstellen.</span><span class="sxs-lookup"><span data-stu-id="e1819-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="e1819-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e1819-115">emailAddress</span></span>|<span data-ttu-id="e1819-116">String</span><span class="sxs-lookup"><span data-stu-id="e1819-116">String</span></span>|<span data-ttu-id="e1819-117">Die e-Mail-Adresse der Person ein.</span><span class="sxs-lookup"><span data-stu-id="e1819-117">The email address of the person.</span></span>|
|<span data-ttu-id="e1819-118">id</span><span class="sxs-lookup"><span data-stu-id="e1819-118">id</span></span>|<span data-ttu-id="e1819-119">String</span><span class="sxs-lookup"><span data-stu-id="e1819-119">String</span></span>| <span data-ttu-id="e1819-120">Die ID für die abgeleitete Entität.</span><span class="sxs-lookup"><span data-stu-id="e1819-120">The ID for the derived entity.</span></span> <span data-ttu-id="e1819-121">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e1819-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1819-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e1819-122">Relationships</span></span>
<span data-ttu-id="e1819-123">Keine</span><span class="sxs-lookup"><span data-stu-id="e1819-123">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e1819-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e1819-124">JSON representation</span></span>

<span data-ttu-id="e1819-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e1819-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->