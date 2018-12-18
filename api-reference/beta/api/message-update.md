---
title: Nachricht aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.
author: angelgolfer-ms
ms.openlocfilehash: 9c717e913c641b6dffd582252538965961369a7f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321476"
---
# <a name="update-message"></a><span data-ttu-id="0270a-103">Nachricht aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0270a-103">Update message</span></span>

> <span data-ttu-id="0270a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0270a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0270a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0270a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0270a-106">Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="0270a-106">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0270a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0270a-107">Permissions</span></span>
<span data-ttu-id="0270a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0270a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0270a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0270a-110">Permission type</span></span>      | <span data-ttu-id="0270a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0270a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0270a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0270a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0270a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0270a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0270a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0270a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0270a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0270a-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0270a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0270a-116">Application</span></span> | <span data-ttu-id="0270a-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0270a-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0270a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0270a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0270a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0270a-119">Request headers</span></span>
| <span data-ttu-id="0270a-120">Name</span><span class="sxs-lookup"><span data-stu-id="0270a-120">Name</span></span>       | <span data-ttu-id="0270a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0270a-121">Type</span></span> | <span data-ttu-id="0270a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0270a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0270a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0270a-123">Authorization</span></span>  | <span data-ttu-id="0270a-124">string</span><span class="sxs-lookup"><span data-stu-id="0270a-124">string</span></span>  | <span data-ttu-id="0270a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0270a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0270a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0270a-127">Content-Type</span></span> | <span data-ttu-id="0270a-128">string</span><span class="sxs-lookup"><span data-stu-id="0270a-128">string</span></span>  | <span data-ttu-id="0270a-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0270a-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="0270a-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0270a-131">Request body</span></span>
<span data-ttu-id="0270a-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="0270a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="0270a-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0270a-136">Property</span></span>     | <span data-ttu-id="0270a-137">Typ</span><span class="sxs-lookup"><span data-stu-id="0270a-137">Type</span></span>   |<span data-ttu-id="0270a-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0270a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0270a-139">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="0270a-139">bccRecipients</span></span>|<span data-ttu-id="0270a-140">Empfänger</span><span class="sxs-lookup"><span data-stu-id="0270a-140">Recipient</span></span>|<span data-ttu-id="0270a-141">Die Bcc-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="0270a-141">The Bcc recipients for the message.</span></span> <span data-ttu-id="0270a-142">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="0270a-142">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0270a-143">categories</span><span class="sxs-lookup"><span data-stu-id="0270a-143">categories</span></span>|<span data-ttu-id="0270a-144">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="0270a-144">String collection</span></span>|<span data-ttu-id="0270a-145">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="0270a-145">The categories associated with the message.</span></span>|
|<span data-ttu-id="0270a-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="0270a-146">ccRecipients</span></span>|<span data-ttu-id="0270a-147">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="0270a-147">Recipient collection</span></span>|<span data-ttu-id="0270a-148">Die Cc-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="0270a-148">The Cc recipients for the message.</span></span> <span data-ttu-id="0270a-149">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="0270a-149">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0270a-150">Von</span><span class="sxs-lookup"><span data-stu-id="0270a-150">from</span></span>|<span data-ttu-id="0270a-151">Empfänger</span><span class="sxs-lookup"><span data-stu-id="0270a-151">Recipient</span></span>|<span data-ttu-id="0270a-152">Der Postfachbesitzer und der Absender der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="0270a-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="0270a-153">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="0270a-153">Updatable only if isDraft = true.</span></span> <span data-ttu-id="0270a-154">Muss das tatsächliche Postfach verwendet entsprechen.</span><span class="sxs-lookup"><span data-stu-id="0270a-154">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="0270a-155">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="0270a-155">importance</span></span>|<span data-ttu-id="0270a-156">String</span><span class="sxs-lookup"><span data-stu-id="0270a-156">String</span></span>|<span data-ttu-id="0270a-p109">Wichtigkeit der Nachricht Mögliche Werte: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="0270a-p109">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="0270a-159">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="0270a-159">inferenceClassification</span></span> | <span data-ttu-id="0270a-160">String</span><span class="sxs-lookup"><span data-stu-id="0270a-160">String</span></span> | <span data-ttu-id="0270a-p110">Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung. Mögliche Werte sind: `focused` oder `other`.</span><span class="sxs-lookup"><span data-stu-id="0270a-p110">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="0270a-163">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="0270a-163">internetMessageId</span></span> |<span data-ttu-id="0270a-164">String</span><span class="sxs-lookup"><span data-stu-id="0270a-164">String</span></span> |<span data-ttu-id="0270a-165">Die Nachrichten-ID im von [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) angegebenen Format.</span><span class="sxs-lookup"><span data-stu-id="0270a-165">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="0270a-166">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="0270a-166">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0270a-167">isRead</span><span class="sxs-lookup"><span data-stu-id="0270a-167">isRead</span></span>|<span data-ttu-id="0270a-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0270a-168">Boolean</span></span>|<span data-ttu-id="0270a-169">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="0270a-169">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="0270a-170">replyTo</span><span class="sxs-lookup"><span data-stu-id="0270a-170">replyTo</span></span>|<span data-ttu-id="0270a-171">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="0270a-171">Recipient collection</span></span>|<span data-ttu-id="0270a-172">Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0270a-172">The email addresses to use when replying.</span></span> <span data-ttu-id="0270a-173">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="0270a-173">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0270a-174">sender</span><span class="sxs-lookup"><span data-stu-id="0270a-174">sender</span></span>|<span data-ttu-id="0270a-175">Empfänger</span><span class="sxs-lookup"><span data-stu-id="0270a-175">Recipient</span></span>|<span data-ttu-id="0270a-176">Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.</span><span class="sxs-lookup"><span data-stu-id="0270a-176">The account that is actually used to generate the message.</span></span> <span data-ttu-id="0270a-177">Aktualisierbare nur, wenn IsDraft = true und beim Senden einer Nachricht von einem [freigegebenen Postfach](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)oder Senden einer Nachricht als [Delegieren](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="0270a-177">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="0270a-178">Der Wert muss in jedem Fall das tatsächliche Postfach verwendet entsprechen.</span><span class="sxs-lookup"><span data-stu-id="0270a-178">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="0270a-179">toRecipients</span><span class="sxs-lookup"><span data-stu-id="0270a-179">toRecipients</span></span>|<span data-ttu-id="0270a-180">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="0270a-180">Recipient collection</span></span>|<span data-ttu-id="0270a-181">Die an-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="0270a-181">The To recipients for the message.</span></span> <span data-ttu-id="0270a-182">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="0270a-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0270a-183">body</span><span class="sxs-lookup"><span data-stu-id="0270a-183">body</span></span>|<span data-ttu-id="0270a-184">ItemBody</span><span class="sxs-lookup"><span data-stu-id="0270a-184">ItemBody</span></span>|<span data-ttu-id="0270a-185">Der Text der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="0270a-185">The body of the message.</span></span> <span data-ttu-id="0270a-186">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="0270a-186">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="0270a-187">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="0270a-187">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="0270a-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0270a-188">Boolean</span></span>|<span data-ttu-id="0270a-189">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="0270a-189">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="0270a-190">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="0270a-190">isReadReceiptRequested</span></span>|<span data-ttu-id="0270a-191">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0270a-191">Boolean</span></span>|<span data-ttu-id="0270a-192">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="0270a-192">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="0270a-193">subject</span><span class="sxs-lookup"><span data-stu-id="0270a-193">subject</span></span>|<span data-ttu-id="0270a-194">String</span><span class="sxs-lookup"><span data-stu-id="0270a-194">String</span></span>|<span data-ttu-id="0270a-195">Der Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="0270a-195">The subject of the message.</span></span> <span data-ttu-id="0270a-196">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="0270a-196">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="0270a-197">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="0270a-197">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="0270a-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="0270a-198">Response</span></span>

<span data-ttu-id="0270a-199">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0270a-199">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0270a-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0270a-200">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0270a-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0270a-201">Request</span></span>
<span data-ttu-id="0270a-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0270a-202">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
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
##### <a name="response"></a><span data-ttu-id="0270a-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="0270a-203">Response</span></span>
<span data-ttu-id="0270a-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0270a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
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

## <a name="see-also"></a><span data-ttu-id="0270a-207">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0270a-207">See also</span></span>

- [<span data-ttu-id="0270a-208">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="0270a-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0270a-209">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="0270a-209">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="0270a-210">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="0270a-210">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
