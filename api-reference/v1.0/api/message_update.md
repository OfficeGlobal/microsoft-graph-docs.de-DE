# <a name="update-message"></a><span data-ttu-id="b3f14-101">Nachricht aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b3f14-101">Update message</span></span>

<span data-ttu-id="b3f14-102">Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="b3f14-102">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3f14-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b3f14-103">Permissions</span></span>
<span data-ttu-id="b3f14-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b3f14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b3f14-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3f14-106">Permission type</span></span>      | <span data-ttu-id="b3f14-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3f14-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3f14-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3f14-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b3f14-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3f14-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b3f14-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3f14-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3f14-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3f14-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b3f14-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3f14-112">Application</span></span> | <span data-ttu-id="b3f14-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3f14-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3f14-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3f14-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b3f14-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3f14-115">Request headers</span></span>
| <span data-ttu-id="b3f14-116">Name</span><span class="sxs-lookup"><span data-stu-id="b3f14-116">Name</span></span>       | <span data-ttu-id="b3f14-117">Typ</span><span class="sxs-lookup"><span data-stu-id="b3f14-117">Type</span></span> | <span data-ttu-id="b3f14-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3f14-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b3f14-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3f14-119">Authorization</span></span>  | <span data-ttu-id="b3f14-120">string</span><span class="sxs-lookup"><span data-stu-id="b3f14-120">string</span></span>  | <span data-ttu-id="b3f14-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3f14-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3f14-123">Content-Type</span></span> | <span data-ttu-id="b3f14-124">string</span><span class="sxs-lookup"><span data-stu-id="b3f14-124">string</span></span>  | <span data-ttu-id="b3f14-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="b3f14-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3f14-127">Request body</span></span>
<span data-ttu-id="b3f14-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="b3f14-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="b3f14-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b3f14-132">Property</span></span>     | <span data-ttu-id="b3f14-133">Typ</span><span class="sxs-lookup"><span data-stu-id="b3f14-133">Type</span></span>   |<span data-ttu-id="b3f14-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3f14-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3f14-135">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="b3f14-135">bccRecipients</span></span>|<span data-ttu-id="b3f14-136">Recipient</span><span class="sxs-lookup"><span data-stu-id="b3f14-136">Recipient</span></span>|<span data-ttu-id="b3f14-p105">Die Bcc:-Empfänger der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p105">The Bcc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="b3f14-139">categories</span><span class="sxs-lookup"><span data-stu-id="b3f14-139">categories</span></span>|<span data-ttu-id="b3f14-140">String collection</span><span class="sxs-lookup"><span data-stu-id="b3f14-140">String collection</span></span>|<span data-ttu-id="b3f14-141">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="b3f14-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="b3f14-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="b3f14-142">ccRecipients</span></span>|<span data-ttu-id="b3f14-143">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="b3f14-143">Recipient collection</span></span>|<span data-ttu-id="b3f14-p106">Die Cc:-Empfänger der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p106">The Cc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="b3f14-146">Von</span><span class="sxs-lookup"><span data-stu-id="b3f14-146">from</span></span>|<span data-ttu-id="b3f14-147">Recipient</span><span class="sxs-lookup"><span data-stu-id="b3f14-147">Recipient</span></span>|<span data-ttu-id="b3f14-p107">Der Postfachbesitzer und der Absender der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p107">The mailbox owner and sender of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="b3f14-150">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="b3f14-150">importance</span></span>|<span data-ttu-id="b3f14-151">String</span><span class="sxs-lookup"><span data-stu-id="b3f14-151">String</span></span>|<span data-ttu-id="b3f14-p108">Wichtigkeit der Nachricht Mögliche Werte: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p108">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="b3f14-154">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="b3f14-154">inferenceClassification</span></span> | <span data-ttu-id="b3f14-155">String</span><span class="sxs-lookup"><span data-stu-id="b3f14-155">String</span></span> | <span data-ttu-id="b3f14-p109">Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung. Mögliche Werte sind: `focused` oder `other`.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p109">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="b3f14-158">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="b3f14-158">internetMessageId</span></span> |<span data-ttu-id="b3f14-159">String</span><span class="sxs-lookup"><span data-stu-id="b3f14-159">String</span></span> |<span data-ttu-id="b3f14-p110">Die Nachrichten-ID im von [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) angegebenen Format. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p110">The message ID in the format specified by [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="b3f14-162">isRead</span><span class="sxs-lookup"><span data-stu-id="b3f14-162">isRead</span></span>|<span data-ttu-id="b3f14-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3f14-163">Boolean</span></span>|<span data-ttu-id="b3f14-164">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="b3f14-164">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="b3f14-165">replyTo</span><span class="sxs-lookup"><span data-stu-id="b3f14-165">replyTo</span></span>|<span data-ttu-id="b3f14-166">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="b3f14-166">Recipient collection</span></span>|<span data-ttu-id="b3f14-p111">Die E-Mail-Adressen, die beim Antworten verwendet werden sollen. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p111">The email addresses to use when replying. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="b3f14-169">sender</span><span class="sxs-lookup"><span data-stu-id="b3f14-169">sender</span></span>|<span data-ttu-id="b3f14-170">Recipient</span><span class="sxs-lookup"><span data-stu-id="b3f14-170">Recipient</span></span>|<span data-ttu-id="b3f14-p112">Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p112">The account that is actually used to generate the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="b3f14-173">toRecipients</span><span class="sxs-lookup"><span data-stu-id="b3f14-173">toRecipients</span></span>|<span data-ttu-id="b3f14-174">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="b3f14-174">Recipient collection</span></span>|<span data-ttu-id="b3f14-p113">Die An:-Empfänger der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p113">The To recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="b3f14-177">body</span><span class="sxs-lookup"><span data-stu-id="b3f14-177">body</span></span>|<span data-ttu-id="b3f14-178">ItemBody</span><span class="sxs-lookup"><span data-stu-id="b3f14-178">ItemBody</span></span>|<span data-ttu-id="b3f14-p114">Der Text der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p114">The body of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="b3f14-181">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b3f14-181">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="b3f14-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3f14-182">Boolean</span></span>|<span data-ttu-id="b3f14-183">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="b3f14-183">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="b3f14-184">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b3f14-184">isReadReceiptRequested</span></span>|<span data-ttu-id="b3f14-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3f14-185">Boolean</span></span>|<span data-ttu-id="b3f14-186">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="b3f14-186">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="b3f14-187">subject</span><span class="sxs-lookup"><span data-stu-id="b3f14-187">subject</span></span>|<span data-ttu-id="b3f14-188">String</span><span class="sxs-lookup"><span data-stu-id="b3f14-188">String</span></span>|<span data-ttu-id="b3f14-p115">Der Betreff der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p115">The subject of the message. Updatable only if IsDraft = true.</span></span>|

<span data-ttu-id="b3f14-191">Da die **message**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="b3f14-191">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="b3f14-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3f14-192">Response</span></span>

<span data-ttu-id="b3f14-193">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3f14-193">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3f14-194">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3f14-194">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3f14-195">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3f14-195">Request</span></span>
<span data-ttu-id="b3f14-196">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3f14-196">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a><span data-ttu-id="b3f14-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3f14-197">Response</span></span>
<span data-ttu-id="b3f14-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3f14-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a><span data-ttu-id="b3f14-201">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="b3f14-201">See also</span></span>

- [<span data-ttu-id="b3f14-202">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="b3f14-202">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="b3f14-203">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="b3f14-203">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
