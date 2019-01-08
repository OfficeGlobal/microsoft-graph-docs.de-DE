---
title: Nachricht aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.
author: angelgolfer-ms
ms.openlocfilehash: 04a52e28728eda7d778ac76cdc69080cd5b9edf5
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748542"
---
# <a name="update-message"></a><span data-ttu-id="2d36e-103">Nachricht aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2d36e-103">Update message</span></span>

> <span data-ttu-id="2d36e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2d36e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d36e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d36e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d36e-106">Aktualisieren Sie die Eigenschaften des Message-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2d36e-106">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d36e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2d36e-107">Permissions</span></span>
<span data-ttu-id="2d36e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d36e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d36e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d36e-110">Permission type</span></span>      | <span data-ttu-id="2d36e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d36e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d36e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d36e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2d36e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d36e-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2d36e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d36e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d36e-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d36e-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2d36e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d36e-116">Application</span></span> | <span data-ttu-id="2d36e-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d36e-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d36e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d36e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2d36e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d36e-119">Request headers</span></span>
| <span data-ttu-id="2d36e-120">Name</span><span class="sxs-lookup"><span data-stu-id="2d36e-120">Name</span></span>       | <span data-ttu-id="2d36e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2d36e-121">Type</span></span> | <span data-ttu-id="2d36e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d36e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2d36e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d36e-123">Authorization</span></span>  | <span data-ttu-id="2d36e-124">string</span><span class="sxs-lookup"><span data-stu-id="2d36e-124">string</span></span>  | <span data-ttu-id="2d36e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d36e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d36e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d36e-127">Content-Type</span></span> | <span data-ttu-id="2d36e-128">string</span><span class="sxs-lookup"><span data-stu-id="2d36e-128">string</span></span>  | <span data-ttu-id="2d36e-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d36e-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="2d36e-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d36e-131">Request body</span></span>
<span data-ttu-id="2d36e-132">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2d36e-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2d36e-133">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="2d36e-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2d36e-134">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="2d36e-134">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="2d36e-135">Die folgenden Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="2d36e-135">The following properties can be updated.</span></span>

