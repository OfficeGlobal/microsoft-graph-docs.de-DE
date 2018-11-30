---
title: Ressourcentyp bookingReminder
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: f5f7b30c296433dd96ffa14a75e3f0286e8a16a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062340"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="eace3-104">Ressourcentyp bookingReminder</span><span class="sxs-lookup"><span data-stu-id="eace3-104">bookingReminder resource type</span></span>

 > <span data-ttu-id="eace3-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eace3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eace3-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eace3-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="eace3-107">Stellt dar, wann und an eine e-Mail-Benachrichtigung gesendet.</span><span class="sxs-lookup"><span data-stu-id="eace3-107">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="eace3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eace3-108">Properties</span></span>
| <span data-ttu-id="eace3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eace3-109">Property</span></span>     | <span data-ttu-id="eace3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="eace3-110">Type</span></span>   |<span data-ttu-id="eace3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eace3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eace3-112">message</span><span class="sxs-lookup"><span data-stu-id="eace3-112">message</span></span>|<span data-ttu-id="eace3-113">String</span><span class="sxs-lookup"><span data-stu-id="eace3-113">String</span></span>|<span data-ttu-id="eace3-114">Die Nachricht in der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="eace3-114">The message in the reminder.</span></span>|
|<span data-ttu-id="eace3-115">Offset</span><span class="sxs-lookup"><span data-stu-id="eace3-115">offset</span></span>|<span data-ttu-id="eace3-116">Duration</span><span class="sxs-lookup"><span data-stu-id="eace3-116">Duration</span></span>|<span data-ttu-id="eace3-117">Der Zeitraum vor dem Beginn des Termins, die die Erinnerung gesendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="eace3-117">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="eace3-118">Es wird im [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format angegeben.</span><span class="sxs-lookup"><span data-stu-id="eace3-118">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="eace3-119">recipients</span><span class="sxs-lookup"><span data-stu-id="eace3-119">recipients</span></span>|<span data-ttu-id="eace3-120">String</span><span class="sxs-lookup"><span data-stu-id="eace3-120">String</span></span>| <span data-ttu-id="eace3-121">Die Personen, die empfangen müssen die Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="eace3-121">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="eace3-122">Mögliche Werte sind: `allAttendees`, `staff` und `customer`.</span><span class="sxs-lookup"><span data-stu-id="eace3-122">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eace3-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eace3-123">JSON representation</span></span>

<span data-ttu-id="eace3-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eace3-124">The following is a JSON representation of the resource.</span></span>

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