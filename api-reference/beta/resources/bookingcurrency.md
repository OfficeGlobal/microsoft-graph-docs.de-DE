---
title: Ressourcentyp bookingCurrency
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9d4feac66e72c756173113101a88bf8bbe35563a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518198"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="efdc5-104">Ressourcentyp bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="efdc5-104">bookingCurrency resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="efdc5-105">Stellt eine monetäre Währung, die von einem [BookingBusiness](bookingbusiness.md)unterstützt.</span><span class="sxs-lookup"><span data-stu-id="efdc5-105">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="efdc5-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="efdc5-106">Methods</span></span>

| <span data-ttu-id="efdc5-107">Methode</span><span class="sxs-lookup"><span data-stu-id="efdc5-107">Method</span></span>           | <span data-ttu-id="efdc5-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="efdc5-108">Return Type</span></span>    |<span data-ttu-id="efdc5-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efdc5-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efdc5-110">Liste bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="efdc5-110">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="efdc5-111">[BookingCurrency](bookingcurrency.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="efdc5-111">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="efdc5-112">Abrufen einer Liste von **BookingCurrency** -Objekten für ein Microsoft Bookings Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="efdc5-112">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="efdc5-113">Abrufen von bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="efdc5-113">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="efdc5-114">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="efdc5-114">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="efdc5-115">Rufen Sie die Eigenschaften eines **BookingCurrency** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="efdc5-115">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="efdc5-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="efdc5-116">Properties</span></span>
| <span data-ttu-id="efdc5-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="efdc5-117">Property</span></span>     | <span data-ttu-id="efdc5-118">Typ</span><span class="sxs-lookup"><span data-stu-id="efdc5-118">Type</span></span>   |<span data-ttu-id="efdc5-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efdc5-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efdc5-120">id</span><span class="sxs-lookup"><span data-stu-id="efdc5-120">id</span></span>|<span data-ttu-id="efdc5-121">String</span><span class="sxs-lookup"><span data-stu-id="efdc5-121">String</span></span>| <span data-ttu-id="efdc5-122">Ein 3-Zeichen Währungscode, basierend auf [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="efdc5-122">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="efdc5-123">Beispiel für US-Dollar der Währungscode ist US-Dollar und für Australien Dollar ist AUD.</span><span class="sxs-lookup"><span data-stu-id="efdc5-123">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="efdc5-124">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="efdc5-124">Read-only.</span></span>|
|<span data-ttu-id="efdc5-125">Symbol</span><span class="sxs-lookup"><span data-stu-id="efdc5-125">symbol</span></span>|<span data-ttu-id="efdc5-126">String</span><span class="sxs-lookup"><span data-stu-id="efdc5-126">String</span></span>| <span data-ttu-id="efdc5-127">Das Währungssymbol.</span><span class="sxs-lookup"><span data-stu-id="efdc5-127">The currency symbol.</span></span> <span data-ttu-id="efdc5-128">Beispielsweise ist das Währungssymbol für US-Dollar und Australien Dollar $.</span><span class="sxs-lookup"><span data-stu-id="efdc5-128">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="efdc5-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="efdc5-129">Relationships</span></span>
<span data-ttu-id="efdc5-130">Keine</span><span class="sxs-lookup"><span data-stu-id="efdc5-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="efdc5-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="efdc5-131">JSON representation</span></span>

<span data-ttu-id="efdc5-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="efdc5-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCurrency"
}-->

```json
{
  "id": "String (identifier)",
  "symbol": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcurrency.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
