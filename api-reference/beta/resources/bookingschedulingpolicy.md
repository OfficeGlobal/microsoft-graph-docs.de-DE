---
title: Ressourcentyp bookingSchedulingPolicy
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3dee3314818d46c4131526dc92565eb4f8ca6ea2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523449"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="88a00-104">Ressourcentyp bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="88a00-104">bookingSchedulingPolicy resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="88a00-105">Repräsentiert den Satz von Richtlinien, die bestimmen, wie Termine in einem Kalender Microsoft Bookings erstellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="88a00-105">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="88a00-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88a00-106">Properties</span></span>
| <span data-ttu-id="88a00-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88a00-107">Property</span></span>     | <span data-ttu-id="88a00-108">Typ</span><span class="sxs-lookup"><span data-stu-id="88a00-108">Type</span></span>   |<span data-ttu-id="88a00-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88a00-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88a00-110">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="88a00-110">allowStaffSelection</span></span>|<span data-ttu-id="88a00-111">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="88a00-111">Boolean</span></span>|<span data-ttu-id="88a00-112">"True" If Kunden für die Buchen eine bestimmte Person auswählen können.</span><span class="sxs-lookup"><span data-stu-id="88a00-112">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="88a00-113">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="88a00-113">maximumAdvance</span></span>|<span data-ttu-id="88a00-114">Dauer</span><span class="sxs-lookup"><span data-stu-id="88a00-114">Duration</span></span>|<span data-ttu-id="88a00-115">Maximale Anzahl der Tage im voraus, die ein buchen hergestellt werden kann.</span><span class="sxs-lookup"><span data-stu-id="88a00-115">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="88a00-116">Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.</span><span class="sxs-lookup"><span data-stu-id="88a00-116">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="88a00-117">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="88a00-117">minimumLeadTime</span></span>|<span data-ttu-id="88a00-118">Dauer</span><span class="sxs-lookup"><span data-stu-id="88a00-118">Duration</span></span>|<span data-ttu-id="88a00-119">Die minimale Zeitspanne vor dem Buchungen und-absagen vorgenommen werden müssen.</span><span class="sxs-lookup"><span data-stu-id="88a00-119">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="88a00-120">Es folgt das [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format.</span><span class="sxs-lookup"><span data-stu-id="88a00-120">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="88a00-121">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="88a00-121">sendConfirmationsToOwner</span></span>|<span data-ttu-id="88a00-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="88a00-122">Boolean</span></span>| <span data-ttu-id="88a00-123">True, wenn das Unternehmen per e-Mail benachrichtigen, wenn ein buchen erstellt oder geändert wird.</span><span class="sxs-lookup"><span data-stu-id="88a00-123">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="88a00-124">Verwenden Sie die e-Mail-Adresse in der **e-Mail** -Eigenschaft der Entität **BookingBusiness** für das Unternehmen angegeben.</span><span class="sxs-lookup"><span data-stu-id="88a00-124">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="88a00-125">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="88a00-125">timeSlotInterval</span></span>|<span data-ttu-id="88a00-126">Dauer</span><span class="sxs-lookup"><span data-stu-id="88a00-126">Duration</span></span>|<span data-ttu-id="88a00-127">Dauer der jedes Zeitintervall im [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="88a00-127">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88a00-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88a00-128">JSON representation</span></span>

<span data-ttu-id="88a00-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88a00-129">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingschedulingpolicy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
