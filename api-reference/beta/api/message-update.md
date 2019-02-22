---
title: Nachricht aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4b3c54e85c96524305fdba32525e277dd15508ed
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142819"
---
# <a name="update-message"></a><span data-ttu-id="7f5fc-103">Nachricht aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7f5fc-103">Update message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f5fc-104">Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f5fc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7f5fc-105">Permissions</span></span>
<span data-ttu-id="7f5fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f5fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f5fc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f5fc-108">Permission type</span></span>      | <span data-ttu-id="7f5fc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f5fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f5fc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f5fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f5fc-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f5fc-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7f5fc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f5fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f5fc-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f5fc-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7f5fc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f5fc-114">Application</span></span> | <span data-ttu-id="7f5fc-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f5fc-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f5fc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f5fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7f5fc-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f5fc-117">Request headers</span></span>
| <span data-ttu-id="7f5fc-118">Name</span><span class="sxs-lookup"><span data-stu-id="7f5fc-118">Name</span></span>       | <span data-ttu-id="7f5fc-119">Typ</span><span class="sxs-lookup"><span data-stu-id="7f5fc-119">Type</span></span> | <span data-ttu-id="7f5fc-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f5fc-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7f5fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f5fc-121">Authorization</span></span>  | <span data-ttu-id="7f5fc-122">string</span><span class="sxs-lookup"><span data-stu-id="7f5fc-122">string</span></span>  | <span data-ttu-id="7f5fc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f5fc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f5fc-125">Content-Type</span></span> | <span data-ttu-id="7f5fc-126">string</span><span class="sxs-lookup"><span data-stu-id="7f5fc-126">string</span></span>  | <span data-ttu-id="7f5fc-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="7f5fc-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f5fc-129">Request body</span></span>
<span data-ttu-id="7f5fc-130">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7f5fc-131">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7f5fc-132">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="7f5fc-133">Die folgenden Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-133">The following properties can be updated.</span></span>

