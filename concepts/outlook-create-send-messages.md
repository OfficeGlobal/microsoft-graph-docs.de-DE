# <a name="create-and-send-outlook-messages"></a><span data-ttu-id="15a09-101">Erstellen und Senden von Outlook-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="15a09-101">Create and send Outlook messages</span></span>

<span data-ttu-id="15a09-102">E-Mails werden in Microsoft Graph durch die [message](../api-reference/v1.0/resources/message.md)-Ressource dargestellt.</span><span class="sxs-lookup"><span data-stu-id="15a09-102">Emails are represented by the [message](../api-reference/v1.0/resources/message.md) resource in Microsoft Graph.</span></span>

<span data-ttu-id="15a09-103">Standardmäßig werden Nachrichten durch eine eindeutige Eintrags-ID in der **id**-Eigenschaft identifiziert.</span><span class="sxs-lookup"><span data-stu-id="15a09-103">By default, messages are identified by a unique entry ID in the **id** property.</span></span> <span data-ttu-id="15a09-104">Ein Speicheranbieter weist einer Nachricht eine Eintrags-ID zu, wenn die Nachricht zuerst als Entwurf gespeichert oder gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="15a09-104">A store provider assigns a message an entry ID when the message is initially saved as a draft or sent.</span></span> <span data-ttu-id="15a09-105">Diese ID ändert sich, wenn die Nachricht kopiert oder in einen anderen Ordner, einen Store oder eine PST-Datei verschoben wird.</span><span class="sxs-lookup"><span data-stu-id="15a09-105">That ID changes when the message is copied or moved to another folder, store, or .PST file.</span></span>

## <a name="creating-and-sending-mail"></a><span data-ttu-id="15a09-106">Erstellen und Senden von Mail</span><span class="sxs-lookup"><span data-stu-id="15a09-106">Creating and sending mail</span></span>

<span data-ttu-id="15a09-107">In Outlook können Sie eine E-Mail in derselben [SendMail](../api-reference/v1.0/api/user_sendmail.md)-Aktion erstellen und senden, oder Sie können einen Entwurf [erstellen](../api-reference/v1.0/api/user_post_messages.md), anschließend [Inhalt hinzufügen](../api-reference/v1.0/api/message_update.md) und den Entwurf dann [senden](../api-reference/v1.0/api/message_send.md).</span><span class="sxs-lookup"><span data-stu-id="15a09-107">In Outlook, you can create and send an email in the same [sendMail](../api-reference/v1.0/api/user_sendmail.md) action, or you can [create](../api-reference/v1.0/api/user_post_messages.md) a draft, subsequently [add content](../api-reference/v1.0/api/message_update.md) and [send](../api-reference/v1.0/api/message_send.md) the draft.</span></span>

