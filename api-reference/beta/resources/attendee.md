---
title: attendee-Ressourcentyp
description: Ein Teilnehmer eines Ereignisses. Dies kann eine Person oder eine Ressource sein, wie z. B. Besprechungsräume oder Geräte, die als Ressource auf dem Exchange-Server für den Mandanten eingerichtet wurden.
localization_priority: Normal
ms.openlocfilehash: d50b6756c7d0077ec95f10988d06fa2ff81631fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529313"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="e94ac-104">attendee-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e94ac-104">attendee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e94ac-105">Ein Teilnehmer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="e94ac-105">An event attendee.</span></span> <span data-ttu-id="e94ac-106">Dies kann eine Person oder eine Ressource sein, wie z. B. Besprechungsräume oder Geräte, die als Ressource auf dem Exchange-Server für den Mandanten eingerichtet wurden.</span><span class="sxs-lookup"><span data-stu-id="e94ac-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="e94ac-107">Abgeleitet von [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="e94ac-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e94ac-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e94ac-108">Properties</span></span>
| <span data-ttu-id="e94ac-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e94ac-109">Property</span></span>     | <span data-ttu-id="e94ac-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e94ac-110">Type</span></span>   |<span data-ttu-id="e94ac-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e94ac-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e94ac-112">status</span><span class="sxs-lookup"><span data-stu-id="e94ac-112">status</span></span>|[<span data-ttu-id="e94ac-113">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="e94ac-113">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="e94ac-114">Die Antwort des Teilnehmers (keine, akzeptiert, abgelehnt, usw.) für das Ereignis und das Datum und die Uhrzeit, an dem/der die Antwort gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="e94ac-114">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="e94ac-115">Typ</span><span class="sxs-lookup"><span data-stu-id="e94ac-115">type</span></span>|<span data-ttu-id="e94ac-116">String</span><span class="sxs-lookup"><span data-stu-id="e94ac-116">String</span></span>|<span data-ttu-id="e94ac-117">Der Teilnehmertyp: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="e94ac-117">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="e94ac-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e94ac-118">emailAddress</span></span>|[<span data-ttu-id="e94ac-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e94ac-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="e94ac-120">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="e94ac-120">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e94ac-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e94ac-121">JSON representation</span></span>

<span data-ttu-id="e94ac-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e94ac-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendee.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
