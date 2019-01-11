---
title: Ressourcentyp „attendeeBase“
description: Der Typ eines Teilnehmers.
localization_priority: Normal
ms.openlocfilehash: d009ef6a58c63017addf8b8a1bdecc1974abbff3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878673"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="59fc3-103">Ressourcentyp „attendeeBase“</span><span class="sxs-lookup"><span data-stu-id="59fc3-103">attendeeBase resource type</span></span>

<span data-ttu-id="59fc3-104">Der Typ eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="59fc3-104">The type of attendee.</span></span>

<span data-ttu-id="59fc3-105">Abgeleitet von [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="59fc3-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="59fc3-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="59fc3-106">JSON representation</span></span>

<span data-ttu-id="59fc3-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="59fc3-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="59fc3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="59fc3-108">Properties</span></span>
| <span data-ttu-id="59fc3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="59fc3-109">Property</span></span>     | <span data-ttu-id="59fc3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="59fc3-110">Type</span></span>   |<span data-ttu-id="59fc3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59fc3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59fc3-112">type</span><span class="sxs-lookup"><span data-stu-id="59fc3-112">type</span></span>|<span data-ttu-id="59fc3-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="59fc3-113">attendeeType</span></span>| <span data-ttu-id="59fc3-114">Der Typ eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="59fc3-114">The type of attendee.</span></span> <span data-ttu-id="59fc3-115">Die möglichen Werte sind: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="59fc3-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="59fc3-116">Derzeit Wenn Teilnehmer einer Person ist, [FindMeetingTimes](../api/user-findmeetingtimes.md) immer berücksichtigt die Person ist, der die `Required` Typ.</span><span class="sxs-lookup"><span data-stu-id="59fc3-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="59fc3-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="59fc3-117">emailAddress</span></span>|[<span data-ttu-id="59fc3-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="59fc3-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="59fc3-119">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="59fc3-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
