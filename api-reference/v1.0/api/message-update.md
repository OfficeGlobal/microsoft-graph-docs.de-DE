---
title: Nachricht aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.
author: angelgolfer-ms
ms.openlocfilehash: b8f39dc9648203f86749ba06b88bf2f74b79d88a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337541"
---
# <a name="update-message"></a><span data-ttu-id="79ad7-103">Nachricht aktualisieren</span><span class="sxs-lookup"><span data-stu-id="79ad7-103">Update message</span></span>

<span data-ttu-id="79ad7-104">Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="79ad7-104">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="79ad7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="79ad7-105">Permissions</span></span>
<span data-ttu-id="79ad7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79ad7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79ad7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79ad7-108">Permission type</span></span>      | <span data-ttu-id="79ad7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79ad7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79ad7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79ad7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79ad7-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79ad7-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="79ad7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79ad7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79ad7-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79ad7-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="79ad7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79ad7-114">Application</span></span> | <span data-ttu-id="79ad7-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79ad7-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="79ad7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79ad7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="79ad7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79ad7-117">Request headers</span></span>
| <span data-ttu-id="79ad7-118">Name</span><span class="sxs-lookup"><span data-stu-id="79ad7-118">Name</span></span>       | <span data-ttu-id="79ad7-119">Typ</span><span class="sxs-lookup"><span data-stu-id="79ad7-119">Type</span></span> | <span data-ttu-id="79ad7-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79ad7-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="79ad7-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="79ad7-121">Authorization</span></span>  | <span data-ttu-id="79ad7-122">string</span><span class="sxs-lookup"><span data-stu-id="79ad7-122">string</span></span>  | <span data-ttu-id="79ad7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="79ad7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79ad7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79ad7-125">Content-Type</span></span> | <span data-ttu-id="79ad7-126">string</span><span class="sxs-lookup"><span data-stu-id="79ad7-126">string</span></span>  | <span data-ttu-id="79ad7-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="79ad7-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="79ad7-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79ad7-129">Request body</span></span>
<span data-ttu-id="79ad7-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="79ad7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="79ad7-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79ad7-134">Property</span></span>     | <span data-ttu-id="79ad7-135">Typ</span><span class="sxs-lookup"><span data-stu-id="79ad7-135">Type</span></span>   |<span data-ttu-id="79ad7-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79ad7-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79ad7-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="79ad7-137">bccRecipients</span></span>|<span data-ttu-id="79ad7-138">Empfänger</span><span class="sxs-lookup"><span data-stu-id="79ad7-138">Recipient</span></span>|<span data-ttu-id="79ad7-139">Die Bcc-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="79ad7-139">The Bcc recipients for the message.</span></span> <span data-ttu-id="79ad7-140">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="79ad7-140">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="79ad7-141">categories</span><span class="sxs-lookup"><span data-stu-id="79ad7-141">categories</span></span>|<span data-ttu-id="79ad7-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="79ad7-142">String collection</span></span>|<span data-ttu-id="79ad7-143">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="79ad7-143">The categories associated with the message.</span></span>|
|<span data-ttu-id="79ad7-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="79ad7-144">ccRecipients</span></span>|<span data-ttu-id="79ad7-145">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="79ad7-145">Recipient collection</span></span>|<span data-ttu-id="79ad7-146">Die Cc-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="79ad7-146">The Cc recipients for the message.</span></span> <span data-ttu-id="79ad7-147">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="79ad7-147">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="79ad7-148">Von</span><span class="sxs-lookup"><span data-stu-id="79ad7-148">from</span></span>|<span data-ttu-id="79ad7-149">Empfänger</span><span class="sxs-lookup"><span data-stu-id="79ad7-149">Recipient</span></span>|<span data-ttu-id="79ad7-150">Der Postfachbesitzer und der Absender der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="79ad7-150">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="79ad7-151">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="79ad7-151">Updatable only if isDraft = true.</span></span> <span data-ttu-id="79ad7-152">Muss das tatsächliche Postfach verwendet entsprechen.</span><span class="sxs-lookup"><span data-stu-id="79ad7-152">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="79ad7-153">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="79ad7-153">importance</span></span>|<span data-ttu-id="79ad7-154">String</span><span class="sxs-lookup"><span data-stu-id="79ad7-154">String</span></span>|<span data-ttu-id="79ad7-155">Die Wichtigkeit der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="79ad7-155">The importance of the message.</span></span> <span data-ttu-id="79ad7-156">Die möglichen Werte sind: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="79ad7-156">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="79ad7-157">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="79ad7-157">inferenceClassification</span></span> | <span data-ttu-id="79ad7-158">String</span><span class="sxs-lookup"><span data-stu-id="79ad7-158">String</span></span> | <span data-ttu-id="79ad7-159">Die Klassifizierung der Nachricht für Benutzer, basierend auf abgeleiteten Relevanz oder Wichtigkeit oder auf eine explizite Außerkraftsetzung vorliegt.</span><span class="sxs-lookup"><span data-stu-id="79ad7-159">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="79ad7-160">Die möglichen Werte sind: `focused` oder `other`.</span><span class="sxs-lookup"><span data-stu-id="79ad7-160">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="79ad7-161">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="79ad7-161">internetMessageId</span></span> |<span data-ttu-id="79ad7-162">String</span><span class="sxs-lookup"><span data-stu-id="79ad7-162">String</span></span> |<span data-ttu-id="79ad7-163">Die Nachrichten-ID im von [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) angegebenen Format.</span><span class="sxs-lookup"><span data-stu-id="79ad7-163">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="79ad7-164">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="79ad7-164">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="79ad7-165">isRead</span><span class="sxs-lookup"><span data-stu-id="79ad7-165">isRead</span></span>|<span data-ttu-id="79ad7-166">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="79ad7-166">Boolean</span></span>|<span data-ttu-id="79ad7-167">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="79ad7-167">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="79ad7-168">replyTo</span><span class="sxs-lookup"><span data-stu-id="79ad7-168">replyTo</span></span>|<span data-ttu-id="79ad7-169">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="79ad7-169">Recipient collection</span></span>|<span data-ttu-id="79ad7-170">Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="79ad7-170">The email addresses to use when replying.</span></span> <span data-ttu-id="79ad7-171">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="79ad7-171">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="79ad7-172">sender</span><span class="sxs-lookup"><span data-stu-id="79ad7-172">sender</span></span>|<span data-ttu-id="79ad7-173">Empfänger</span><span class="sxs-lookup"><span data-stu-id="79ad7-173">Recipient</span></span>|<span data-ttu-id="79ad7-174">Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.</span><span class="sxs-lookup"><span data-stu-id="79ad7-174">The account that is actually used to generate the message.</span></span> <span data-ttu-id="79ad7-175">Aktualisierbare nur, wenn IsDraft = true und beim Senden einer Nachricht von einem [freigegebenen Postfach](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)oder Senden einer Nachricht als [Delegieren](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="79ad7-175">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="79ad7-176">Der Wert muss in jedem Fall das tatsächliche Postfach verwendet entsprechen.</span><span class="sxs-lookup"><span data-stu-id="79ad7-176">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="79ad7-177">toRecipients</span><span class="sxs-lookup"><span data-stu-id="79ad7-177">toRecipients</span></span>|<span data-ttu-id="79ad7-178">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="79ad7-178">Recipient collection</span></span>|<span data-ttu-id="79ad7-179">Die an-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="79ad7-179">The To recipients for the message.</span></span> <span data-ttu-id="79ad7-180">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="79ad7-180">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="79ad7-181">body</span><span class="sxs-lookup"><span data-stu-id="79ad7-181">body</span></span>|<span data-ttu-id="79ad7-182">ItemBody</span><span class="sxs-lookup"><span data-stu-id="79ad7-182">ItemBody</span></span>|<span data-ttu-id="79ad7-183">Der Text der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="79ad7-183">The body of the message.</span></span> <span data-ttu-id="79ad7-184">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="79ad7-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="79ad7-185">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="79ad7-185">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="79ad7-186">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="79ad7-186">Boolean</span></span>|<span data-ttu-id="79ad7-187">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="79ad7-187">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="79ad7-188">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="79ad7-188">isReadReceiptRequested</span></span>|<span data-ttu-id="79ad7-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="79ad7-189">Boolean</span></span>|<span data-ttu-id="79ad7-190">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="79ad7-190">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="79ad7-191">subject</span><span class="sxs-lookup"><span data-stu-id="79ad7-191">subject</span></span>|<span data-ttu-id="79ad7-192">String</span><span class="sxs-lookup"><span data-stu-id="79ad7-192">String</span></span>|<span data-ttu-id="79ad7-193">Der Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="79ad7-193">The subject of the message.</span></span> <span data-ttu-id="79ad7-194">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="79ad7-194">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="79ad7-195">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="79ad7-195">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="79ad7-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="79ad7-196">Response</span></span>

<span data-ttu-id="79ad7-197">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79ad7-197">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79ad7-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79ad7-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79ad7-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79ad7-199">Request</span></span>
<span data-ttu-id="79ad7-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79ad7-200">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="79ad7-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="79ad7-201">Response</span></span>
<span data-ttu-id="79ad7-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79ad7-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="79ad7-205">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="79ad7-205">See also</span></span>

- [<span data-ttu-id="79ad7-206">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="79ad7-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="79ad7-207">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="79ad7-207">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
