---
title: Ressourcentyp bookingReminder
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0e5188a5a440134d11404c102b4641fc98cad04f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526081"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="62348-104">Ressourcentyp bookingReminder</span><span class="sxs-lookup"><span data-stu-id="62348-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="62348-105">Stellt dar, wann und an eine e-Mail-Benachrichtigung gesendet.</span><span class="sxs-lookup"><span data-stu-id="62348-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="62348-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="62348-106">Properties</span></span>
| <span data-ttu-id="62348-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="62348-107">Property</span></span>     | <span data-ttu-id="62348-108">Typ</span><span class="sxs-lookup"><span data-stu-id="62348-108">Type</span></span>   |<span data-ttu-id="62348-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62348-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62348-110">message</span><span class="sxs-lookup"><span data-stu-id="62348-110">message</span></span>|<span data-ttu-id="62348-111">String</span><span class="sxs-lookup"><span data-stu-id="62348-111">String</span></span>|<span data-ttu-id="62348-112">Die Nachricht in der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="62348-112">The message in the reminder.</span></span>|
|<span data-ttu-id="62348-113">OFFSET</span><span class="sxs-lookup"><span data-stu-id="62348-113">offset</span></span>|<span data-ttu-id="62348-114">Dauer</span><span class="sxs-lookup"><span data-stu-id="62348-114">Duration</span></span>|<span data-ttu-id="62348-115">Der Zeitraum vor dem Beginn des Termins, die die Erinnerung gesendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="62348-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="62348-116">Es wird im [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) -Format angegeben.</span><span class="sxs-lookup"><span data-stu-id="62348-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="62348-117">recipients</span><span class="sxs-lookup"><span data-stu-id="62348-117">recipients</span></span>|<span data-ttu-id="62348-118">String</span><span class="sxs-lookup"><span data-stu-id="62348-118">String</span></span>| <span data-ttu-id="62348-119">Die Personen, die empfangen müssen die Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="62348-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="62348-120">Mögliche Werte sind: `allAttendees`, `staff` und `customer`.</span><span class="sxs-lookup"><span data-stu-id="62348-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62348-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="62348-121">JSON representation</span></span>

<span data-ttu-id="62348-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="62348-122">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
