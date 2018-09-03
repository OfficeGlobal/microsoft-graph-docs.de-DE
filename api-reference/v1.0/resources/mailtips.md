# <a name="mailtips-resource-type"></a><span data-ttu-id="0969b-101">Ressourcentyp mailTips</span><span class="sxs-lookup"><span data-stu-id="0969b-101">mailTips resource type</span></span>

<span data-ttu-id="0969b-102">Informative Nachrichten über einen Empfänger, die Benutzern beim Verfassen einer Nachricht angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0969b-102">Informative messages displayed to users while they are composing a message.</span></span> <span data-ttu-id="0969b-103">Zum Beispiel eine Abwesenheitsnachricht als automatische Antwort für einen Nachrichtenempfänger.</span><span class="sxs-lookup"><span data-stu-id="0969b-103">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="0969b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0969b-104">Properties</span></span>
| <span data-ttu-id="0969b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0969b-105">Property</span></span>     | <span data-ttu-id="0969b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="0969b-106">Type</span></span>   |<span data-ttu-id="0969b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0969b-107">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0969b-108">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="0969b-108">AutomaticReplies</span></span> | [<span data-ttu-id="0969b-109">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="0969b-109">AutomaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="0969b-110">E-Mail-Info für die automatische Antwort, wenn sie vom Empfänger eingerichtet wurde.</span><span class="sxs-lookup"><span data-stu-id="0969b-110">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="0969b-111">customMailTip</span><span class="sxs-lookup"><span data-stu-id="0969b-111">CustomMailTip</span></span> | <span data-ttu-id="0969b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0969b-112">String</span></span> | <span data-ttu-id="0969b-113">Eine benutzerdefinierte E-Mail-Info, die auf dem Postfach des Empfängers eingestellt werden kann.</span><span class="sxs-lookup"><span data-stu-id="0969b-113">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="0969b-114">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="0969b-114">DeliveryRestricted</span></span>| <span data-ttu-id="0969b-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0969b-115">Boolean</span></span> | <span data-ttu-id="0969b-116">Ob das Postfach des Empfängers eingeschränkt ist, z. B. nur Nachrichten von einer vordefinierten Liste von Absendern annehmen, Nachrichten von einer vordefinierten Liste von Absendern ablehnen oder nur Nachrichten von authentifizierten Absendern annehmen.</span><span class="sxs-lookup"><span data-stu-id="0969b-116">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="0969b-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0969b-117">emailAddress</span></span> | [<span data-ttu-id="0969b-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0969b-118">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="0969b-119">Die E-Mail-Adresse des Empfängers, für den Sie E-Mail-Info erhalten möchten.</span><span class="sxs-lookup"><span data-stu-id="0969b-119">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="0969b-120">error</span><span class="sxs-lookup"><span data-stu-id="0969b-120">error</span></span> | [<span data-ttu-id="0969b-121">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="0969b-121">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="0969b-122">Fehler, die während der Aktion [getMailTips](../api/user_getmailtips.md) auftreten.</span><span class="sxs-lookup"><span data-stu-id="0969b-122">Errors that occur during the [GetMailTips](../api/user_getmailtips.md) action.</span></span> |
| <span data-ttu-id="0969b-123">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="0969b-123">ExternalMemberCount</span></span> | <span data-ttu-id="0969b-124">Int32</span><span class="sxs-lookup"><span data-stu-id="0969b-124">Int32</span></span> | <span data-ttu-id="0969b-125">Die Anzahl der externen Mitglieder, wenn der Empfänger eine Verteilerliste ist.</span><span class="sxs-lookup"><span data-stu-id="0969b-125">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="0969b-126">isModerated</span><span class="sxs-lookup"><span data-stu-id="0969b-126">IsModerated</span></span> |<span data-ttu-id="0969b-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0969b-127">Boolean</span></span>  | <span data-ttu-id="0969b-128">Ob das Versenden von Nachrichten an den Empfänger eine Genehmigung benötigt.</span><span class="sxs-lookup"><span data-stu-id="0969b-128">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="0969b-129">Zum Beispiel, wenn der Empfänger eine große Verteilerliste ist und ein Moderator eingerichtet wurde, um an diese Verteilerliste gesendete Nachrichten zu genehmigen, oder wenn das Senden von Nachrichten an einen Empfänger die Genehmigung des Managers des Empfängers benötigt.</span><span class="sxs-lookup"><span data-stu-id="0969b-129">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="0969b-130">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="0969b-130">MailboxFull</span></span> | <span data-ttu-id="0969b-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0969b-131">Boolean</span></span> | <span data-ttu-id="0969b-132">Der Status Postfach voll des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="0969b-132">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="0969b-133">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="0969b-133">MaxMessageSize</span></span> | <span data-ttu-id="0969b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="0969b-134">Int32</span></span> | <span data-ttu-id="0969b-135">Die maximale Nachrichtengröße, die für die Organisation oder das Postfach des Empfängers konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="0969b-135">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="0969b-136">recipientScope</span><span class="sxs-lookup"><span data-stu-id="0969b-136">RecipientScope</span></span> | <span data-ttu-id="0969b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0969b-137">String</span></span> | <span data-ttu-id="0969b-138">Der Bereich des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="0969b-138">The scope of the recipient, such as internal, external, partner.</span></span> <span data-ttu-id="0969b-139">Mögliche Werte sind: `none`, `internal`, `external`, `externalPartner` und `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="0969b-139">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="0969b-140">Beispielsweise kann ein Administrator eine andere Organisation als "Partner" festlegen.</span><span class="sxs-lookup"><span data-stu-id="0969b-140">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="0969b-141">Der Bereich ist nützlich, wenn ein Administrator möchte, dass bestimmte E-Mail-Info für bestimmte Bereiche zugänglich sind.</span><span class="sxs-lookup"><span data-stu-id="0969b-141">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="0969b-142">Es ist auch nützlich, die Absender darüber zu informieren, dass ihre Nachricht die Organisation verlassen kann, um ihnen bei den richtigen Entscheidungen über Wortlaut, Ton und Inhalt zu helfen.</span><span class="sxs-lookup"><span data-stu-id="0969b-142">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="0969b-143">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="0969b-143">RecipientSuggestions</span></span> | <span data-ttu-id="0969b-144">[Empfänger](../resources/recipient.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0969b-144">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="0969b-145">Empfänger, die auf der Grundlage früherer Kontexte vorgeschlagen werden, in denen sie in der gleichen Nachricht erscheinen.</span><span class="sxs-lookup"><span data-stu-id="0969b-145">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="0969b-146">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="0969b-146">TotalMemberCount</span></span> | <span data-ttu-id="0969b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0969b-147">Int32</span></span> | <span data-ttu-id="0969b-148">Die Anzahl der Mitglieder, wenn der Empfänger eine Verteilerliste ist.</span><span class="sxs-lookup"><span data-stu-id="0969b-148">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0969b-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0969b-149">JSON representation</span></span>

<span data-ttu-id="0969b-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0969b-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->