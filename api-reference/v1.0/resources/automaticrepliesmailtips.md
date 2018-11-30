---
title: Ressourcentyp automaticRepliesMailTips
description: E-Mail-Infos zu automatischen Antworten, die für ein Postfach festgelegt wurden.
ms.openlocfilehash: 943a465671c777305e5623104c82f377ff9496dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018005"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="d28a4-103">Ressourcentyp automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="d28a4-103">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="d28a4-104">[E-Mail-Infos](../resources/mailtips.md) zu automatischen Antworten, die für ein Postfach festgelegt wurden.</span><span class="sxs-lookup"><span data-stu-id="d28a4-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="d28a4-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d28a4-105">Properties</span></span>
| <span data-ttu-id="d28a4-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d28a4-106">Property</span></span>     | <span data-ttu-id="d28a4-107">Typ</span><span class="sxs-lookup"><span data-stu-id="d28a4-107">Type</span></span>   |<span data-ttu-id="d28a4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d28a4-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="d28a4-109">message</span><span class="sxs-lookup"><span data-stu-id="d28a4-109">message</span></span> | <span data-ttu-id="d28a4-110">String</span><span class="sxs-lookup"><span data-stu-id="d28a4-110">String</span></span> | <span data-ttu-id="d28a4-111">Die automatische Antwortnachricht.</span><span class="sxs-lookup"><span data-stu-id="d28a4-111">The automatic reply message.</span></span> |
| <span data-ttu-id="d28a4-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="d28a4-112">messageLanguage</span></span> | [<span data-ttu-id="d28a4-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="d28a4-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="d28a4-114">Die Sprache, der in die automatische Antwort ist.</span><span class="sxs-lookup"><span data-stu-id="d28a4-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="d28a4-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="d28a4-115">scheduledEndTime</span></span> | [<span data-ttu-id="d28a4-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d28a4-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="d28a4-117">Das Datum und die Uhrzeit, die automatische Antworten für das Ende festgelegt sind.</span><span class="sxs-lookup"><span data-stu-id="d28a4-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="d28a4-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="d28a4-118">scheduledStartTime</span></span> | [<span data-ttu-id="d28a4-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d28a4-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="d28a4-120">Das Datum und die Uhrzeit, die automatische Antworten beginnen festgelegt sind.</span><span class="sxs-lookup"><span data-stu-id="d28a4-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d28a4-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d28a4-121">JSON representation</span></span>

<span data-ttu-id="d28a4-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d28a4-122">Here is a JSON representation of the resource.</span></span>

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