# <a name="configuring-the-invitation-message"></a><span data-ttu-id="461c2-101">Konfigurieren der Einladungsnachricht</span><span class="sxs-lookup"><span data-stu-id="461c2-101">Configuring the invitation message</span></span>

<span data-ttu-id="461c2-102">Mit dem invitedUserMessageInfo-Objekt können Sie die [invitation](invitation.md)-Nachricht konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="461c2-102">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="461c2-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="461c2-103">Properties</span></span>
| <span data-ttu-id="461c2-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="461c2-104">Property</span></span>     | <span data-ttu-id="461c2-105">Typ</span><span class="sxs-lookup"><span data-stu-id="461c2-105">Type</span></span>   |<span data-ttu-id="461c2-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="461c2-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="461c2-107">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="461c2-107">ccRecipients</span></span>|[<span data-ttu-id="461c2-108">Empfänger</span><span class="sxs-lookup"><span data-stu-id="461c2-108">Recipient</span></span>](recipient.md)|<span data-ttu-id="461c2-p101">Weitere Empfänger, an die die Einladungsnachricht gesendet werden soll. Derzeit wird nur 1 zusätzlicher Empfänger unterstützt.</span><span class="sxs-lookup"><span data-stu-id="461c2-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="461c2-111">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="461c2-111">customizedMessageBody</span></span>|<span data-ttu-id="461c2-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="461c2-112">String</span></span>|<span data-ttu-id="461c2-113">Angepasster Nachrichtentext, den Sie senden möchten, wenn Sie nicht die Standardnachricht senden.</span><span class="sxs-lookup"><span data-stu-id="461c2-113">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="461c2-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="461c2-114">messageLanguage</span></span>|<span data-ttu-id="461c2-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="461c2-115">String</span></span>|<span data-ttu-id="461c2-p102">Die Sprache, in der Sie die Standardnachricht senden möchten. Wenn customizedMessageBody angegeben ist, wird diese Eigenschaft ignoriert und die Nachricht wird mithilfe von customizedMessageBody gesendet. Das Sprachformat sollte ISO 639 sein. Der Standardwert ist en-US.</span><span class="sxs-lookup"><span data-stu-id="461c2-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="461c2-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="461c2-120">JSON representation</span></span>
<span data-ttu-id="461c2-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="461c2-121">Here is a JSON representation of the resource</span></span>

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
