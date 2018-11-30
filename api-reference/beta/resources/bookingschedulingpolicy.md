---
title: Ressourcentyp bookingSchedulingPolicy
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 7a16e9a2ec4e64978dd3c20f7510cfd42d76e826
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061566"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="97e6a-104">Ressourcentyp bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="97e6a-104">bookingSchedulingPolicy resource type</span></span>

 > <span data-ttu-id="97e6a-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="97e6a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97e6a-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97e6a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="97e6a-107">Repräsentiert den Satz von Richtlinien, die bestimmen, wie Termine in einem Kalender Microsoft Bookings erstellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="97e6a-107">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="97e6a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="97e6a-108">Properties</span></span>
| <span data-ttu-id="97e6a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97e6a-109">Property</span></span>     | <span data-ttu-id="97e6a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="97e6a-110">Type</span></span>   |<span data-ttu-id="97e6a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97e6a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97e6a-112">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="97e6a-112">allowStaffSelection</span></span>|<span data-ttu-id="97e6a-113">Boolesch</span><span class="sxs-lookup"><span data-stu-id="97e6a-113">Boolean</span></span>|<span data-ttu-id="97e6a-114">"True" If Kunden für die Buchen eine bestimmte Person auswählen können.</span><span class="sxs-lookup"><span data-stu-id="97e6a-114">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="97e6a-115">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="97e6a-115">maximumAdvance</span></span>|<span data-ttu-id="97e6a-116">Duration</span><span class="sxs-lookup"><span data-stu-id="97e6a-116">Duration</span></span>|<span data-ttu-id="97e6a-117">Maximale Anzahl der Tage im voraus, die ein buchen hergestellt werden kann.</span><span class="sxs-lookup"><span data-stu-id="97e6a-117">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="97e6a-118">Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.</span><span class="sxs-lookup"><span data-stu-id="97e6a-118">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="97e6a-119">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="97e6a-119">minimumLeadTime</span></span>|<span data-ttu-id="97e6a-120">Duration</span><span class="sxs-lookup"><span data-stu-id="97e6a-120">Duration</span></span>|<span data-ttu-id="97e6a-121">Die minimale Zeitspanne vor dem Buchungen und-absagen vorgenommen werden müssen.</span><span class="sxs-lookup"><span data-stu-id="97e6a-121">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="97e6a-122">Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.</span><span class="sxs-lookup"><span data-stu-id="97e6a-122">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="97e6a-123">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="97e6a-123">sendConfirmationsToOwner</span></span>|<span data-ttu-id="97e6a-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="97e6a-124">Boolean</span></span>| <span data-ttu-id="97e6a-125">True, wenn das Unternehmen per e-Mail benachrichtigen, wenn ein buchen erstellt oder geändert wird.</span><span class="sxs-lookup"><span data-stu-id="97e6a-125">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="97e6a-126">Verwenden Sie die e-Mail-Adresse in der **e-Mail** -Eigenschaft der Entität **BookingBusiness** für das Unternehmen angegeben.</span><span class="sxs-lookup"><span data-stu-id="97e6a-126">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="97e6a-127">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="97e6a-127">timeSlotInterval</span></span>|<span data-ttu-id="97e6a-128">Duration</span><span class="sxs-lookup"><span data-stu-id="97e6a-128">Duration</span></span>|<span data-ttu-id="97e6a-129">Dauer der jedes Zeitintervall im [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="97e6a-129">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97e6a-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="97e6a-130">JSON representation</span></span>

<span data-ttu-id="97e6a-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="97e6a-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->