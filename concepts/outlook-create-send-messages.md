---
title: Automatisieren des Erstellens, Sendens und Verarbeitens von Nachrichten
description: E-Mails werden in Microsoft Graph durch die message-Ressource dargestellt.
ms.openlocfilehash: 9eba9e04426bdf1339d9ae287c1cf085bcf3b500
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283689"
---
# <a name="automate-creating-sending-and-processing-messages"></a><span data-ttu-id="7a813-103">Automatisieren des Erstellens, Sendens und Verarbeitens von Nachrichten</span><span class="sxs-lookup"><span data-stu-id="7a813-103">Automate creating, sending, and processing messages</span></span>

<span data-ttu-id="7a813-104">E-Mails werden in Microsoft Graph durch die [message](/graph/api/resources/message?view=graph-rest-1.0)-Ressource dargestellt.</span><span class="sxs-lookup"><span data-stu-id="7a813-104">Emails are represented by the [message](/graph/api/resources/message?view=graph-rest-1.0) resource in Microsoft Graph.</span></span>

<span data-ttu-id="7a813-105">Standardmäßig werden Nachrichten durch eine eindeutige Eintrags-ID in der **id**-Eigenschaft identifiziert.</span><span class="sxs-lookup"><span data-stu-id="7a813-105">By default, messages are identified by a unique entry ID in the **id** property.</span></span> <span data-ttu-id="7a813-106">Der Speicheranbieter weist der Nachricht eine Eintrags-ID zu, wenn die Nachricht zuerst als Entwurf gespeichert oder gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="7a813-106">When a message is initially created and saved as a draft or sent, the store provider assigns the message an entry ID.</span></span> <span data-ttu-id="7a813-107">Diese ID ändert sich standardmäßig, wenn die Nachricht kopiert oder in einen anderen Ordner, einen Store oder eine PST-Datei verschoben wird.</span><span class="sxs-lookup"><span data-stu-id="7a813-107">That ID changes when the message is copied or moved to another folder, store, or .PST file.</span></span> <span data-ttu-id="7a813-108">Auf die Nachricht wird anhand ihrer aktuellen ID für die weitere Verarbeitung verwiesen.</span><span class="sxs-lookup"><span data-stu-id="7a813-108">You reference the message by its current ID for further processing.</span></span>

## <a name="creating-and-sending-mail"></a><span data-ttu-id="7a813-109">Erstellen und Senden von Nachrichten</span><span class="sxs-lookup"><span data-stu-id="7a813-109">Creating and sending mail</span></span>