<span data-ttu-id="15a09-108">Wenn Sie auf eine E-Mail antworten, können Sie auf ähnliche Weise die Antwort in derselben Aktion erstellen und senden ([reply](../api-reference/v1.0/api/message_reply.md), [reply-all](../api-reference/v1.0/api//message_replyall.md) oder [forward](../api-reference/v1.0/api/message_forward.md)).</span><span class="sxs-lookup"><span data-stu-id="15a09-108">Similarly, when responding to an email, you can create and send the response in the same action ([reply](../api-reference/v1.0/api/message_reply.md), [reply-all](../api-reference/v1.0/api//message_replyall.md), or [forward](../api-reference/v1.0/api/message_forward.md)).</span></span> <span data-ttu-id="15a09-109">Sie können auch einen Entwurf für die Antwort erstellen ([reply](../api-reference/v1.0/api/message_createreply.md), [reply-all](../api-reference/v1.0/api//message_createreplyall.md) oder [forward](../api-reference/v1.0/api/message_createforward.md)), [Inhalt hinzufügen](../api-reference/v1.0/api/message_update.md) und den Entwurf zu einem späteren Zeitpunkt [senden](../api-reference/v1.0/api/message_send.md).</span><span class="sxs-lookup"><span data-stu-id="15a09-109">Or, you can create a draft for the response ([reply](../api-reference/v1.0/api/message_createreply.md), [reply-all](../api-reference/v1.0/api//message_createreplyall.md), or [forward](../api-reference/v1.0/api/message_createforward.md)), [add content](../api-reference/v1.0/api/message_update.md), and then [send](../api-reference/v1.0/api/message_send.md) the draft at a later time.</span></span>

<span data-ttu-id="15a09-110">Um programmgesteuert zwischen einem Entwurf und einer gesendeten Nachricht zu unterscheiden, überprüfen Sie die Eigenschaft **isDraft**.</span><span class="sxs-lookup"><span data-stu-id="15a09-110">To distinguish between a draft and a sent message programmatically, check the **isDraft** property.</span></span>

<span data-ttu-id="15a09-111">Standardmäßig werden Nachrichtenentwürfe im Ordner `Drafts`gespeichert, und gesendete Nachrichten werden im Ordner `Sent Items` gespeichert.</span><span class="sxs-lookup"><span data-stu-id="15a09-111">By default, draft messages are saved in the `Drafts` folder, sent messages are saved in the `Sent Items` folder.</span></span> <span data-ttu-id="15a09-112">Sie können den Ordner für Entwürfe und den Ordner für gesendete Elemente auch einfach anhand ihrer [bekannten Ordnernamen](../api-reference/v1.0/resources/mailfolder.md) erkennen.</span><span class="sxs-lookup"><span data-stu-id="15a09-112">For convenience, you can identify the Drafts folder and SentItems folder by their corresponding [well-known folder names](../api-reference/v1.0/resources/mailfolder.md).</span></span> <span data-ttu-id="15a09-113">Sie können z. B. Folgendes durchführen, um die [Nachrichten](../api-reference/v1.0/api/user_list_messages.md) im Ordner „Entwürfe“ abzurufen:</span><span class="sxs-lookup"><span data-stu-id="15a09-113">For example, you can do the following to [get the messages](../api-reference/v1.0/api/user_list_messages.md) in the Drafts folder:</span></span>

```http
GET /me/mailfolders('Drafts')
```

### <a name="body-format-and-malicious-script"></a><span data-ttu-id="15a09-114">Textformat und bösartige Skripts</span><span class="sxs-lookup"><span data-stu-id="15a09-114">Body format and malicious script</span></span>

<!-- Remove the following 2 sections from the message.md topics
-->

<span data-ttu-id="15a09-115">Der Nachrichtentext kann entweder das HTML- oder Textformat aufweisen, wobei HTML der standardmäßige Nachrichtentexttyp ist, der bei einer GET-Antwort zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="15a09-115">The message body can be either HTML or text, with HTML as the default message body type returned in a GET response.</span></span>

<span data-ttu-id="15a09-116">Wenn Sie [eine Nachricht abrufen](../api-reference/v1.0/api/message_get.md), können Sie den folgenden Anforderungsheader angeben, um die Eigenschaften **body** und **uniqueBody** im Textformat zurückzugeben:</span><span class="sxs-lookup"><span data-stu-id="15a09-116">When [getting a message](../api-reference/v1.0/api/message_get.md), you can specify the following request header to return the **body** and **uniqueBody** properties in text format:</span></span>

```http
Prefer: outlook.body-content-type="text"
```

<span data-ttu-id="15a09-117">Sie können den folgenden Header angeben oder ihn einfach überspringen, um den Nachrichtentext im HTML-Format zu erhalten:</span><span class="sxs-lookup"><span data-stu-id="15a09-117">You can specify the following header, or, just skip the header, to get the message body in HTML format:</span></span>

```http
Prefer: outlook.body-content-type="html"
```

<span data-ttu-id="15a09-118">Wenn Sie einen der Header angeben, enthält eine erfolgreiche Antwort den entsprechenden `Preference-Applied`-Header:</span><span class="sxs-lookup"><span data-stu-id="15a09-118">When you specify either header, a successful response would include the corresponding `Preference-Applied` header:</span></span>

- <span data-ttu-id="15a09-119">Für Textformatanforderungen: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="15a09-119">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="15a09-120">Für HTML-Formatanforderungen: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="15a09-120">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

<span data-ttu-id="15a09-121">Wenn der Textkörper im HTML-Format vorliegt, entfernt Outlook standardmäßig alle potenziell unsicheren HTML-Elemente (z. B. JavaScript), die in der **body**-Eigenschaft eingebettet sind, vor dem Zurückgeben des Textkörperinhalts in einer REST-Antwort.</span><span class="sxs-lookup"><span data-stu-id="15a09-121">If the body is HTML, by default, Outlook removes any potentially unsafe HTML (for example, JavaScript) embedded in the **body** property before returning the body content in a REST response.</span></span>

<span data-ttu-id="15a09-122">Um den gesamten ursprünglichen HTML-Inhalt abzurufen, schließen Sie den folgenden HTTP-Anforderungsheader ein:</span><span class="sxs-lookup"><span data-stu-id="15a09-122">To get the entire, original HTML content, include the following HTTP request header:</span></span>

```http
Prefer: outlook.allow-unsafe-html
```

### <a name="differentiating-the-from-and-sender-properties"></a><span data-ttu-id="15a09-123">Unterscheiden der „Von“- und „Absender“-Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="15a09-123">Differentiating the from and sender properties</span></span>

<span data-ttu-id="15a09-124">Wenn in Outlook eine Nachricht erstellt wird legt Outlook in den meisten Fällen denselben angemeldeten Benutzer für die Eigenschaften **from** und **sender** fest.</span><span class="sxs-lookup"><span data-stu-id="15a09-124">When a message is being composed, in most cases, Outlook sets the **from** and **sender** properties to the same signed-in user.</span></span> <span data-ttu-id="15a09-125">Sie können diese Eigenschaften in den folgenden Szenarien aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="15a09-125">You can update these properties in the following scenarios:</span></span>

- <span data-ttu-id="15a09-p105">Die **from**-Eigenschaft kann geändert werden, wenn der Exchange-Administrator **sendAs**-Rechte des Postfachs anderen Benutzern zugewiesen hat. Der Administrator kann dies tun, indem er **Postfachberechtigungen** des Postfachbesitzers im Azure-Portal auswählt oder das Exchange Admin Center oder ein Windows PowerShell Add-ADPermission-Cmdlet verwendet. Dann können Sie programmgesteuert die **from**-Eigenschaft eines dieser Benutzer festlegen, die **sendAs**-Rechte für das Postfach haben.</span><span class="sxs-lookup"><span data-stu-id="15a09-p105">The **from** property can be changed if the Exchange administrator has assigned **sendAs** rights of the mailbox to some other users. The administrator can do this by selecting **Mailbox Permissions** of the mailbox owner in the Azure portal, or by using the Exchange Admin Center or a Windows PowerShell Add-ADPermission cmdlet. Then, you can programmatically set the **from** property to one of these users who have **sendAs** rights for that mailbox.</span></span>
- <span data-ttu-id="15a09-129">Die **sender**-Eigenschaft kann geändert werden, wenn der Postfachbesitzer das Recht, Nachrichten von diesem Postfach aus zu senden, an einen oder mehrere Benutzer delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="15a09-129">The **sender** property can be changed if the mailbox owner has delegated one or more users to be able to send messages from that mailbox.</span></span> <span data-ttu-id="15a09-130">Der Postfachbesitzer kann in Outlook an einen Stellvertreter delegieren.</span><span class="sxs-lookup"><span data-stu-id="15a09-130">The mailbox owner can delegate in Outlook.</span></span> <span data-ttu-id="15a09-131">Wenn ein Stellvertreter eine Nachricht im Namen des Postfachbesitzers sendet, legt Outlook die **sender**-Eigenschaft auf das Konto des Stellvertreters fest, während die **from**-Eigenschaft weiterhin den Postfachbesitzer angibt.</span><span class="sxs-lookup"><span data-stu-id="15a09-131">When a delegate sends a message on behalf of the mailbox owner, Outlook sets the **sender** property to the delegate’s account, and the **from** property remains as the mailbox owner.</span></span> <span data-ttu-id="15a09-132">Programmgesteuert können Sie die **sender**-Eigenschaft auf einen Benutzer festlegen, der Stellvertretungsberechtigungen für dieses Postfach besitzt.</span><span class="sxs-lookup"><span data-stu-id="15a09-132">Programmatically, you can set the **sender** property to a user who has got delegate permissions for that mailbox.</span></span>

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a><span data-ttu-id="15a09-133">Verwenden von MailTips zum Überprüfen des Empfängerstatus und Sparen von Zeit (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="15a09-133">Using MailTips to check recipient status and save time (preview)</span></span>

<span data-ttu-id="15a09-134">Mit [MailTips](../api-reference/beta/resources/mailtips.md) können Sie intelligente Entscheidungen treffen, bevor Sie eine E-Mail senden.</span><span class="sxs-lookup"><span data-stu-id="15a09-134">Use [MailTips](../api-reference/beta/resources/mailtips.md) to make smart decisions before sending an email.</span></span>
<span data-ttu-id="15a09-135">MailTips stellt Ihnen Informationen bereit, wie z. B. darüber, ob das Postfach eines Empfängers auf bestimmte Absender beschränkt ist oder ob zum Senden von E-Mails an den Empfänger eine Genehmigung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="15a09-135">MailTips can tell you information such as the recipient's mailbox is restricted to specific senders, or approval is required for emailing the recipient.</span></span>

## <a name="integrating-with--social-gesture-preview"></a><span data-ttu-id="15a09-136">Integration mit der Geste „@“ aus sozialen Netzwerken (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="15a09-136">Integrating with '@' social gesture (preview)</span></span>

<span data-ttu-id="15a09-137">@-Erwähnungen sind Benachrichtigungen, um Benutzer darauf hinzuweisen, dass sie in Nachrichten erwähnt werden.</span><span class="sxs-lookup"><span data-stu-id="15a09-137">@-mentions are notifications to alert users if they are mentioned in messages.</span></span> <span data-ttu-id="15a09-138">Mit der [mention](../api-reference/beta/resources/mention.md)-Ressource können Apps die aus sozialen Netzwerken bekannte Geste, das Präfix „@“, in E-Mails festlegen und daraus abrufen.</span><span class="sxs-lookup"><span data-stu-id="15a09-138">The [mention](../api-reference/beta/resources/mention.md) resource enables apps to set and get the common online social gesture, the '@' prefix, in emails.</span></span>
<span data-ttu-id="15a09-139">Sie können:</span><span class="sxs-lookup"><span data-stu-id="15a09-139">You can:</span></span>

- <span data-ttu-id="15a09-140">@-Erwähnungen beim [Erstellen einer Nachricht](../api-reference/beta/api/user_post_messages.md#request-2) erstellen</span><span class="sxs-lookup"><span data-stu-id="15a09-140">Create @-mentions when [creating a message](../api-reference/beta/api/user_post_messages.md#request-2)</span></span>
- [<span data-ttu-id="15a09-141">Alle Nachrichten im Postfach eines Benutzers abrufen, die eine @-Erwähnung des Benutzers beinhalten</span><span class="sxs-lookup"><span data-stu-id="15a09-141">Get all the messages in a user's mailbox that contain an @-mention of the user</span></span>](../api-reference/beta/api/user_list_messages.md#request-2)
- [<span data-ttu-id="15a09-142">Alle @-Erwähnungen in einer Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="15a09-142">Get all the @-mention is a message</span></span>](../api-reference/beta/api/message_get.md#request-2)

## <a name="other-shared-capabilities"></a><span data-ttu-id="15a09-143">Sonstige gemeinsam genutzte Funktionen</span><span class="sxs-lookup"><span data-stu-id="15a09-143">Other shared capabilities</span></span>

<span data-ttu-id="15a09-144">Nutzen Sie die Vorteile der folgenden gemeinsamen Funktionen, die von allen Entitäten in Microsoft Graph verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="15a09-144">Take advantage of the following common capabilities that are shared among Microsoft Graph entities:</span></span>

- <span data-ttu-id="15a09-145">Abonnieren Sie [Änderungsbenachrichtigungen](../api-reference/v1.0/resources/webhooks.md) für Nachrichten, wenn eine oder mehrere Typen von Änderungen auftreten, z. B. das Erstellen oder Aktualisieren von Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="15a09-145">Subscribe to [change notifications](../api-reference/v1.0/resources/webhooks.md) on messages when one or more types of changes occur, such as message creation or update.</span></span>
- <span data-ttu-id="15a09-146">[Verfolgen Sie diese inkrementellen Änderungen an Nachrichten in einem Ordner](delta_query_messages.md).</span><span class="sxs-lookup"><span data-stu-id="15a09-146">[Track these incremental changes to messages in a folder](delta_query_messages.md).</span></span>
- <span data-ttu-id="15a09-147">Erstellen Sie [offene Erweiterungen](extensibility_overview.md#open-extensions) oder [Schemaerweiterungen](extensibility_overview.md#schema-extensions), um einer Nachrichteninstanz benutzerdefinierte Daten hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="15a09-147">Create [open extensions](extensibility_overview.md#open-extensions) or [schema extensions](extensibility_overview.md#schema-extensions) to add custom data to a message instance.</span></span>
- <span data-ttu-id="15a09-148">Erstellen Sie [erweiterte Eigenschaften](../api-reference/v1.0/resources/extended-properties-overview.md) in einer Nachrichteninstanz, um benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zu speichern, wenn diese Eigenschaften in den Metadaten der Microsoft Graph-API noch nicht offengelegt wurden.</span><span class="sxs-lookup"><span data-stu-id="15a09-148">Create [extended properties](../api-reference/v1.0/resources/extended-properties-overview.md) in a message instance to store custom data for Outlook MAPI properties, when these properties are not already exposed in the Microsoft Graph API metadata.</span></span>

## <a name="next-steps"></a><span data-ttu-id="15a09-149">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="15a09-149">Next steps</span></span>

<span data-ttu-id="15a09-150">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="15a09-150">Find out more about:</span></span>

- [<span data-ttu-id="15a09-151">Gründe für die Integration in Outlook-Mail</span><span class="sxs-lookup"><span data-stu-id="15a09-151">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="15a09-152">[Verwenden der Mail-API](../api-reference/v1.0/resources/mail_api_overview.md) und [Anwendungsfälle](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) für diese in Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="15a09-152">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /concepts/outlook-create-send-messages.md:
        BookmarkSkippedDocFileNotFound: Link '[creating a message](../api-reference/beta/api/user_post_messages.md#request-2)'.",
    "Error: /concepts/outlook-create-send-messages.md:
      BookmarkSkippedDocFileNotFound: Link '[Get all the messages in a user's mailbox that contain an @-mention of the user](../api-reference/beta/api/user_list_messages.md#request-2)'.",
    "Error: /concepts/outlook-create-send-messages.md:
      BookmarkSkippedDocFileNotFound: Link '[Get all the @-mention is a message](../api-reference/beta/api/message_get.md#request-2)'."
  ]
}-->
