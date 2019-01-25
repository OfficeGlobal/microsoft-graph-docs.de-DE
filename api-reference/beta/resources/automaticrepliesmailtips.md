---
title: Ressourcentyp automaticRepliesMailTips
description: E-Mail-Infos zu automatischen Antworten, die für ein Postfach festgelegt wurden.
localization_priority: Normal
ms.openlocfilehash: 7eb9d57da427090c554e111ae6ba1eeb369437ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513676"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="a9259-103">Ressourcentyp automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="a9259-103">automaticRepliesMailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9259-104">[E-Mail-Infos](../resources/mailtips.md) zu automatischen Antworten, die für ein Postfach festgelegt wurden.</span><span class="sxs-lookup"><span data-stu-id="a9259-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="a9259-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a9259-105">Properties</span></span>
| <span data-ttu-id="a9259-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a9259-106">Property</span></span>     | <span data-ttu-id="a9259-107">Typ</span><span class="sxs-lookup"><span data-stu-id="a9259-107">Type</span></span>   |<span data-ttu-id="a9259-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9259-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="a9259-109">message</span><span class="sxs-lookup"><span data-stu-id="a9259-109">message</span></span> | <span data-ttu-id="a9259-110">String</span><span class="sxs-lookup"><span data-stu-id="a9259-110">String</span></span> | <span data-ttu-id="a9259-111">Die automatische Antwortnachricht.</span><span class="sxs-lookup"><span data-stu-id="a9259-111">The automatic reply message.</span></span> |
| <span data-ttu-id="a9259-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="a9259-112">messageLanguage</span></span> | [<span data-ttu-id="a9259-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="a9259-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="a9259-114">Die Sprache, der in die automatische Antwort ist.</span><span class="sxs-lookup"><span data-stu-id="a9259-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="a9259-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="a9259-115">scheduledEndTime</span></span> | [<span data-ttu-id="a9259-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a9259-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="a9259-117">Das Datum und die Uhrzeit, die automatische Antworten für das Ende festgelegt sind.</span><span class="sxs-lookup"><span data-stu-id="a9259-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="a9259-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="a9259-118">scheduledStartTime</span></span> | [<span data-ttu-id="a9259-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a9259-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="a9259-120">Das Datum und die Uhrzeit, die automatische Antworten beginnen festgelegt sind.</span><span class="sxs-lookup"><span data-stu-id="a9259-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a9259-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a9259-121">JSON representation</span></span>

<span data-ttu-id="a9259-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a9259-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/automaticrepliesmailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
