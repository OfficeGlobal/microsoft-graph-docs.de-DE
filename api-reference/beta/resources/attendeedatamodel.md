---
title: attendeeDataModel-Ressourcentyp
description: Der Typ eines Teilnehmers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e8659b88cae8b9d2a94177593da40b61363fa23b
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057387"
---
# <a name="attendeedatamodel-resource-type"></a><span data-ttu-id="a33d8-103">attendeeDataModel-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a33d8-103">attendeeDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a33d8-104">Stellt eine Person oder Ressource dar, die in einer Besprechung eingeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="a33d8-104">Represents a person or resource who is being included in a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a33d8-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a33d8-105">JSON representation</span></span>

<span data-ttu-id="a33d8-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a33d8-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "type"
  ],
  "@odata.type": "microsoft.graph.attendeeDataModel"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="a33d8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a33d8-107">Properties</span></span>
| <span data-ttu-id="a33d8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a33d8-108">Property</span></span>     | <span data-ttu-id="a33d8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a33d8-109">Type</span></span>   |<span data-ttu-id="a33d8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a33d8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a33d8-111">type</span><span class="sxs-lookup"><span data-stu-id="a33d8-111">type</span></span>|<span data-ttu-id="a33d8-112">attendeeType</span><span class="sxs-lookup"><span data-stu-id="a33d8-112">attendeeType</span></span>| <span data-ttu-id="a33d8-113">Der Typ eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="a33d8-113">The type of attendee.</span></span> <span data-ttu-id="a33d8-114">Die möglichen Werte sind: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="a33d8-114">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="a33d8-115">Wenn es sich bei dem Teilnehmer um eine Person handelt, ist [findMeetingTimes](../api/user-findmeetingtimes.md) immer der `required` Typ der Person.</span><span class="sxs-lookup"><span data-stu-id="a33d8-115">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `required` type.</span></span>|
|<span data-ttu-id="a33d8-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a33d8-116">emailAddress</span></span>|[<span data-ttu-id="a33d8-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a33d8-117">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a33d8-118">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="a33d8-118">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeedatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->