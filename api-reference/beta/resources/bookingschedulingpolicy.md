---
title: Ressourcentyp bookingSchedulingPolicy
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 039d76b00787c9bf2e4f0bee4eb927a7628a9e76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914637"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="e070e-104">Ressourcentyp bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="e070e-104">bookingSchedulingPolicy resource type</span></span>

 > <span data-ttu-id="e070e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e070e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e070e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e070e-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e070e-107">Repräsentiert den Satz von Richtlinien, die bestimmen, wie Termine in einem Kalender Microsoft Bookings erstellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="e070e-107">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="e070e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e070e-108">Properties</span></span>
| <span data-ttu-id="e070e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e070e-109">Property</span></span>     | <span data-ttu-id="e070e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e070e-110">Type</span></span>   |<span data-ttu-id="e070e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e070e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e070e-112">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="e070e-112">allowStaffSelection</span></span>|<span data-ttu-id="e070e-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e070e-113">Boolean</span></span>|<span data-ttu-id="e070e-114">"True" If Kunden für die Buchen eine bestimmte Person auswählen können.</span><span class="sxs-lookup"><span data-stu-id="e070e-114">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="e070e-115">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="e070e-115">maximumAdvance</span></span>|<span data-ttu-id="e070e-116">Duration</span><span class="sxs-lookup"><span data-stu-id="e070e-116">Duration</span></span>|<span data-ttu-id="e070e-117">Maximale Anzahl der Tage im voraus, die ein buchen hergestellt werden kann.</span><span class="sxs-lookup"><span data-stu-id="e070e-117">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="e070e-118">Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.</span><span class="sxs-lookup"><span data-stu-id="e070e-118">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="e070e-119">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="e070e-119">minimumLeadTime</span></span>|<span data-ttu-id="e070e-120">Duration</span><span class="sxs-lookup"><span data-stu-id="e070e-120">Duration</span></span>|<span data-ttu-id="e070e-121">Die minimale Zeitspanne vor dem Buchungen und-absagen vorgenommen werden müssen.</span><span class="sxs-lookup"><span data-stu-id="e070e-121">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="e070e-122">Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.</span><span class="sxs-lookup"><span data-stu-id="e070e-122">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="e070e-123">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="e070e-123">sendConfirmationsToOwner</span></span>|<span data-ttu-id="e070e-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e070e-124">Boolean</span></span>| <span data-ttu-id="e070e-125">True, wenn das Unternehmen per e-Mail benachrichtigen, wenn ein buchen erstellt oder geändert wird.</span><span class="sxs-lookup"><span data-stu-id="e070e-125">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="e070e-126">Verwenden Sie die e-Mail-Adresse in der **e-Mail** -Eigenschaft der Entität **BookingBusiness** für das Unternehmen angegeben.</span><span class="sxs-lookup"><span data-stu-id="e070e-126">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="e070e-127">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="e070e-127">timeSlotInterval</span></span>|<span data-ttu-id="e070e-128">Duration</span><span class="sxs-lookup"><span data-stu-id="e070e-128">Duration</span></span>|<span data-ttu-id="e070e-129">Dauer der jedes Zeitintervall im [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="e070e-129">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e070e-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e070e-130">JSON representation</span></span>

<span data-ttu-id="e070e-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e070e-131">The following is a JSON representation of the resource.</span></span>

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
