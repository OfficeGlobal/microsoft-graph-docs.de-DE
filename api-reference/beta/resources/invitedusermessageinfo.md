---
title: Konfigurieren der Einladungsnachricht
description: Mit dem invitedUserMessageInfo-Objekt können Sie die invitation-Nachricht konfigurieren.
localization_priority: Normal
ms.openlocfilehash: fa7ead6938ddfaca78322f56f4638c45d3f2df14
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643790"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="d61e6-103">Konfigurieren der Einladungsnachricht</span><span class="sxs-lookup"><span data-stu-id="d61e6-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d61e6-104">Mit dem invitedUserMessageInfo-Objekt können Sie die [invitation](invitation.md)-Nachricht konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="d61e6-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="d61e6-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d61e6-105">Properties</span></span>
| <span data-ttu-id="d61e6-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d61e6-106">Property</span></span>     | <span data-ttu-id="d61e6-107">Typ</span><span class="sxs-lookup"><span data-stu-id="d61e6-107">Type</span></span>   |<span data-ttu-id="d61e6-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d61e6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d61e6-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="d61e6-109">ccRecipients</span></span>|[<span data-ttu-id="d61e6-110">Recipients</span><span class="sxs-lookup"><span data-stu-id="d61e6-110">Recipients</span></span>](recipient.md)|<span data-ttu-id="d61e6-p101">Weitere Empfänger, an die die Einladungsnachricht gesendet werden soll. Derzeit wird nur 1 zusätzlicher Empfänger unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d61e6-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="d61e6-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="d61e6-113">customizedMessageBody</span></span>|<span data-ttu-id="d61e6-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d61e6-114">String</span></span>|<span data-ttu-id="d61e6-115">Angepasster Nachrichtentext, den Sie senden möchten, wenn Sie nicht die Standardnachricht senden.</span><span class="sxs-lookup"><span data-stu-id="d61e6-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="d61e6-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="d61e6-116">messageLanguage</span></span>|<span data-ttu-id="d61e6-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d61e6-117">String</span></span>|<span data-ttu-id="d61e6-p102">Die Sprache, in der Sie die Standardnachricht senden möchten. Wenn customizedMessageBody angegeben ist, wird diese Eigenschaft ignoriert und die Nachricht wird mithilfe von customizedMessageBody gesendet. Das Sprachformat sollte ISO 639 sein. Der Standardwert ist en-US.</span><span class="sxs-lookup"><span data-stu-id="d61e6-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d61e6-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d61e6-122">JSON representation</span></span>
<span data-ttu-id="d61e6-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d61e6-123">Here is a JSON representation of the resource</span></span>

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitedusermessageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
