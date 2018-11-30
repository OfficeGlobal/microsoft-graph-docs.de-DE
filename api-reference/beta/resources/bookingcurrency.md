---
title: Ressourcentyp bookingCurrency
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: a68b88160e42217f3605c4a4bb30f692e8dafc06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059593"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="e26d3-104">Ressourcentyp bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="e26d3-104">bookingCurrency resource type</span></span>

 > <span data-ttu-id="e26d3-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e26d3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e26d3-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e26d3-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e26d3-107">Stellt eine monetäre Währung, die von einem [BookingBusiness](bookingbusiness.md)unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e26d3-107">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="e26d3-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="e26d3-108">Methods</span></span>

| <span data-ttu-id="e26d3-109">Methode</span><span class="sxs-lookup"><span data-stu-id="e26d3-109">Method</span></span>           | <span data-ttu-id="e26d3-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e26d3-110">Return Type</span></span>    |<span data-ttu-id="e26d3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e26d3-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e26d3-112">Liste bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="e26d3-112">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="e26d3-113">[BookingCurrency](bookingcurrency.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e26d3-113">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="e26d3-114">Abrufen einer Liste von **BookingCurrency** -Objekten für ein Microsoft Bookings Unternehmen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="e26d3-114">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="e26d3-115">Abrufen von bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="e26d3-115">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="e26d3-116">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="e26d3-116">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="e26d3-117">Rufen Sie die Eigenschaften eines **BookingCurrency** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e26d3-117">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="e26d3-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e26d3-118">Properties</span></span>
| <span data-ttu-id="e26d3-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e26d3-119">Property</span></span>     | <span data-ttu-id="e26d3-120">Typ</span><span class="sxs-lookup"><span data-stu-id="e26d3-120">Type</span></span>   |<span data-ttu-id="e26d3-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e26d3-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e26d3-122">id</span><span class="sxs-lookup"><span data-stu-id="e26d3-122">id</span></span>|<span data-ttu-id="e26d3-123">String</span><span class="sxs-lookup"><span data-stu-id="e26d3-123">String</span></span>| <span data-ttu-id="e26d3-124">Ein 3-Zeichen Währungscode, basierend auf [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="e26d3-124">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="e26d3-125">Beispiel für US-Dollar der Währungscode ist US-Dollar und für Australien Dollar ist AUD.</span><span class="sxs-lookup"><span data-stu-id="e26d3-125">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="e26d3-126">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e26d3-126">Read-only.</span></span>|
|<span data-ttu-id="e26d3-127">Symbol</span><span class="sxs-lookup"><span data-stu-id="e26d3-127">symbol</span></span>|<span data-ttu-id="e26d3-128">String</span><span class="sxs-lookup"><span data-stu-id="e26d3-128">String</span></span>| <span data-ttu-id="e26d3-129">Das Währungssymbol.</span><span class="sxs-lookup"><span data-stu-id="e26d3-129">The currency symbol.</span></span> <span data-ttu-id="e26d3-130">Beispielsweise ist das Währungssymbol für US-Dollar und Australien Dollar $.</span><span class="sxs-lookup"><span data-stu-id="e26d3-130">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="e26d3-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e26d3-131">Relationships</span></span>
<span data-ttu-id="e26d3-132">Keine</span><span class="sxs-lookup"><span data-stu-id="e26d3-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e26d3-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e26d3-133">JSON representation</span></span>

<span data-ttu-id="e26d3-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e26d3-134">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->