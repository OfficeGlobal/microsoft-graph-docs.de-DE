---
title: Nachricht aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.
ms.openlocfilehash: 7d78f3827618378299043c601fcf490556b5d5b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016560"
---
# <a name="update-message"></a><span data-ttu-id="87c50-103">Nachricht aktualisieren</span><span class="sxs-lookup"><span data-stu-id="87c50-103">Update message</span></span>

<span data-ttu-id="87c50-104">Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="87c50-104">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="87c50-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87c50-105">Permissions</span></span>
<span data-ttu-id="87c50-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87c50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87c50-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87c50-108">Permission type</span></span>      | <span data-ttu-id="87c50-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87c50-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87c50-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87c50-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87c50-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87c50-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="87c50-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87c50-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87c50-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87c50-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="87c50-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87c50-114">Application</span></span> | <span data-ttu-id="87c50-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87c50-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="87c50-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c50-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="87c50-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87c50-117">Request headers</span></span>
| <span data-ttu-id="87c50-118">Name</span><span class="sxs-lookup"><span data-stu-id="87c50-118">Name</span></span>       | <span data-ttu-id="87c50-119">Typ</span><span class="sxs-lookup"><span data-stu-id="87c50-119">Type</span></span> | <span data-ttu-id="87c50-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87c50-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="87c50-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="87c50-121">Authorization</span></span>  | <span data-ttu-id="87c50-122">string</span><span class="sxs-lookup"><span data-stu-id="87c50-122">string</span></span>  | <span data-ttu-id="87c50-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87c50-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87c50-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87c50-125">Content-Type</span></span> | <span data-ttu-id="87c50-126">string</span><span class="sxs-lookup"><span data-stu-id="87c50-126">string</span></span>  | <span data-ttu-id="87c50-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87c50-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="87c50-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87c50-129">Request body</span></span>
<span data-ttu-id="87c50-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="87c50-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="87c50-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87c50-134">Property</span></span>     | <span data-ttu-id="87c50-135">Typ</span><span class="sxs-lookup"><span data-stu-id="87c50-135">Type</span></span>   |<span data-ttu-id="87c50-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87c50-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87c50-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="87c50-137">bccRecipients</span></span>|<span data-ttu-id="87c50-138">Empfänger</span><span class="sxs-lookup"><span data-stu-id="87c50-138">Recipient</span></span>|<span data-ttu-id="87c50-139">Die Bcc-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="87c50-139">The Bcc recipients for the message.</span></span> <span data-ttu-id="87c50-140">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="87c50-140">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="87c50-141">categories</span><span class="sxs-lookup"><span data-stu-id="87c50-141">categories</span></span>|<span data-ttu-id="87c50-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="87c50-142">String collection</span></span>|<span data-ttu-id="87c50-143">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="87c50-143">The categories associated with the message.</span></span>|
|<span data-ttu-id="87c50-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="87c50-144">ccRecipients</span></span>|<span data-ttu-id="87c50-145">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="87c50-145">Recipient collection</span></span>|<span data-ttu-id="87c50-146">Die Cc-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="87c50-146">The Cc recipients for the message.</span></span> <span data-ttu-id="87c50-147">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="87c50-147">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="87c50-148">Von</span><span class="sxs-lookup"><span data-stu-id="87c50-148">from</span></span>|<span data-ttu-id="87c50-149">Empfänger</span><span class="sxs-lookup"><span data-stu-id="87c50-149">Recipient</span></span>|<span data-ttu-id="87c50-150">Der Postfachbesitzer und der Absender der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="87c50-150">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="87c50-151">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="87c50-151">Updatable only if isDraft = true.</span></span> <span data-ttu-id="87c50-152">Muss das tatsächliche Postfach verwendet entsprechen.</span><span class="sxs-lookup"><span data-stu-id="87c50-152">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="87c50-153">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="87c50-153">importance</span></span>|<span data-ttu-id="87c50-154">String</span><span class="sxs-lookup"><span data-stu-id="87c50-154">String</span></span>|<span data-ttu-id="87c50-155">Die Wichtigkeit der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="87c50-155">The importance of the message.</span></span> <span data-ttu-id="87c50-156">Die möglichen Werte sind: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="87c50-156">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="87c50-157">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="87c50-157">inferenceClassification</span></span> | <span data-ttu-id="87c50-158">String</span><span class="sxs-lookup"><span data-stu-id="87c50-158">String</span></span> | <span data-ttu-id="87c50-159">Die Klassifizierung der Nachricht für Benutzer, basierend auf abgeleiteten Relevanz oder Wichtigkeit oder auf eine explizite Außerkraftsetzung vorliegt.</span><span class="sxs-lookup"><span data-stu-id="87c50-159">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="87c50-160">Die möglichen Werte sind: `focused` oder `other`.</span><span class="sxs-lookup"><span data-stu-id="87c50-160">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="87c50-161">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="87c50-161">internetMessageId</span></span> |<span data-ttu-id="87c50-162">String</span><span class="sxs-lookup"><span data-stu-id="87c50-162">String</span></span> |<span data-ttu-id="87c50-163">Die Nachrichten-ID im von [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) angegebenen Format.</span><span class="sxs-lookup"><span data-stu-id="87c50-163">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="87c50-164">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="87c50-164">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="87c50-165">isRead</span><span class="sxs-lookup"><span data-stu-id="87c50-165">isRead</span></span>|<span data-ttu-id="87c50-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="87c50-166">Boolean</span></span>|<span data-ttu-id="87c50-167">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="87c50-167">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="87c50-168">replyTo</span><span class="sxs-lookup"><span data-stu-id="87c50-168">replyTo</span></span>|<span data-ttu-id="87c50-169">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="87c50-169">Recipient collection</span></span>|<span data-ttu-id="87c50-170">Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="87c50-170">The email addresses to use when replying.</span></span> <span data-ttu-id="87c50-171">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="87c50-171">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="87c50-172">sender</span><span class="sxs-lookup"><span data-stu-id="87c50-172">sender</span></span>|<span data-ttu-id="87c50-173">Empfänger</span><span class="sxs-lookup"><span data-stu-id="87c50-173">Recipient</span></span>|<span data-ttu-id="87c50-174">Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.</span><span class="sxs-lookup"><span data-stu-id="87c50-174">The account that is actually used to generate the message.</span></span> <span data-ttu-id="87c50-175">Aktualisierbare nur, wenn IsDraft = true und beim Senden einer Nachricht von einem [freigegebenen Postfach](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)oder Senden einer Nachricht als [Delegieren](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="87c50-175">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="87c50-176">Der Wert muss in jedem Fall das tatsächliche Postfach verwendet entsprechen.</span><span class="sxs-lookup"><span data-stu-id="87c50-176">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="87c50-177">toRecipients</span><span class="sxs-lookup"><span data-stu-id="87c50-177">toRecipients</span></span>|<span data-ttu-id="87c50-178">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="87c50-178">Recipient collection</span></span>|<span data-ttu-id="87c50-179">Die an-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="87c50-179">The To recipients for the message.</span></span> <span data-ttu-id="87c50-180">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="87c50-180">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="87c50-181">body</span><span class="sxs-lookup"><span data-stu-id="87c50-181">body</span></span>|<span data-ttu-id="87c50-182">ItemBody</span><span class="sxs-lookup"><span data-stu-id="87c50-182">ItemBody</span></span>|<span data-ttu-id="87c50-183">Der Text der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="87c50-183">The body of the message.</span></span> <span data-ttu-id="87c50-184">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="87c50-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="87c50-185">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="87c50-185">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="87c50-186">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="87c50-186">Boolean</span></span>|<span data-ttu-id="87c50-187">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="87c50-187">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="87c50-188">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="87c50-188">isReadReceiptRequested</span></span>|<span data-ttu-id="87c50-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="87c50-189">Boolean</span></span>|<span data-ttu-id="87c50-190">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="87c50-190">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="87c50-191">subject</span><span class="sxs-lookup"><span data-stu-id="87c50-191">subject</span></span>|<span data-ttu-id="87c50-192">String</span><span class="sxs-lookup"><span data-stu-id="87c50-192">String</span></span>|<span data-ttu-id="87c50-193">Der Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="87c50-193">The subject of the message.</span></span> <span data-ttu-id="87c50-194">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="87c50-194">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="87c50-195">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="87c50-195">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="87c50-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c50-196">Response</span></span>

<span data-ttu-id="87c50-197">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87c50-197">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87c50-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87c50-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87c50-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c50-199">Request</span></span>
<span data-ttu-id="87c50-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87c50-200">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="87c50-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c50-201">Response</span></span>
<span data-ttu-id="87c50-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87c50-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="87c50-205">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="87c50-205">See also</span></span>

- [<span data-ttu-id="87c50-206">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="87c50-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="87c50-207">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="87c50-207">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
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