<span data-ttu-id="7a813-110">In Outlook können Sie eine E-Mail in derselben [SendMail](/graph/api/user-sendmail?view=graph-rest-1.0)-Aktion erstellen und senden, oder Sie können einen Entwurf [erstellen](/graph/api/user-post-messages?view=graph-rest-1.0), anschließend [Inhalt hinzufügen](/graph/api/message-update?view=graph-rest-1.0) und den Entwurf dann [senden](/graph/api/message-send?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="7a813-110">In Outlook, you can create and send an email in the same [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) action, or you can [create](/graph/api/user-post-messages?view=graph-rest-1.0) a draft, subsequently [add content](/graph/api/message-update?view=graph-rest-1.0) and [send](/graph/api/message-send?view=graph-rest-1.0) the draft.</span></span>

<span data-ttu-id="7a813-111">Wenn Sie auf eine E-Mail antworten, können Sie auf ähnliche Weise die Antwort in derselben Aktion erstellen und senden ([reply](/graph/api/message-reply?view=graph-rest-1.0), [reply-all](/graph/api/message-replyall?view=graph-rest-1.0) oder [forward](/graph/api/message-forward?view=graph-rest-1.0)).</span><span class="sxs-lookup"><span data-stu-id="7a813-111">Similarly, when responding to an email, you can create and send the response in the same action ([reply](/graph/api/message-reply?view=graph-rest-1.0), [reply-all](/graph/api/message-replyall?view=graph-rest-1.0), or [forward](/graph/api/message-forward?view=graph-rest-1.0)).</span></span> <span data-ttu-id="7a813-112">Sie können auch einen Entwurf für die Antwort erstellen ([reply](/graph/api/message-createreply?view=graph-rest-1.0), [reply-all](/graph/api/message-createreplyall?view=graph-rest-1.0) oder [forward](/graph/api/message-createforward?view=graph-rest-1.0)), [Inhalt hinzufügen](/graph/api/message-update?view=graph-rest-1.0) und den Entwurf zu einem späteren Zeitpunkt [senden](/graph/api/message-send?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="7a813-112">Or, you can create a draft for the response ([reply](/graph/api/message-createreply?view=graph-rest-1.0), [reply-all](/graph/api/message-createreplyall?view=graph-rest-1.0), or [forward](/graph/api/message-createforward?view=graph-rest-1.0)), [add content](/graph/api/message-update?view=graph-rest-1.0), and then [send](/graph/api/message-send?view=graph-rest-1.0) the draft at a later time.</span></span>

<span data-ttu-id="7a813-113">Um programmgesteuert zwischen einem Entwurf und einer gesendeten Nachricht zu unterscheiden, überprüfen Sie die Eigenschaft **isDraft**.</span><span class="sxs-lookup"><span data-stu-id="7a813-113">To distinguish between a draft and a sent message programmatically, check the **isDraft** property.</span></span>

<span data-ttu-id="7a813-114">Standardmäßig werden Nachrichtenentwürfe im Ordner `Drafts`gespeichert, und gesendete Nachrichten werden im Ordner `Sent Items` gespeichert.</span><span class="sxs-lookup"><span data-stu-id="7a813-114">By default, draft messages are saved in the `Drafts` folder, sent messages are saved in the `Sent Items` folder.</span></span> <span data-ttu-id="7a813-115">Sie können den Ordner für Entwürfe und den Ordner für gesendete Elemente auch einfach anhand ihrer [bekannten Ordnernamen](/graph/api/resources/mailfolder?view=graph-rest-1.0) erkennen.</span><span class="sxs-lookup"><span data-stu-id="7a813-115">For convenience, you can identify the Drafts folder and SentItems folder by their corresponding [well-known folder names](/graph/api/resources/mailfolder?view=graph-rest-1.0).</span></span> 

### <a name="setting-the-from-and-sender-properties"></a><span data-ttu-id="7a813-116">Festlegen der from- und sender-Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7a813-116">Setting the from and sender properties</span></span>

<span data-ttu-id="7a813-117">Wenn in Outlook eine Nachricht erstellt wird legt Outlook in den meisten Fällen denselben angemeldeten Benutzer für die Eigenschaften **from** und **sender** fest.</span><span class="sxs-lookup"><span data-stu-id="7a813-117">When a message is being composed, in most cases, Outlook sets the **from** and **sender** properties to the same signed-in user.</span></span> <span data-ttu-id="7a813-118">Sie können diese Eigenschaften in den folgenden Szenarien aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="7a813-118">You can update these properties in the following scenarios:</span></span>

- <span data-ttu-id="7a813-p105">Die **from**-Eigenschaft kann geändert werden, wenn der Exchange-Administrator **sendAs**-Rechte des Postfachs anderen Benutzern zugewiesen hat. Der Administrator kann dies tun, indem er **Postfachberechtigungen** des Postfachbesitzers im Azure-Portal auswählt oder das Exchange Admin Center oder ein Windows PowerShell Add-ADPermission-Cmdlet verwendet. Dann können Sie programmgesteuert die **from**-Eigenschaft eines dieser Benutzer festlegen, die **sendAs**-Rechte für das Postfach haben.</span><span class="sxs-lookup"><span data-stu-id="7a813-p105">The **from** property can be changed if the Exchange administrator has assigned **sendAs** rights of the mailbox to some other users. The administrator can do this by selecting **Mailbox Permissions** of the mailbox owner in the Azure portal, or by using the Exchange Admin Center or a Windows PowerShell Add-ADPermission cmdlet. Then, you can programmatically set the **from** property to one of these users who have **sendAs** rights for that mailbox.</span></span>
- <span data-ttu-id="7a813-122">Die **sender**-Eigenschaft kann geändert werden, wenn der Postfachbesitzer das Recht, Nachrichten von diesem Postfach aus zu senden, an einen oder mehrere Benutzer delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="7a813-122">The **sender** property can be changed if the mailbox owner has delegated one or more users to be able to send messages from that mailbox.</span></span> <span data-ttu-id="7a813-123">Der Postfachbesitzer kann in Outlook an einen Stellvertreter delegieren.</span><span class="sxs-lookup"><span data-stu-id="7a813-123">The mailbox owner can delegate in Outlook.</span></span> <span data-ttu-id="7a813-124">Wenn ein Stellvertreter eine Nachricht im Namen des Postfachbesitzers sendet, legt Outlook die **sender**-Eigenschaft auf das Konto des Stellvertreters fest, während die **from**-Eigenschaft weiterhin den Postfachbesitzer angibt.</span><span class="sxs-lookup"><span data-stu-id="7a813-124">When a delegate sends a message on behalf of the mailbox owner, Outlook sets the **sender** property to the delegate’s account, and the **from** property remains as the mailbox owner.</span></span> <span data-ttu-id="7a813-125">Programmgesteuert können Sie die **sender**-Eigenschaft auf einen Benutzer festlegen, der Stellvertretungsberechtigungen für dieses Postfach besitzt.</span><span class="sxs-lookup"><span data-stu-id="7a813-125">Programmatically, you can set the **sender** property to a user who has got delegate permissions for that mailbox.</span></span>

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a><span data-ttu-id="7a813-126">Verwenden von MailTips zum Überprüfen des Empfängerstatus und Sparen von Zeit (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="7a813-126">Using MailTips to check recipient status and save time (preview)</span></span>

<span data-ttu-id="7a813-127">Mit [MailTips](/graph/api/resources/mailtips?view=graph-rest-beta) können Sie intelligente Entscheidungen treffen, bevor Sie eine E-Mail senden.</span><span class="sxs-lookup"><span data-stu-id="7a813-127">Use [MailTips](/graph/api/resources/mailtips?view=graph-rest-beta) to make smart decisions before sending an email.</span></span>
<span data-ttu-id="7a813-128">MailTips stellt Ihnen Informationen bereit, wie z. B. darüber, ob das Postfach eines Empfängers auf bestimmte Absender beschränkt ist oder ob zum Senden von E-Mails an den Empfänger eine Genehmigung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="7a813-128">MailTips can tell you information such as the recipient's mailbox is restricted to specific senders, or approval is required for emailing the recipient.</span></span>


## <a name="reading-messages-with-control-over-the-body-format-returned"></a><span data-ttu-id="7a813-129">Lesen von Nachrichten mit Kontrolle über das zurückgegebene Textformat</span><span class="sxs-lookup"><span data-stu-id="7a813-129">Reading messages with control over the body format returned</span></span>

<span data-ttu-id="7a813-130">Sie können eine [Nachricht](/graph/api/message-get?view=graph-rest-1.0) in einem Postfach lesen, indem Sie auf ihre ID verweisen:</span><span class="sxs-lookup"><span data-stu-id="7a813-130">You can [read a message](/graph/api/message-get?view=graph-rest-1.0) in a mailbox by referencing its ID:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AAMkADhMGAAA="]
}-->
```http
GET /me/messages/AAMkADhMGAAA=
```

Oder Sie können [die Nachrichten in einem bestimmten Ordner abrufen](/graph/api/user-list-messages?view=graph-rest-1.0). <span data-ttu-id="7a813-132">Gehen Sie beispielsweise folgendermaßen vor, um Nachrichten im Ordner „Entwürfe“ des angemeldeten Benutzers zu lesen:</span><span class="sxs-lookup"><span data-stu-id="7a813-132">For example, to read messages in the signed-in user's Drafts folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailfolders('Drafts')
```

<span data-ttu-id="7a813-133">Der Nachrichtentext einer Outlook-Nachricht kann entweder das HTML- oder Textformat aufweisen, wobei HTML der standardmäßige Nachrichtentexttyp ist, der bei einer GET-Antwort zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="7a813-133">The message body can be either HTML or text, with HTML as the default message body type returned in a GET response.</span></span>

<span data-ttu-id="7a813-134">Wenn Sie eine Nachricht abrufen, können Sie den folgenden Anforderungsheader angeben, um die Eigenschaften **body** and **uniqueBody** im Textformat zurückzugeben:</span><span class="sxs-lookup"><span data-stu-id="7a813-134">When getting a message, you can specify the following request header to return the body and uniqueBody properties in text format:</span></span>

```http
Prefer: outlook.body-content-type="text"
```

<span data-ttu-id="7a813-135">Sie können den folgenden Header angeben oder ihn einfach überspringen, um den Nachrichtentext im HTML-Format zu erhalten:</span><span class="sxs-lookup"><span data-stu-id="7a813-135">You can specify the following header, or, just skip the header, to get the message body in HTML format:</span></span>

```http
Prefer: outlook.body-content-type="html"
```

<span data-ttu-id="7a813-136">Wenn Sie einen der Header angeben, enthält eine erfolgreiche Antwort den entsprechenden `Preference-Applied`-Header:</span><span class="sxs-lookup"><span data-stu-id="7a813-136">When you specify either header, a successful response would include the corresponding `Preference-Applied` header:</span></span>

- <span data-ttu-id="7a813-137">Für Textformatanforderungen: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="7a813-137">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="7a813-138">Für HTML-Formatanforderungen: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="7a813-138">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

<span data-ttu-id="7a813-139">Wenn der Textkörper im HTML-Format vorliegt, entfernt Outlook standardmäßig alle potenziell unsicheren HTML-Elemente (z. B. JavaScript), die in der **body**-Eigenschaft eingebettet sind, vor dem Zurückgeben des Textkörperinhalts in einer REST-Antwort.</span><span class="sxs-lookup"><span data-stu-id="7a813-139">If the body is HTML, by default, Outlook removes any potentially unsafe HTML (for example, JavaScript) embedded in the **body** property before returning the body content in a REST response.</span></span>

<span data-ttu-id="7a813-140">Um den gesamten ursprünglichen HTML-Inhalt abzurufen, schließen Sie den folgenden HTTP-Anforderungsheader ein:</span><span class="sxs-lookup"><span data-stu-id="7a813-140">To get the entire, original HTML content, include the following HTTP request header:</span></span>

```http
Prefer: outlook.allow-unsafe-html
```

## <a name="integrating-with--social-gesture-preview"></a><span data-ttu-id="7a813-141">Integration mit der Geste „@“ aus sozialen Netzwerken (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="7a813-141">Integrating with '@' social gesture (preview)</span></span>

<span data-ttu-id="7a813-142">@-Erwähnungen sind Benachrichtigungen, um Benutzer darauf hinzuweisen, dass sie in Nachrichten erwähnt werden.</span><span class="sxs-lookup"><span data-stu-id="7a813-142">@-mentions are notifications to alert users if they are mentioned in messages.</span></span> <span data-ttu-id="7a813-143">Mit der [mention](/graph/api/resources/mention?view=graph-rest-beta)-Ressource können Apps die aus sozialen Netzwerken bekannte Geste, das Präfix „@“, in E-Mails festlegen und daraus abrufen.</span><span class="sxs-lookup"><span data-stu-id="7a813-143">The [mention](/graph/api/resources/mention?view=graph-rest-beta) resource enables apps to set and get the common online social gesture, the '@' prefix, in emails.</span></span>
<span data-ttu-id="7a813-144">Sie können:</span><span class="sxs-lookup"><span data-stu-id="7a813-144">You can:</span></span>

- <span data-ttu-id="7a813-145">@-Erwähnungen beim [Erstellen einer Nachricht](/graph/api/user-post-messages?view=graph-rest-beta#request-2) erstellen</span><span class="sxs-lookup"><span data-stu-id="7a813-145">Create @-mentions when [creating a message](/graph/api/user-post-messages?view=graph-rest-beta#request-2)</span></span>
- [<span data-ttu-id="7a813-146">Alle Nachrichten im Postfach eines Benutzers abrufen, die eine @-Erwähnung des Benutzers beinhalten</span><span class="sxs-lookup"><span data-stu-id="7a813-146">Get all the messages in a user's mailbox that contain an @-mention of the user</span></span>](/graph/api/user-list-messages?view=graph-rest-beta#request-2)
- [<span data-ttu-id="7a813-147">Alle @-Erwähnungen in einer Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="7a813-147">Get all the @-mention is a message</span></span>](/graph/api/message-get?view=graph-rest-beta#request-2)

## <a name="other-shared-capabilities"></a><span data-ttu-id="7a813-148">Sonstige gemeinsam genutzte Funktionen</span><span class="sxs-lookup"><span data-stu-id="7a813-148">Other shared capabilities</span></span>

<span data-ttu-id="7a813-149">Nutzen Sie die Vorteile der folgenden gemeinsamen Funktionen, die von allen Entitäten in Microsoft Graph verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="7a813-149">Take advantage of the following common capabilities that are shared among Microsoft Graph entities:</span></span>

- <span data-ttu-id="7a813-150">Abonnieren Sie [Änderungsbenachrichtigungen](/graph/api/resources/webhooks?view=graph-rest-1.0) für Nachrichten, wenn eine oder mehrere Typen von Änderungen auftreten, z. B. das Erstellen oder Aktualisieren von Nachrichten.</span><span class="sxs-lookup"><span data-stu-id="7a813-150">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-1.0) on messages when one or more types of changes occur, such as message creation or update.</span></span>
- <span data-ttu-id="7a813-151">[Verfolgen Sie diese inkrementellen Änderungen an Nachrichten in einem Ordner](delta-query-messages.md).</span><span class="sxs-lookup"><span data-stu-id="7a813-151">[Track these incremental changes to messages in a folder](delta-query-messages.md).</span></span>
- <span data-ttu-id="7a813-152">Erstellen Sie [offene Erweiterungen](extensibility-overview.md#open-extensions) oder [Schemaerweiterungen](extensibility-overview.md#schema-extensions), um einer Nachrichteninstanz benutzerdefinierte Daten hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="7a813-152">Create [open extensions](extensibility-overview.md#open-extensions) or [schema extensions](extensibility-overview.md#schema-extensions) to add custom data to a message instance.</span></span>
- <span data-ttu-id="7a813-153">Erstellen Sie [erweiterte Eigenschaften](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) in einer Nachrichteninstanz, um benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zu speichern, wenn diese Eigenschaften in den Metadaten der Microsoft Graph-API noch nicht offengelegt wurden.</span><span class="sxs-lookup"><span data-stu-id="7a813-153">Create [extended properties](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) in a message instance to store custom data for Outlook MAPI properties, when these properties are not already exposed in the Microsoft Graph API metadata.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7a813-154">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="7a813-154">Next steps</span></span>

<span data-ttu-id="7a813-155">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="7a813-155">Find out more about:</span></span>

- [<span data-ttu-id="7a813-156">Gründe für die Integration in Outlook-Mail</span><span class="sxs-lookup"><span data-stu-id="7a813-156">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- [<span data-ttu-id="7a813-157">Abrufen von unveränderlichen Bezeichnern für Outlook-Ressourcen (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="7a813-157">Get immutable identifiers for Outlook resources</span></span>](outlook-immutable-id.md)
- <span data-ttu-id="7a813-158">[Verwenden der Mail-API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) und [Anwendungsfälle](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) für diese in Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="7a813-158">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>
