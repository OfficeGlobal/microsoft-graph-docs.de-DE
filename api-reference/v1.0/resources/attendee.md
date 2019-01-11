---
title: attendee-Ressourcentyp
description: Ein Teilnehmer eines Ereignisses. Dies kann eine Person oder eine Ressource sein, wie z. B. Besprechungsräume oder Geräte, die als Ressource auf dem Exchange-Server für den Mandanten eingerichtet wurden.
localization_priority: Normal
ms.openlocfilehash: 89c289a342bb0b761bed982f88d0f47470eaa237
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856539"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="33874-104">attendee-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="33874-104">attendee resource type</span></span>

<span data-ttu-id="33874-105">Ein Teilnehmer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="33874-105">An event attendee.</span></span> <span data-ttu-id="33874-106">Dies kann eine Person oder eine Ressource sein, wie z. B. Besprechungsräume oder Geräte, die als Ressource auf dem Exchange-Server für den Mandanten eingerichtet wurden.</span><span class="sxs-lookup"><span data-stu-id="33874-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="33874-107">Abgeleitet von [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="33874-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="33874-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="33874-108">Properties</span></span>
| <span data-ttu-id="33874-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33874-109">Property</span></span>     | <span data-ttu-id="33874-110">Typ</span><span class="sxs-lookup"><span data-stu-id="33874-110">Type</span></span>   |<span data-ttu-id="33874-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33874-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33874-112">status</span><span class="sxs-lookup"><span data-stu-id="33874-112">status</span></span>|[<span data-ttu-id="33874-113">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="33874-113">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="33874-114">Die Antwort des Teilnehmers (keine, akzeptiert, abgelehnt, usw.) für das Ereignis und das Datum und die Uhrzeit, an dem/der die Antwort gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="33874-114">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="33874-115">Typ</span><span class="sxs-lookup"><span data-stu-id="33874-115">type</span></span>|<span data-ttu-id="33874-116">String</span><span class="sxs-lookup"><span data-stu-id="33874-116">String</span></span>|<span data-ttu-id="33874-117">Der Teilnehmertyp: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="33874-117">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="33874-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="33874-118">emailAddress</span></span>|[<span data-ttu-id="33874-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="33874-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="33874-120">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="33874-120">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33874-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="33874-121">JSON representation</span></span>

<span data-ttu-id="33874-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="33874-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
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
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
