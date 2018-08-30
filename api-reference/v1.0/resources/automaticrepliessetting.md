# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="8fa58-101">Ressourcentyp automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="8fa58-101">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="8fa58-p101">Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer. Beispiel: eine automatische Antwort, die darüber informiert, dass der angemeldete Benutzer zur Beantwortung von E-Mails nicht verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="8fa58-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="8fa58-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8fa58-104">Properties</span></span>
| <span data-ttu-id="8fa58-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8fa58-105">Property</span></span>     | <span data-ttu-id="8fa58-106">Typ</span><span class="sxs-lookup"><span data-stu-id="8fa58-106">Type</span></span>   |<span data-ttu-id="8fa58-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fa58-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fa58-108">externalAudience</span><span class="sxs-lookup"><span data-stu-id="8fa58-108">externalAudience</span></span>|<span data-ttu-id="8fa58-109">ExternalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="8fa58-109">ExternalAudienceScope</span></span>| <span data-ttu-id="8fa58-110">Die Benutzergruppe außerhalb der Organisation des angemeldeten Benutzers, der die **ExternalReplyMessage** erhält, wenn der **Status** `AlwaysEnabled` oder `Scheduled` ist.</span><span class="sxs-lookup"><span data-stu-id="8fa58-110">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or . Possible values are: , , `Scheduled`.</span></span> <span data-ttu-id="8fa58-111">Mögliche Werte sind: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="8fa58-111">The possible values are `none`, `contactsOnly`, `all`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="8fa58-112">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="8fa58-112">externalReplyMessage</span></span>|<span data-ttu-id="8fa58-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fa58-113">string</span></span>|<span data-ttu-id="8fa58-114">Die automatische Antwort an die angegebene externe Zielgruppe, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.</span><span class="sxs-lookup"><span data-stu-id="8fa58-114">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="8fa58-115">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="8fa58-115">internalReplyMessage</span></span>|<span data-ttu-id="8fa58-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8fa58-116">string</span></span>|<span data-ttu-id="8fa58-117">Die automatische Antwort an die interne Zielgruppe in der Organisation des angemeldeten Benutzers, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.</span><span class="sxs-lookup"><span data-stu-id="8fa58-117">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="8fa58-118">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="8fa58-118">scheduledEndDateTime</span></span>|[<span data-ttu-id="8fa58-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8fa58-119">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="8fa58-120">Datum und Uhrzeit, die zum Beenden der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="8fa58-120">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="8fa58-121">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="8fa58-121">scheduledStartDateTime</span></span>|[<span data-ttu-id="8fa58-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8fa58-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="8fa58-123">Datum und Uhrzeit, die für den Beginn der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="8fa58-123">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="8fa58-124">Status</span><span class="sxs-lookup"><span data-stu-id="8fa58-124">status</span></span>|<span data-ttu-id="8fa58-125">AutomaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="8fa58-125">AutomaticRepliesStatus</span></span>|<span data-ttu-id="8fa58-126">Status der Konfigurationen für automatische Antworten.</span><span class="sxs-lookup"><span data-stu-id="8fa58-126">Configurations status for automatic replies. Possible values are: , , .</span></span> <span data-ttu-id="8fa58-127">Mögliche Werte sind: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="8fa58-127">The possible values are `disabled`, `alwaysEnabled`, `scheduled`, , , , , , , , , or .</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fa58-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8fa58-128">JSON representation</span></span>

<span data-ttu-id="8fa58-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8fa58-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
