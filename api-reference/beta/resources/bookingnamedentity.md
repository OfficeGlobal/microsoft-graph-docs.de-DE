---
title: Ressourcentyp bookingNamedEntity
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: fa307d0ee07b43a44210fc6ceaf4c74a29999caa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860501"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="94a0b-104">Ressourcentyp bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="94a0b-104">bookingNamedEntity resource type</span></span>

 > <span data-ttu-id="94a0b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="94a0b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94a0b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="94a0b-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="94a0b-107">Dies ist ein Basistyp für Microsoft Bookings Entitäten, die einen Anzeigenamen ein, beispielsweise bereitstellen, [BookingBusiness](bookingbusiness.md), [BookingPerson](bookingperson.md), [BookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="94a0b-107">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="94a0b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="94a0b-108">Properties</span></span>
| <span data-ttu-id="94a0b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94a0b-109">Property</span></span>     | <span data-ttu-id="94a0b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="94a0b-110">Type</span></span>   |<span data-ttu-id="94a0b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94a0b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94a0b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="94a0b-112">displayName</span></span>|<span data-ttu-id="94a0b-113">String</span><span class="sxs-lookup"><span data-stu-id="94a0b-113">String</span></span>|<span data-ttu-id="94a0b-114">Ein Name für die abgeleitete Entität, welche mit Kunden Schnittstellen.</span><span class="sxs-lookup"><span data-stu-id="94a0b-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="94a0b-115">id</span><span class="sxs-lookup"><span data-stu-id="94a0b-115">id</span></span>|<span data-ttu-id="94a0b-116">String</span><span class="sxs-lookup"><span data-stu-id="94a0b-116">String</span></span>| <span data-ttu-id="94a0b-117">Die ID für die abgeleitete Entität.</span><span class="sxs-lookup"><span data-stu-id="94a0b-117">The ID for the derived entity.</span></span> <span data-ttu-id="94a0b-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="94a0b-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94a0b-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="94a0b-119">Relationships</span></span>
<span data-ttu-id="94a0b-120">Keine</span><span class="sxs-lookup"><span data-stu-id="94a0b-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="94a0b-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="94a0b-121">JSON representation</span></span>

<span data-ttu-id="94a0b-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="94a0b-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
