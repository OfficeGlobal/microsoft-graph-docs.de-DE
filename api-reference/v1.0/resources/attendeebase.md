---
title: Ressourcentyp „attendeeBase“
description: Der Typ eines Teilnehmers.
ms.openlocfilehash: 6995ac94a600a60313ef26208b441c6ef6fdf001
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018634"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="91196-103">Ressourcentyp „attendeeBase“</span><span class="sxs-lookup"><span data-stu-id="91196-103">attendeeBase resource type</span></span>

<span data-ttu-id="91196-104">Der Typ eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="91196-104">The type of attendee.</span></span>

<span data-ttu-id="91196-105">Abgeleitet von [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="91196-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="91196-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91196-106">JSON representation</span></span>

<span data-ttu-id="91196-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91196-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="91196-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91196-108">Properties</span></span>
| <span data-ttu-id="91196-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91196-109">Property</span></span>     | <span data-ttu-id="91196-110">Typ</span><span class="sxs-lookup"><span data-stu-id="91196-110">Type</span></span>   |<span data-ttu-id="91196-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91196-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91196-112">Typ</span><span class="sxs-lookup"><span data-stu-id="91196-112">type</span></span>|<span data-ttu-id="91196-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="91196-113">attendeeType</span></span>| <span data-ttu-id="91196-114">Der Typ eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="91196-114">The type of attendee.</span></span> <span data-ttu-id="91196-115">Die möglichen Werte sind: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="91196-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="91196-116">Derzeit Wenn Teilnehmer einer Person ist, [FindMeetingTimes](../api/user-findmeetingtimes.md) immer berücksichtigt die Person ist, der die `Required` Typ.</span><span class="sxs-lookup"><span data-stu-id="91196-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="91196-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="91196-117">emailAddress</span></span>|[<span data-ttu-id="91196-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="91196-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="91196-119">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="91196-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
