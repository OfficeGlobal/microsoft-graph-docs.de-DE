# <a name="update-message"></a><span data-ttu-id="4600e-101">Nachricht aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4600e-101">Update message</span></span>

<span data-ttu-id="4600e-102">Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="4600e-102">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4600e-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4600e-103">Permissions</span></span>
<span data-ttu-id="4600e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4600e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4600e-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4600e-106">Permission type</span></span>      | <span data-ttu-id="4600e-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4600e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4600e-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4600e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4600e-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4600e-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4600e-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4600e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4600e-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4600e-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4600e-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4600e-112">Application</span></span> | <span data-ttu-id="4600e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4600e-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4600e-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4600e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4600e-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4600e-115">Request headers</span></span>
| <span data-ttu-id="4600e-116">Name</span><span class="sxs-lookup"><span data-stu-id="4600e-116">Name</span></span>       | <span data-ttu-id="4600e-117">Typ</span><span class="sxs-lookup"><span data-stu-id="4600e-117">Type</span></span> | <span data-ttu-id="4600e-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4600e-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4600e-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4600e-119">Authorization</span></span>  | <span data-ttu-id="4600e-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4600e-120">string</span></span>  | <span data-ttu-id="4600e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4600e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4600e-123">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="4600e-123">Content-Type</span></span> | <span data-ttu-id="4600e-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4600e-124">string</span></span>  | <span data-ttu-id="4600e-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4600e-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="4600e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4600e-127">Request body</span></span>
<span data-ttu-id="4600e-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="4600e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="4600e-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4600e-132">Property</span></span>     | <span data-ttu-id="4600e-133">Typ</span><span class="sxs-lookup"><span data-stu-id="4600e-133">Type</span></span>   |<span data-ttu-id="4600e-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4600e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4600e-135">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="4600e-135">bccRecipients</span></span>|<span data-ttu-id="4600e-136">Empfänger</span><span class="sxs-lookup"><span data-stu-id="4600e-136">Recipient</span></span>|<span data-ttu-id="4600e-137">Die BCC-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4600e-137">The Bcc: recipients for the message.</span></span> <span data-ttu-id="4600e-138">Nur aktualisierbar, wenn isDraft=true.</span><span class="sxs-lookup"><span data-stu-id="4600e-138">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="4600e-139">categories</span><span class="sxs-lookup"><span data-stu-id="4600e-139">categories</span></span>|<span data-ttu-id="4600e-140">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4600e-140">String collection</span></span>|<span data-ttu-id="4600e-141">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="4600e-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="4600e-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="4600e-142">ccRecipients</span></span>|<span data-ttu-id="4600e-143">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="4600e-143">Recipient collection</span></span>|<span data-ttu-id="4600e-144">Die CC-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4600e-144">The Cc: recipients for the message.</span></span> <span data-ttu-id="4600e-145">Nur aktualisierbar, wenn isDraft=true.</span><span class="sxs-lookup"><span data-stu-id="4600e-145">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="4600e-146">Von</span><span class="sxs-lookup"><span data-stu-id="4600e-146">from</span></span>|<span data-ttu-id="4600e-147">Empfänger</span><span class="sxs-lookup"><span data-stu-id="4600e-147">Recipient</span></span>|<span data-ttu-id="4600e-148">Der Postfachbesitzer und der Absender der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4600e-148">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="4600e-149">Nur aktualisierbar, wenn isDraft=true.</span><span class="sxs-lookup"><span data-stu-id="4600e-149">Updatable only if isDraft = true.</span></span> <span data-ttu-id="4600e-150">Muss dem tatsächlich verwendeten Posteingang entsprechen.</span><span class="sxs-lookup"><span data-stu-id="4600e-150">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="4600e-151">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="4600e-151">importance</span></span>|<span data-ttu-id="4600e-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4600e-152">String</span></span>|<span data-ttu-id="4600e-153">Die Wichtigkeit der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4600e-153">The importance of the message: , , .</span></span> <span data-ttu-id="4600e-154">Mögliche Werte sind: `Low`, `Normal` und `High`.</span><span class="sxs-lookup"><span data-stu-id="4600e-154">The possible values are:</span></span>|
|<span data-ttu-id="4600e-155">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="4600e-155">inferenceClassification</span></span> | <span data-ttu-id="4600e-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4600e-156">String</span></span> | <span data-ttu-id="4600e-157">Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung.</span><span class="sxs-lookup"><span data-stu-id="4600e-157">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: , .</span></span> <span data-ttu-id="4600e-158">Mögliche Werte sind `focused`, oder `other`.</span><span class="sxs-lookup"><span data-stu-id="4600e-158">The possible values are `focused`, , or `other`.</span></span> |
|<span data-ttu-id="4600e-159">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="4600e-159">internetMessageId</span></span> |<span data-ttu-id="4600e-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4600e-160">String</span></span> |<span data-ttu-id="4600e-161">Die Nachrichten-ID im von [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) angegebenen Format.</span><span class="sxs-lookup"><span data-stu-id="4600e-161">The message ID in the format specified by [RFC2822](http://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="4600e-162">Nur aktualisierbar, wenn isDraft=true.</span><span class="sxs-lookup"><span data-stu-id="4600e-162">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="4600e-163">isRead</span><span class="sxs-lookup"><span data-stu-id="4600e-163">isRead</span></span>|<span data-ttu-id="4600e-164">Boolesch</span><span class="sxs-lookup"><span data-stu-id="4600e-164">Boolean</span></span>|<span data-ttu-id="4600e-165">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="4600e-165">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="4600e-166">replyTo</span><span class="sxs-lookup"><span data-stu-id="4600e-166">replyTo</span></span>|<span data-ttu-id="4600e-167">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="4600e-167">Recipient collection</span></span>|<span data-ttu-id="4600e-168">Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4600e-168">The email addresses to use when replying.</span></span> <span data-ttu-id="4600e-169">Nur aktualisierbar, wenn isDraft=true.</span><span class="sxs-lookup"><span data-stu-id="4600e-169">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="4600e-170">sender</span><span class="sxs-lookup"><span data-stu-id="4600e-170">sender</span></span>|<span data-ttu-id="4600e-171">Empfänger</span><span class="sxs-lookup"><span data-stu-id="4600e-171">Recipient</span></span>|<span data-ttu-id="4600e-172">Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.</span><span class="sxs-lookup"><span data-stu-id="4600e-172">The account that is actually used to generate the message.</span></span> <span data-ttu-id="4600e-173">Nur aktualisierbar, wenn isDraft=true und wenn eine Nachricht von einem [geteilten Postfach](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes) gesendet wird oder wenn die Nachricht im [Auftrag von jemanden](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926) gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="4600e-173">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="4600e-174">Der Wert muss in jedem Fall dem tatsächlich verwendeten Postfach entsprechen.</span><span class="sxs-lookup"><span data-stu-id="4600e-174">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="4600e-175">toRecipients</span><span class="sxs-lookup"><span data-stu-id="4600e-175">toRecipients</span></span>|<span data-ttu-id="4600e-176">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="4600e-176">Recipient collection</span></span>|<span data-ttu-id="4600e-177">Die Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4600e-177">The To: recipients for the message.</span></span> <span data-ttu-id="4600e-178">Nur aktualisierbar, wenn isDraft=true.</span><span class="sxs-lookup"><span data-stu-id="4600e-178">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="4600e-179">Text</span><span class="sxs-lookup"><span data-stu-id="4600e-179">body</span></span>|<span data-ttu-id="4600e-180">ItemBody</span><span class="sxs-lookup"><span data-stu-id="4600e-180">ItemBody</span></span>|<span data-ttu-id="4600e-181">Der Text der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4600e-181">The body of the message.</span></span> <span data-ttu-id="4600e-182">Nur aktualisierbar, wenn isDraft=true.</span><span class="sxs-lookup"><span data-stu-id="4600e-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="4600e-183">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="4600e-183">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="4600e-184">Boolesch</span><span class="sxs-lookup"><span data-stu-id="4600e-184">Boolean</span></span>|<span data-ttu-id="4600e-185">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="4600e-185">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="4600e-186">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="4600e-186">isReadReceiptRequested</span></span>|<span data-ttu-id="4600e-187">Boolesch</span><span class="sxs-lookup"><span data-stu-id="4600e-187">Boolean</span></span>|<span data-ttu-id="4600e-188">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="4600e-188">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="4600e-189">Betreff</span><span class="sxs-lookup"><span data-stu-id="4600e-189">subject</span></span>|<span data-ttu-id="4600e-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4600e-190">String</span></span>|<span data-ttu-id="4600e-191">Der Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="4600e-191">The subject of the message.</span></span> <span data-ttu-id="4600e-192">Nur aktualisierbar, wenn isDraft=true.</span><span class="sxs-lookup"><span data-stu-id="4600e-192">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="4600e-193">Da die **message**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="4600e-193">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="4600e-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="4600e-194">Response</span></span>

<span data-ttu-id="4600e-195">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4600e-195">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4600e-196">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4600e-196">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4600e-197">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4600e-197">Request</span></span>
<span data-ttu-id="4600e-198">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4600e-198">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4600e-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="4600e-199">Response</span></span>
<span data-ttu-id="4600e-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4600e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4600e-203">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="4600e-203">See also</span></span>

- [<span data-ttu-id="4600e-204">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="4600e-204">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="4600e-205">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="4600e-205">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
