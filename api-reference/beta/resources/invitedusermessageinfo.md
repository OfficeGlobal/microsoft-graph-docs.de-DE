---
title: Konfigurieren der Einladungsnachricht
description: Mit dem invitedUserMessageInfo-Objekt können Sie die invitation-Nachricht konfigurieren.
localization_priority: Normal
ms.openlocfilehash: f8a6dd118f1774320e3fe8327d284dac1141fc55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874123"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="ad212-103">Konfigurieren der Einladungsnachricht</span><span class="sxs-lookup"><span data-stu-id="ad212-103">Configuring the invitation message</span></span>

> <span data-ttu-id="ad212-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ad212-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad212-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad212-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad212-106">Mit dem invitedUserMessageInfo-Objekt können Sie die [invitation](invitation.md)-Nachricht konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="ad212-106">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="ad212-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ad212-107">Properties</span></span>
| <span data-ttu-id="ad212-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad212-108">Property</span></span>     | <span data-ttu-id="ad212-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ad212-109">Type</span></span>   |<span data-ttu-id="ad212-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad212-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad212-111">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="ad212-111">ccRecipients</span></span>|[<span data-ttu-id="ad212-112">Empfänger</span><span class="sxs-lookup"><span data-stu-id="ad212-112">Recipients</span></span>](recipient.md)|<span data-ttu-id="ad212-p102">Weitere Empfänger, an die die Einladungsnachricht gesendet werden soll. Derzeit wird nur 1 zusätzlicher Empfänger unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad212-p102">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="ad212-115">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="ad212-115">customizedMessageBody</span></span>|<span data-ttu-id="ad212-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ad212-116">String</span></span>|<span data-ttu-id="ad212-117">Angepasster Nachrichtentext, den Sie senden möchten, wenn Sie nicht die Standardnachricht senden.</span><span class="sxs-lookup"><span data-stu-id="ad212-117">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="ad212-118">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="ad212-118">messageLanguage</span></span>|<span data-ttu-id="ad212-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ad212-119">String</span></span>|<span data-ttu-id="ad212-p103">Die Sprache, in der Sie die Standardnachricht senden möchten. Wenn customizedMessageBody angegeben ist, wird diese Eigenschaft ignoriert und die Nachricht wird mithilfe von customizedMessageBody gesendet. Das Sprachformat sollte ISO 639 sein. Der Standardwert ist en-US.</span><span class="sxs-lookup"><span data-stu-id="ad212-p103">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad212-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ad212-124">JSON representation</span></span>
<span data-ttu-id="ad212-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ad212-125">Here is a JSON representation of the resource</span></span>

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
