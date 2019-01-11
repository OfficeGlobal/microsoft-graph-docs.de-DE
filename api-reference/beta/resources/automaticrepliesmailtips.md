---
title: Ressourcentyp automaticRepliesMailTips
description: E-Mail-Infos zu automatischen Antworten, die für ein Postfach festgelegt wurden.
localization_priority: Normal
ms.openlocfilehash: 80ecaaa9fced0bcb00494b0414a86f0a11fd8996
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833229"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="c1a0a-103">Ressourcentyp automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="c1a0a-103">automaticRepliesMailTips resource type</span></span>

> <span data-ttu-id="c1a0a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c1a0a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1a0a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1a0a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1a0a-106">[E-Mail-Infos](../resources/mailtips.md) zu automatischen Antworten, die für ein Postfach festgelegt wurden.</span><span class="sxs-lookup"><span data-stu-id="c1a0a-106">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="c1a0a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c1a0a-107">Properties</span></span>
| <span data-ttu-id="c1a0a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1a0a-108">Property</span></span>     | <span data-ttu-id="c1a0a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c1a0a-109">Type</span></span>   |<span data-ttu-id="c1a0a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1a0a-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="c1a0a-111">message</span><span class="sxs-lookup"><span data-stu-id="c1a0a-111">message</span></span> | <span data-ttu-id="c1a0a-112">String</span><span class="sxs-lookup"><span data-stu-id="c1a0a-112">String</span></span> | <span data-ttu-id="c1a0a-113">Die automatische Antwortnachricht.</span><span class="sxs-lookup"><span data-stu-id="c1a0a-113">The automatic reply message.</span></span> |
| <span data-ttu-id="c1a0a-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="c1a0a-114">messageLanguage</span></span> | [<span data-ttu-id="c1a0a-115">localeInfo</span><span class="sxs-lookup"><span data-stu-id="c1a0a-115">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="c1a0a-116">Die Sprache, der in die automatische Antwort ist.</span><span class="sxs-lookup"><span data-stu-id="c1a0a-116">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="c1a0a-117">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="c1a0a-117">scheduledEndTime</span></span> | [<span data-ttu-id="c1a0a-118">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c1a0a-118">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="c1a0a-119">Das Datum und die Uhrzeit, die automatische Antworten für das Ende festgelegt sind.</span><span class="sxs-lookup"><span data-stu-id="c1a0a-119">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="c1a0a-120">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="c1a0a-120">scheduledStartTime</span></span> | [<span data-ttu-id="c1a0a-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c1a0a-121">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="c1a0a-122">Das Datum und die Uhrzeit, die automatische Antworten beginnen festgelegt sind.</span><span class="sxs-lookup"><span data-stu-id="c1a0a-122">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c1a0a-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c1a0a-123">JSON representation</span></span>

<span data-ttu-id="c1a0a-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c1a0a-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
