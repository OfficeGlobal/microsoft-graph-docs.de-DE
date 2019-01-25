---
title: Ressourcentyp „attendeeBase“
description: Der Typ eines Teilnehmers.
localization_priority: Normal
ms.openlocfilehash: bce1550c107f2114d02744091b5863360ab0bcea
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517456"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="a3369-103">Ressourcentyp „attendeeBase“</span><span class="sxs-lookup"><span data-stu-id="a3369-103">attendeeBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3369-104">Der Typ eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="a3369-104">The type of attendee.</span></span>

<span data-ttu-id="a3369-105">Abgeleitet von [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="a3369-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3369-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a3369-106">JSON representation</span></span>

<span data-ttu-id="a3369-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a3369-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="a3369-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a3369-108">Properties</span></span>
| <span data-ttu-id="a3369-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a3369-109">Property</span></span>     | <span data-ttu-id="a3369-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a3369-110">Type</span></span>   |<span data-ttu-id="a3369-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3369-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3369-112">type</span><span class="sxs-lookup"><span data-stu-id="a3369-112">type</span></span>|<span data-ttu-id="a3369-113">String</span><span class="sxs-lookup"><span data-stu-id="a3369-113">String</span></span>| <span data-ttu-id="a3369-p101">Der Typ eines Teilnehmers. Mögliche Werte sind: `required`, `optional` und `resource`. Ist der Teilnehmer eine Person, geht [findMeetingTimes](../api/user-findmeetingtimes.md) aktuell grundsätzlich davon aus, dass diese Person vom Typ `Required` ist.</span><span class="sxs-lookup"><span data-stu-id="a3369-p101">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="a3369-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a3369-117">emailAddress</span></span>|[<span data-ttu-id="a3369-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a3369-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a3369-119">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="a3369-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeebase.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