| <span data-ttu-id="2d36e-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d36e-136">Property</span></span>     | <span data-ttu-id="2d36e-137">Typ</span><span class="sxs-lookup"><span data-stu-id="2d36e-137">Type</span></span>   |<span data-ttu-id="2d36e-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d36e-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d36e-139">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="2d36e-139">bccRecipients</span></span>|<span data-ttu-id="2d36e-140">Empfänger</span><span class="sxs-lookup"><span data-stu-id="2d36e-140">Recipient</span></span>|<span data-ttu-id="2d36e-141">Die Bcc-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="2d36e-141">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="2d36e-142">body</span><span class="sxs-lookup"><span data-stu-id="2d36e-142">body</span></span>|<span data-ttu-id="2d36e-143">ItemBody</span><span class="sxs-lookup"><span data-stu-id="2d36e-143">ItemBody</span></span>|<span data-ttu-id="2d36e-144">Der Text der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="2d36e-144">The body of the message.</span></span> <span data-ttu-id="2d36e-145">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="2d36e-145">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2d36e-146">categories</span><span class="sxs-lookup"><span data-stu-id="2d36e-146">categories</span></span>|<span data-ttu-id="2d36e-147">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="2d36e-147">String collection</span></span>|<span data-ttu-id="2d36e-148">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="2d36e-148">The categories associated with the message.</span></span>|
|<span data-ttu-id="2d36e-149">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="2d36e-149">ccRecipients</span></span>|<span data-ttu-id="2d36e-150">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="2d36e-150">Recipient collection</span></span>|<span data-ttu-id="2d36e-151">Die Cc-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="2d36e-151">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="2d36e-152">Von</span><span class="sxs-lookup"><span data-stu-id="2d36e-152">from</span></span>|<span data-ttu-id="2d36e-153">Empfänger</span><span class="sxs-lookup"><span data-stu-id="2d36e-153">Recipient</span></span>|<span data-ttu-id="2d36e-154">Der Postfachbesitzer und der Absender der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="2d36e-154">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="2d36e-155">Muss das tatsächliche Postfach verwendet entsprechen.</span><span class="sxs-lookup"><span data-stu-id="2d36e-155">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="2d36e-156">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="2d36e-156">importance</span></span>|<span data-ttu-id="2d36e-157">String</span><span class="sxs-lookup"><span data-stu-id="2d36e-157">String</span></span>|<span data-ttu-id="2d36e-p108">Wichtigkeit der Nachricht Mögliche Werte: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="2d36e-p108">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="2d36e-160">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="2d36e-160">inferenceClassification</span></span> | <span data-ttu-id="2d36e-161">String</span><span class="sxs-lookup"><span data-stu-id="2d36e-161">String</span></span> | <span data-ttu-id="2d36e-p109">Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung. Mögliche Werte sind: `focused` oder `other`.</span><span class="sxs-lookup"><span data-stu-id="2d36e-p109">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="2d36e-164">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="2d36e-164">internetMessageId</span></span> |<span data-ttu-id="2d36e-165">String</span><span class="sxs-lookup"><span data-stu-id="2d36e-165">String</span></span> |<span data-ttu-id="2d36e-166">Die Nachrichten-ID im von [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) angegebenen Format.</span><span class="sxs-lookup"><span data-stu-id="2d36e-166">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="2d36e-167">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="2d36e-167">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2d36e-168">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2d36e-168">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="2d36e-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2d36e-169">Boolean</span></span>|<span data-ttu-id="2d36e-170">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="2d36e-170">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="2d36e-171">isRead</span><span class="sxs-lookup"><span data-stu-id="2d36e-171">isRead</span></span>|<span data-ttu-id="2d36e-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2d36e-172">Boolean</span></span>|<span data-ttu-id="2d36e-173">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="2d36e-173">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="2d36e-174">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2d36e-174">isReadReceiptRequested</span></span>|<span data-ttu-id="2d36e-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2d36e-175">Boolean</span></span>|<span data-ttu-id="2d36e-176">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="2d36e-176">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="2d36e-177">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="2d36e-177">multiValueExtendedProperties</span></span>|<span data-ttu-id="2d36e-178">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2d36e-178">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="2d36e-179">Die Auflistung der Mehrfachwert erweiterte Eigenschaften für die Nachricht definiert ist.</span><span class="sxs-lookup"><span data-stu-id="2d36e-179">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="2d36e-180">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="2d36e-180">Nullable.</span></span>|
|<span data-ttu-id="2d36e-181">replyTo</span><span class="sxs-lookup"><span data-stu-id="2d36e-181">replyTo</span></span>|<span data-ttu-id="2d36e-182">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="2d36e-182">Recipient collection</span></span>|<span data-ttu-id="2d36e-183">Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="2d36e-183">The email addresses to use when replying.</span></span> <span data-ttu-id="2d36e-184">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="2d36e-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2d36e-185">sender</span><span class="sxs-lookup"><span data-stu-id="2d36e-185">sender</span></span>|<span data-ttu-id="2d36e-186">Empfänger</span><span class="sxs-lookup"><span data-stu-id="2d36e-186">Recipient</span></span>|<span data-ttu-id="2d36e-187">Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.</span><span class="sxs-lookup"><span data-stu-id="2d36e-187">The account that is actually used to generate the message.</span></span> <span data-ttu-id="2d36e-188">Aktualisierbare beim Senden einer Nachricht von einem [freigegebenen Postfach](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)oder Senden einer Nachricht als [Delegieren](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span><span class="sxs-lookup"><span data-stu-id="2d36e-188">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="2d36e-189">Der Wert muss in jedem Fall das tatsächliche Postfach verwendet entsprechen.</span><span class="sxs-lookup"><span data-stu-id="2d36e-189">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="2d36e-190">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="2d36e-190">singleValueExtendedProperties</span></span>|<span data-ttu-id="2d36e-191">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2d36e-191">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="2d36e-192">Die Auflistung der einwertig erweiterte Eigenschaften für die Nachricht definiert ist.</span><span class="sxs-lookup"><span data-stu-id="2d36e-192">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="2d36e-193">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="2d36e-193">Nullable.</span></span>|
|<span data-ttu-id="2d36e-194">Betreff</span><span class="sxs-lookup"><span data-stu-id="2d36e-194">subject</span></span>|<span data-ttu-id="2d36e-195">String</span><span class="sxs-lookup"><span data-stu-id="2d36e-195">String</span></span>|<span data-ttu-id="2d36e-196">Der Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="2d36e-196">The subject of the message.</span></span> <span data-ttu-id="2d36e-197">Aktualisierbare nur, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="2d36e-197">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2d36e-198">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2d36e-198">toRecipients</span></span>|<span data-ttu-id="2d36e-199">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="2d36e-199">Recipient collection</span></span>|<span data-ttu-id="2d36e-200">Die an-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="2d36e-200">The To recipients for the message.</span></span> |

<span data-ttu-id="2d36e-201">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="2d36e-201">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="2d36e-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d36e-202">Response</span></span>

<span data-ttu-id="2d36e-203">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d36e-203">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d36e-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d36e-204">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d36e-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d36e-205">Request</span></span>
<span data-ttu-id="2d36e-206">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d36e-206">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2d36e-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d36e-207">Response</span></span>
<span data-ttu-id="2d36e-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d36e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2d36e-211">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="2d36e-211">See also</span></span>

- [<span data-ttu-id="2d36e-212">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="2d36e-212">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2d36e-213">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="2d36e-213">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2d36e-214">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="2d36e-214">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
