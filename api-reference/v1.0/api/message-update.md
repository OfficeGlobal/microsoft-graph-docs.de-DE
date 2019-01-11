---
title: Nachricht aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 24705fbf986f9ecf1142e66d189ae2071e1be223
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884784"
---
# <a name="update-message"></a><span data-ttu-id="ee574-103">Nachricht aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ee574-103">Update message</span></span>

<span data-ttu-id="ee574-104">Aktualisieren Sie die Eigenschaften des Message-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ee574-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee574-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ee574-105">Permissions</span></span>
<span data-ttu-id="ee574-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee574-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee574-108">Permission type</span></span>      | <span data-ttu-id="ee574-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee574-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee574-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee574-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee574-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee574-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ee574-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee574-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee574-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee574-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ee574-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee574-114">Application</span></span> | <span data-ttu-id="ee574-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee574-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee574-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee574-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ee574-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee574-117">Request headers</span></span>
| <span data-ttu-id="ee574-118">Name</span><span class="sxs-lookup"><span data-stu-id="ee574-118">Name</span></span>       | <span data-ttu-id="ee574-119">Typ</span><span class="sxs-lookup"><span data-stu-id="ee574-119">Type</span></span> | <span data-ttu-id="ee574-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee574-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ee574-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee574-121">Authorization</span></span>  | <span data-ttu-id="ee574-122">string</span><span class="sxs-lookup"><span data-stu-id="ee574-122">string</span></span>  | <span data-ttu-id="ee574-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ee574-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee574-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee574-125">Content-Type</span></span> | <span data-ttu-id="ee574-126">string</span><span class="sxs-lookup"><span data-stu-id="ee574-126">string</span></span>  | <span data-ttu-id="ee574-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ee574-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="ee574-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ee574-129">Request body</span></span>
<span data-ttu-id="ee574-130">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ee574-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ee574-131">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="ee574-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ee574-132">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="ee574-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="ee574-133">Die folgenden Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="ee574-133">The following properties can be updated.</span></span>

