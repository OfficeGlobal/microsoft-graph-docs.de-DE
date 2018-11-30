---
title: Konfigurieren der Einladungsnachricht
description: Mit dem invitedUserMessageInfo-Objekt können Sie die invitation-Nachricht konfigurieren.
ms.openlocfilehash: c8258d2b90d1aa5f5081b271ccc70fcb7408b132
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019222"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="dcfcd-103">Konfigurieren der Einladungsnachricht</span><span class="sxs-lookup"><span data-stu-id="dcfcd-103">Configuring the invitation message</span></span>

<span data-ttu-id="dcfcd-104">Mit dem invitedUserMessageInfo-Objekt können Sie die [invitation](invitation.md)-Nachricht konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="dcfcd-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dcfcd-105">Properties</span></span>
| <span data-ttu-id="dcfcd-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dcfcd-106">Property</span></span>     | <span data-ttu-id="dcfcd-107">Typ</span><span class="sxs-lookup"><span data-stu-id="dcfcd-107">Type</span></span>   |<span data-ttu-id="dcfcd-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dcfcd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcfcd-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="dcfcd-109">ccRecipients</span></span>|<span data-ttu-id="dcfcd-110">[Recipient collection](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="dcfcd-110">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="dcfcd-p101">Weitere Empfänger, an die die Einladungsnachricht gesendet werden soll. Derzeit wird nur 1 zusätzlicher Empfänger unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="dcfcd-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="dcfcd-113">customizedMessageBody</span></span>|<span data-ttu-id="dcfcd-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dcfcd-114">String</span></span>|<span data-ttu-id="dcfcd-115">Angepasster Nachrichtentext, den Sie senden möchten, wenn Sie nicht die Standardnachricht senden.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="dcfcd-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="dcfcd-116">messageLanguage</span></span>|<span data-ttu-id="dcfcd-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dcfcd-117">String</span></span>|<span data-ttu-id="dcfcd-p102">Die Sprache, in der Sie die Standardnachricht senden möchten. Wenn customizedMessageBody angegeben ist, wird diese Eigenschaft ignoriert und die Nachricht wird mithilfe von customizedMessageBody gesendet. Das Sprachformat sollte ISO 639 sein. Der Standardwert ist en-US.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dcfcd-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dcfcd-122">JSON representation</span></span>
<span data-ttu-id="dcfcd-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-123">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
