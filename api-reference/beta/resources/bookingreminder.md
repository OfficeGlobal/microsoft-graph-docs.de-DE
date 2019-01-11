---
title: Ressourcentyp bookingReminder
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 1f1708d4ac9606ad5c862cb9b1bc73e1ddcfec4a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853865"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="1539c-104">Ressourcentyp bookingReminder</span><span class="sxs-lookup"><span data-stu-id="1539c-104">bookingReminder resource type</span></span>

 > <span data-ttu-id="1539c-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1539c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1539c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1539c-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="1539c-107">Stellt dar, wann und an eine e-Mail-Benachrichtigung gesendet.</span><span class="sxs-lookup"><span data-stu-id="1539c-107">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="1539c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1539c-108">Properties</span></span>
| <span data-ttu-id="1539c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1539c-109">Property</span></span>     | <span data-ttu-id="1539c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1539c-110">Type</span></span>   |<span data-ttu-id="1539c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1539c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1539c-112">message</span><span class="sxs-lookup"><span data-stu-id="1539c-112">message</span></span>|<span data-ttu-id="1539c-113">String</span><span class="sxs-lookup"><span data-stu-id="1539c-113">String</span></span>|<span data-ttu-id="1539c-114">Die Nachricht in der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="1539c-114">The message in the reminder.</span></span>|
|<span data-ttu-id="1539c-115">Offset</span><span class="sxs-lookup"><span data-stu-id="1539c-115">offset</span></span>|<span data-ttu-id="1539c-116">Duration</span><span class="sxs-lookup"><span data-stu-id="1539c-116">Duration</span></span>|<span data-ttu-id="1539c-117">Der Zeitraum vor dem Beginn des Termins, die die Erinnerung gesendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1539c-117">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="1539c-118">Es wird im [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format angegeben.</span><span class="sxs-lookup"><span data-stu-id="1539c-118">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="1539c-119">recipients</span><span class="sxs-lookup"><span data-stu-id="1539c-119">recipients</span></span>|<span data-ttu-id="1539c-120">String</span><span class="sxs-lookup"><span data-stu-id="1539c-120">String</span></span>| <span data-ttu-id="1539c-121">Die Personen, die empfangen müssen die Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="1539c-121">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="1539c-122">Mögliche Werte sind: `allAttendees`, `staff` und `customer`.</span><span class="sxs-lookup"><span data-stu-id="1539c-122">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1539c-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1539c-123">JSON representation</span></span>

<span data-ttu-id="1539c-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1539c-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingReminder"
}-->

```json
{
  "message": "String",
  "offset": "String (timestamp)",
  "recipients": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
