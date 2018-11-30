---
title: attendee-Ressourcentyp
description: Ein Teilnehmer eines Ereignisses. Dies kann eine Person oder eine Ressource sein, wie z. B. Besprechungsräume oder Geräte, die als Ressource auf dem Exchange-Server für den Mandanten eingerichtet wurden.
ms.openlocfilehash: 7c9040b563840c22eec1dd7456892fc7ff83ee4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020133"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="6db7e-104">attendee-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6db7e-104">attendee resource type</span></span>

<span data-ttu-id="6db7e-105">Ein Teilnehmer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="6db7e-105">An event attendee.</span></span> <span data-ttu-id="6db7e-106">Dies kann eine Person oder eine Ressource sein, wie z. B. Besprechungsräume oder Geräte, die als Ressource auf dem Exchange-Server für den Mandanten eingerichtet wurden.</span><span class="sxs-lookup"><span data-stu-id="6db7e-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="6db7e-107">Abgeleitet von [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="6db7e-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6db7e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6db7e-108">Properties</span></span>
| <span data-ttu-id="6db7e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6db7e-109">Property</span></span>     | <span data-ttu-id="6db7e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6db7e-110">Type</span></span>   |<span data-ttu-id="6db7e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6db7e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6db7e-112">status</span><span class="sxs-lookup"><span data-stu-id="6db7e-112">status</span></span>|[<span data-ttu-id="6db7e-113">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="6db7e-113">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="6db7e-114">Die Antwort des Teilnehmers (keine, akzeptiert, abgelehnt, usw.) für das Ereignis und das Datum und die Uhrzeit, an dem/der die Antwort gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="6db7e-114">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="6db7e-115">Typ</span><span class="sxs-lookup"><span data-stu-id="6db7e-115">type</span></span>|<span data-ttu-id="6db7e-116">String</span><span class="sxs-lookup"><span data-stu-id="6db7e-116">String</span></span>|<span data-ttu-id="6db7e-117">Der Teilnehmertyp: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="6db7e-117">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="6db7e-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6db7e-118">emailAddress</span></span>|[<span data-ttu-id="6db7e-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6db7e-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="6db7e-120">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="6db7e-120">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6db7e-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6db7e-121">JSON representation</span></span>

<span data-ttu-id="6db7e-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6db7e-122">Here is a JSON representation of the resource</span></span>

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