| <span data-ttu-id="7f5fc-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7f5fc-134">Property</span></span>     | <span data-ttu-id="7f5fc-135">Typ</span><span class="sxs-lookup"><span data-stu-id="7f5fc-135">Type</span></span>   |<span data-ttu-id="7f5fc-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f5fc-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f5fc-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="7f5fc-137">bccRecipients</span></span>|<span data-ttu-id="7f5fc-138">Empfänger</span><span class="sxs-lookup"><span data-stu-id="7f5fc-138">Recipient</span></span>|<span data-ttu-id="7f5fc-139">Die Bcc:-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="7f5fc-140">body</span><span class="sxs-lookup"><span data-stu-id="7f5fc-140">body</span></span>|<span data-ttu-id="7f5fc-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="7f5fc-141">ItemBody</span></span>|<span data-ttu-id="7f5fc-142">Der Text der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-142">The body of the message.</span></span> <span data-ttu-id="7f5fc-143">Kann nur aktualisiert werden, wenn isDraft = True.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="7f5fc-144">categories</span><span class="sxs-lookup"><span data-stu-id="7f5fc-144">categories</span></span>|<span data-ttu-id="7f5fc-145">String collection</span><span class="sxs-lookup"><span data-stu-id="7f5fc-145">String collection</span></span>|<span data-ttu-id="7f5fc-146">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="7f5fc-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="7f5fc-147">ccRecipients</span></span>|<span data-ttu-id="7f5fc-148">Empfänger-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7f5fc-148">Recipient collection</span></span>|<span data-ttu-id="7f5fc-149">Die Cc:-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="7f5fc-150">Flag</span><span class="sxs-lookup"><span data-stu-id="7f5fc-150">flag</span></span>|[<span data-ttu-id="7f5fc-151">followupFlag</span><span class="sxs-lookup"><span data-stu-id="7f5fc-151">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="7f5fc-152">Der Wert des Flags, der den Status, das Startdatum, das Fälligkeitsdatum oder das Enddatum für die Nachricht angibt.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-152">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="7f5fc-153">Von</span><span class="sxs-lookup"><span data-stu-id="7f5fc-153">from</span></span>|<span data-ttu-id="7f5fc-154">Empfänger</span><span class="sxs-lookup"><span data-stu-id="7f5fc-154">Recipient</span></span>|<span data-ttu-id="7f5fc-155">Der Postfachbesitzer und Absender der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-155">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="7f5fc-156">Muss dem tatsächlich verwendeten Postfach entsprechen.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-156">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="7f5fc-157">importance</span><span class="sxs-lookup"><span data-stu-id="7f5fc-157">importance</span></span>|<span data-ttu-id="7f5fc-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f5fc-158">String</span></span>|<span data-ttu-id="7f5fc-p107">Wichtigkeit der Nachricht Mögliche Werte: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="7f5fc-161">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="7f5fc-161">inferenceClassification</span></span> | <span data-ttu-id="7f5fc-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f5fc-162">String</span></span> | <span data-ttu-id="7f5fc-p108">Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung. Mögliche Werte sind: `focused` oder `other`.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="7f5fc-165">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="7f5fc-165">internetMessageId</span></span> |<span data-ttu-id="7f5fc-166">String</span><span class="sxs-lookup"><span data-stu-id="7f5fc-166">String</span></span> |<span data-ttu-id="7f5fc-167">Die Nachrichten-ID im von [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) angegebenen Format.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-167">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="7f5fc-168">Kann nur aktualisiert werden, wenn isDraft = True.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-168">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="7f5fc-169">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="7f5fc-169">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="7f5fc-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f5fc-170">Boolean</span></span>|<span data-ttu-id="7f5fc-171">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-171">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="7f5fc-172">isRead</span><span class="sxs-lookup"><span data-stu-id="7f5fc-172">isRead</span></span>|<span data-ttu-id="7f5fc-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f5fc-173">Boolean</span></span>|<span data-ttu-id="7f5fc-174">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-174">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="7f5fc-175">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="7f5fc-175">isReadReceiptRequested</span></span>|<span data-ttu-id="7f5fc-176">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7f5fc-176">Boolean</span></span>|<span data-ttu-id="7f5fc-177">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-177">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="7f5fc-178">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7f5fc-178">multiValueExtendedProperties</span></span>|<span data-ttu-id="7f5fc-179">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7f5fc-179">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="7f5fc-180">Die Sammlung der für die Nachricht definierten mehrwertigen erweiterten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-180">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="7f5fc-181">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-181">Nullable.</span></span>|
|<span data-ttu-id="7f5fc-182">replyTo</span><span class="sxs-lookup"><span data-stu-id="7f5fc-182">replyTo</span></span>|<span data-ttu-id="7f5fc-183">Empfänger-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7f5fc-183">Recipient collection</span></span>|<span data-ttu-id="7f5fc-184">Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-184">The email addresses to use when replying.</span></span> <span data-ttu-id="7f5fc-185">Kann nur aktualisiert werden, wenn isDraft = True.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-185">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="7f5fc-186">sender</span><span class="sxs-lookup"><span data-stu-id="7f5fc-186">sender</span></span>|<span data-ttu-id="7f5fc-187">Empfänger</span><span class="sxs-lookup"><span data-stu-id="7f5fc-187">Recipient</span></span>|<span data-ttu-id="7f5fc-188">Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-188">The account that is actually used to generate the message.</span></span> <span data-ttu-id="7f5fc-189">Kann beim Senden einer Nachricht aus einem [freigegebenen Postfach](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes) oder beim Senden einer Nachricht als[Stellvertretung](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-189">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="7f5fc-190">Der Wert muss auf jeden Fall dem tatsächlich verwendeten Postfach entsprechen.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-190">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="7f5fc-191">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="7f5fc-191">singleValueExtendedProperties</span></span>|<span data-ttu-id="7f5fc-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7f5fc-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="7f5fc-193">Die Sammlung der für die Nachricht definierten einwertigen erweiterten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-193">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="7f5fc-194">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-194">Nullable.</span></span>|
|<span data-ttu-id="7f5fc-195">subject</span><span class="sxs-lookup"><span data-stu-id="7f5fc-195">subject</span></span>|<span data-ttu-id="7f5fc-196">String</span><span class="sxs-lookup"><span data-stu-id="7f5fc-196">String</span></span>|<span data-ttu-id="7f5fc-197">Der Betreff der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-197">The subject of the message.</span></span> <span data-ttu-id="7f5fc-198">Kann nur aktualisiert werden, wenn isDraft = True.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-198">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="7f5fc-199">toRecipients</span><span class="sxs-lookup"><span data-stu-id="7f5fc-199">toRecipients</span></span>|<span data-ttu-id="7f5fc-200">Empfänger-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7f5fc-200">Recipient collection</span></span>|<span data-ttu-id="7f5fc-201">Die An:-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-201">The To recipients for the message.</span></span> |

<span data-ttu-id="7f5fc-202">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-202">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="7f5fc-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f5fc-203">Response</span></span>

<span data-ttu-id="7f5fc-204">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-204">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f5fc-205">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f5fc-205">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f5fc-206">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f5fc-206">Request</span></span>
<span data-ttu-id="7f5fc-207">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-207">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="7f5fc-208">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f5fc-208">Response</span></span>
<span data-ttu-id="7f5fc-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f5fc-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7f5fc-212">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7f5fc-212">See also</span></span>

- [<span data-ttu-id="7f5fc-213">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="7f5fc-213">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7f5fc-214">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="7f5fc-214">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7f5fc-215">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="7f5fc-215">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
