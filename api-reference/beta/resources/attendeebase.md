---
title: Ressourcentyp „attendeeBase“
description: Der Typ eines Teilnehmers.
localization_priority: Normal
ms.openlocfilehash: b30e054e6d89765d280340b31355403739381c2a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844982"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="f3ccc-103">Ressourcentyp „attendeeBase“</span><span class="sxs-lookup"><span data-stu-id="f3ccc-103">attendeeBase resource type</span></span>

> <span data-ttu-id="f3ccc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f3ccc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3ccc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3ccc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3ccc-106">Der Typ eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="f3ccc-106">The type of attendee.</span></span>

<span data-ttu-id="f3ccc-107">Abgeleitet von [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="f3ccc-107">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3ccc-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f3ccc-108">JSON representation</span></span>

<span data-ttu-id="f3ccc-109">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f3ccc-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f3ccc-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f3ccc-110">Properties</span></span>
| <span data-ttu-id="f3ccc-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f3ccc-111">Property</span></span>     | <span data-ttu-id="f3ccc-112">Typ</span><span class="sxs-lookup"><span data-stu-id="f3ccc-112">Type</span></span>   |<span data-ttu-id="f3ccc-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3ccc-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3ccc-114">type</span><span class="sxs-lookup"><span data-stu-id="f3ccc-114">type</span></span>|<span data-ttu-id="f3ccc-115">String</span><span class="sxs-lookup"><span data-stu-id="f3ccc-115">String</span></span>| <span data-ttu-id="f3ccc-p102">Der Typ eines Teilnehmers. Mögliche Werte sind: `required`, `optional` und `resource`. Ist der Teilnehmer eine Person, geht [findMeetingTimes](../api/user-findmeetingtimes.md) aktuell grundsätzlich davon aus, dass diese Person vom Typ `Required` ist.</span><span class="sxs-lookup"><span data-stu-id="f3ccc-p102">The type of attendee. Possible values are: `required`, `optional`, `resource`. Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="f3ccc-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f3ccc-119">emailAddress</span></span>|[<span data-ttu-id="f3ccc-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f3ccc-120">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="f3ccc-121">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="f3ccc-121">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
