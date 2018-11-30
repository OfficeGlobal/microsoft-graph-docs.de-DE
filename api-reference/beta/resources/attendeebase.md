---
title: Ressourcentyp „attendeeBase“
description: Der Typ eines Teilnehmers.
ms.openlocfilehash: 2d7d3889cd65886eba4cf9356862417928ed3296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058142"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="a93da-103">Ressourcentyp „attendeeBase“</span><span class="sxs-lookup"><span data-stu-id="a93da-103">attendeeBase resource type</span></span>

> <span data-ttu-id="a93da-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a93da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a93da-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a93da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a93da-106">Der Typ eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="a93da-106">The type of attendee.</span></span>

<span data-ttu-id="a93da-107">Abgeleitet von [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="a93da-107">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a93da-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a93da-108">JSON representation</span></span>

<span data-ttu-id="a93da-109">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a93da-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a93da-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a93da-110">Properties</span></span>
| <span data-ttu-id="a93da-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a93da-111">Property</span></span>     | <span data-ttu-id="a93da-112">Typ</span><span class="sxs-lookup"><span data-stu-id="a93da-112">Type</span></span>   |<span data-ttu-id="a93da-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a93da-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a93da-114">Typ</span><span class="sxs-lookup"><span data-stu-id="a93da-114">type</span></span>|<span data-ttu-id="a93da-115">String</span><span class="sxs-lookup"><span data-stu-id="a93da-115">String</span></span>| <span data-ttu-id="a93da-p102">Der Typ eines Teilnehmers. Mögliche Werte sind: `required`, `optional` und `resource`. Ist der Teilnehmer eine Person, geht [findMeetingTimes](../api/user-findmeetingtimes.md) aktuell grundsätzlich davon aus, dass diese Person vom Typ `Required` ist.</span><span class="sxs-lookup"><span data-stu-id="a93da-p102">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="a93da-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a93da-119">emailAddress</span></span>|[<span data-ttu-id="a93da-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a93da-120">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a93da-121">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="a93da-121">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->