| <span data-ttu-id="ee574-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ee574-134">Property</span></span>     | <span data-ttu-id="ee574-135">Typ</span><span class="sxs-lookup"><span data-stu-id="ee574-135">Type</span></span>   |<span data-ttu-id="ee574-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee574-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee574-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="ee574-137">bccRecipients</span></span>|<span data-ttu-id="ee574-138">Empfänger</span><span class="sxs-lookup"><span data-stu-id="ee574-138">Recipient</span></span>|<span data-ttu-id="ee574-139">Die Bcc-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="ee574-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="ee574-140">body</span><span class="sxs-lookup"><span data-stu-id="ee574-140">body</span></span>|<span data-ttu-id="ee574-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="ee574-141">ItemBody</span></span>|<span data-ttu-id="ee574-142">Der Text der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="ee574-142">The body of the message.</span></span> <span data-ttu-id="ee574-143">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="ee574-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="ee574-144">categories</span><span class="sxs-lookup"><span data-stu-id="ee574-144">categories</span></span>|<span data-ttu-id="ee574-145">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ee574-145">String collection</span></span>|<span data-ttu-id="ee574-146">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="ee574-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="ee574-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="ee574-147">ccRecipients</span></span>|<span data-ttu-id="ee574-148">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="ee574-148">Recipient collection</span></span>|<span data-ttu-id="ee574-149">Die Cc-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="ee574-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="ee574-150">Von</span><span class="sxs-lookup"><span data-stu-id="ee574-150">from</span></span>|<span data-ttu-id="ee574-151">Empfänger</span><span class="sxs-lookup"><span data-stu-id="ee574-151">Recipient</span></span>|<span data-ttu-id="ee574-152">Der Postfachbesitzer und der Absender der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="ee574-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="ee574-153">Muss das tatsächliche Postfach verwendet entsprechen.</span><span class="sxs-lookup"><span data-stu-id="ee574-153">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="ee574-154">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="ee574-154">importance</span></span>|<span data-ttu-id="ee574-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee574-155">String</span></span>|<span data-ttu-id="ee574-156">Die Wichtigkeit der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="ee574-156">The importance of the message.</span></span> <span data-ttu-id="ee574-157">Die möglichen Werte sind: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="ee574-157">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="ee574-158">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="ee574-158">inferenceClassification</span></span> | <span data-ttu-id="ee574-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee574-159">String</span></span> | <span data-ttu-id="ee574-160">Die Klassifizierung der Nachricht für Benutzer, basierend auf abgeleiteten Relevanz oder Wichtigkeit oder auf eine explizite Außerkraftsetzung vorliegt.</span><span class="sxs-lookup"><span data-stu-id="ee574-160">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="ee574-161">Die möglichen Werte sind: `focused` oder `other`.</span><span class="sxs-lookup"><span data-stu-id="ee574-161">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="ee574-162">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="ee574-162">internetMessageId</span></span> |<span data-ttu-id="ee574-163">String</span><span class="sxs-lookup"><span data-stu-id="ee574-163">String</span></span> |<span data-ttu-id="ee574-164">Die Nachrichten-ID im von [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) angegebenen Format.</span><span class="sxs-lookup"><span data-stu-id="ee574-164">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="ee574-165">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="ee574-165">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="ee574-166">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ee574-166">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="ee574-167">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ee574-167">Boolean</span></span>|<span data-ttu-id="ee574-168">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="ee574-168">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="ee574-169">isRead</span><span class="sxs-lookup"><span data-stu-id="ee574-169">isRead</span></span>|<span data-ttu-id="ee574-170">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ee574-170">Boolean</span></span>|<span data-ttu-id="ee574-171">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="ee574-171">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="ee574-172">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="ee574-172">isReadReceiptRequested</span></span>|<span data-ttu-id="ee574-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ee574-173">Boolean</span></span>|<span data-ttu-id="ee574-174">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="ee574-174">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="ee574-175">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ee574-175">multiValueExtendedProperties</span></span>|<span data-ttu-id="ee574-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ee574-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="ee574-177">Die Auflistung der Mehrfachwert erweiterte Eigenschaften für die Nachricht definiert ist.</span><span class="sxs-lookup"><span data-stu-id="ee574-177">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="ee574-178">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="ee574-178">Nullable.</span></span>|
|<span data-ttu-id="ee574-179">replyTo</span><span class="sxs-lookup"><span data-stu-id="ee574-179">replyTo</span></span>|<span data-ttu-id="ee574-180">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="ee574-180">Recipient collection</span></span>|<span data-ttu-id="ee574-181">Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ee574-181">The email addresses to use when replying.</span></span> <span data-ttu-id="ee574-182">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="ee574-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="ee574-183">sender</span><span class="sxs-lookup"><span data-stu-id="ee574-183">sender</span></span>|<span data-ttu-id="ee574-184">Empfänger</span><span class="sxs-lookup"><span data-stu-id="ee574-184">Recipient</span></span>|<span data-ttu-id="ee574-185">Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.</span><span class="sxs-lookup"><span data-stu-id="ee574-185">The account that is actually used to generate the message.</span></span> <span data-ttu-id="ee574-186">Aktualisierbare beim Senden einer Nachricht von einem [freigegebenen Postfach](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)oder Senden einer Nachricht als [Delegieren](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="ee574-186">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="ee574-187">Der Wert muss in jedem Fall das tatsächliche Postfach verwendet entsprechen.</span><span class="sxs-lookup"><span data-stu-id="ee574-187">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="ee574-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ee574-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="ee574-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ee574-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="ee574-190">Die Auflistung der einwertig erweiterte Eigenschaften für die Nachricht definiert ist.</span><span class="sxs-lookup"><span data-stu-id="ee574-190">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="ee574-191">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="ee574-191">Nullable.</span></span>|
|<span data-ttu-id="ee574-192">Betreff</span><span class="sxs-lookup"><span data-stu-id="ee574-192">subject</span></span>|<span data-ttu-id="ee574-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee574-193">String</span></span>|<span data-ttu-id="ee574-194">Der Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="ee574-194">The subject of the message.</span></span> <span data-ttu-id="ee574-195">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="ee574-195">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="ee574-196">toRecipients</span><span class="sxs-lookup"><span data-stu-id="ee574-196">toRecipients</span></span>|<span data-ttu-id="ee574-197">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="ee574-197">Recipient collection</span></span>|<span data-ttu-id="ee574-198">Die an-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="ee574-198">The To recipients for the message.</span></span>|

<span data-ttu-id="ee574-199">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="ee574-199">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="ee574-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee574-200">Response</span></span>

<span data-ttu-id="ee574-201">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee574-201">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ee574-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee574-202">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee574-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee574-203">Request</span></span>
<span data-ttu-id="ee574-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ee574-204">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ee574-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee574-205">Response</span></span>
<span data-ttu-id="ee574-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee574-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ee574-209">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ee574-209">See also</span></span>

- [<span data-ttu-id="ee574-210">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ee574-210">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ee574-211">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="ee574-211">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
