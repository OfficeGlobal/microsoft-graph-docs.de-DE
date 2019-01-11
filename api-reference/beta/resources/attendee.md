---
title: attendee-Ressourcentyp
description: Ein Teilnehmer eines Ereignisses. Dies kann eine Person oder eine Ressource sein, wie z. B. Besprechungsräume oder Geräte, die als Ressource auf dem Exchange-Server für den Mandanten eingerichtet wurden.
localization_priority: Normal
ms.openlocfilehash: 95881d0e2f3dfe51b975e60ba6f8d32cda5e222c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859325"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="14375-104">attendee-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="14375-104">attendee resource type</span></span>

> <span data-ttu-id="14375-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="14375-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14375-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="14375-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14375-107">Ein Teilnehmer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="14375-107">An event attendee.</span></span> <span data-ttu-id="14375-108">Dies kann eine Person oder eine Ressource sein, wie z. B. Besprechungsräume oder Geräte, die als Ressource auf dem Exchange-Server für den Mandanten eingerichtet wurden.</span><span class="sxs-lookup"><span data-stu-id="14375-108">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="14375-109">Abgeleitet von [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="14375-109">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="14375-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="14375-110">Properties</span></span>
| <span data-ttu-id="14375-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14375-111">Property</span></span>     | <span data-ttu-id="14375-112">Typ</span><span class="sxs-lookup"><span data-stu-id="14375-112">Type</span></span>   |<span data-ttu-id="14375-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14375-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14375-114">status</span><span class="sxs-lookup"><span data-stu-id="14375-114">status</span></span>|[<span data-ttu-id="14375-115">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="14375-115">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="14375-116">Die Antwort des Teilnehmers (keine, akzeptiert, abgelehnt, usw.) für das Ereignis und das Datum und die Uhrzeit, an dem/der die Antwort gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="14375-116">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="14375-117">Typ</span><span class="sxs-lookup"><span data-stu-id="14375-117">type</span></span>|<span data-ttu-id="14375-118">String</span><span class="sxs-lookup"><span data-stu-id="14375-118">String</span></span>|<span data-ttu-id="14375-119">Der Teilnehmertyp: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="14375-119">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="14375-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="14375-120">emailAddress</span></span>|[<span data-ttu-id="14375-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="14375-121">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="14375-122">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="14375-122">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14375-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="14375-123">JSON representation</span></span>

<span data-ttu-id="14375-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="14375-124">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
