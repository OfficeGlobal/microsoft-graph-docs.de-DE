---
title: Ressourcentyp bookingNamedEntity
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 1d82fcf6fcf7ffad6e60baea3f3e1118ec60345d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058610"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="cda16-104">Ressourcentyp bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="cda16-104">bookingNamedEntity resource type</span></span>

 > <span data-ttu-id="cda16-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cda16-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cda16-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cda16-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="cda16-107">Dies ist ein Basistyp für Microsoft Bookings Entitäten, die einen Anzeigenamen ein, beispielsweise bereitstellen, [BookingBusiness](bookingbusiness.md), [BookingPerson](bookingperson.md), [BookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="cda16-107">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cda16-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cda16-108">Properties</span></span>
| <span data-ttu-id="cda16-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cda16-109">Property</span></span>     | <span data-ttu-id="cda16-110">Typ</span><span class="sxs-lookup"><span data-stu-id="cda16-110">Type</span></span>   |<span data-ttu-id="cda16-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cda16-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cda16-112">displayName</span><span class="sxs-lookup"><span data-stu-id="cda16-112">displayName</span></span>|<span data-ttu-id="cda16-113">String</span><span class="sxs-lookup"><span data-stu-id="cda16-113">String</span></span>|<span data-ttu-id="cda16-114">Ein Name für die abgeleitete Entität, welche mit Kunden Schnittstellen.</span><span class="sxs-lookup"><span data-stu-id="cda16-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="cda16-115">id</span><span class="sxs-lookup"><span data-stu-id="cda16-115">id</span></span>|<span data-ttu-id="cda16-116">String</span><span class="sxs-lookup"><span data-stu-id="cda16-116">String</span></span>| <span data-ttu-id="cda16-117">Die ID für die abgeleitete Entität.</span><span class="sxs-lookup"><span data-stu-id="cda16-117">The ID for the derived entity.</span></span> <span data-ttu-id="cda16-118">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cda16-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cda16-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cda16-119">Relationships</span></span>
<span data-ttu-id="cda16-120">Keine</span><span class="sxs-lookup"><span data-stu-id="cda16-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cda16-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cda16-121">JSON representation</span></span>

<span data-ttu-id="cda16-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cda16-122">The following is a JSON representation of the resource.</span></span>

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