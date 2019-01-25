---
title: Nachricht aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5a42e9d6a10e79a4ae801cca464c912dc6fade7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515685"
---
# <a name="update-message"></a><span data-ttu-id="018d3-103">Nachricht aktualisieren</span><span class="sxs-lookup"><span data-stu-id="018d3-103">Update message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="018d3-104">Mit dieser API können Sie die Eigenschaften eines Nachrichtenobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="018d3-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="018d3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="018d3-105">Permissions</span></span>
<span data-ttu-id="018d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="018d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="018d3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="018d3-108">Permission type</span></span>      | <span data-ttu-id="018d3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="018d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="018d3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="018d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="018d3-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="018d3-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="018d3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="018d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="018d3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="018d3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="018d3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="018d3-114">Application</span></span> | <span data-ttu-id="018d3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="018d3-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="018d3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="018d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="018d3-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="018d3-117">Request headers</span></span>
| <span data-ttu-id="018d3-118">Name</span><span class="sxs-lookup"><span data-stu-id="018d3-118">Name</span></span>       | <span data-ttu-id="018d3-119">Typ</span><span class="sxs-lookup"><span data-stu-id="018d3-119">Type</span></span> | <span data-ttu-id="018d3-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="018d3-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="018d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="018d3-121">Authorization</span></span>  | <span data-ttu-id="018d3-122">string</span><span class="sxs-lookup"><span data-stu-id="018d3-122">string</span></span>  | <span data-ttu-id="018d3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="018d3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="018d3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="018d3-125">Content-Type</span></span> | <span data-ttu-id="018d3-126">string</span><span class="sxs-lookup"><span data-stu-id="018d3-126">string</span></span>  | <span data-ttu-id="018d3-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="018d3-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="018d3-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="018d3-129">Request body</span></span>
<span data-ttu-id="018d3-130">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="018d3-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="018d3-131">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="018d3-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="018d3-132">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="018d3-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="018d3-133">Die folgenden Eigenschaften können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="018d3-133">The following properties can be updated.</span></span>

| <span data-ttu-id="018d3-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="018d3-134">Property</span></span>     | <span data-ttu-id="018d3-135">Typ</span><span class="sxs-lookup"><span data-stu-id="018d3-135">Type</span></span>   |<span data-ttu-id="018d3-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="018d3-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="018d3-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="018d3-137">bccRecipients</span></span>|<span data-ttu-id="018d3-138">Empfänger</span><span class="sxs-lookup"><span data-stu-id="018d3-138">Recipient</span></span>|<span data-ttu-id="018d3-139">Die Bcc:-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="018d3-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="018d3-140">body</span><span class="sxs-lookup"><span data-stu-id="018d3-140">body</span></span>|<span data-ttu-id="018d3-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="018d3-141">ItemBody</span></span>|<span data-ttu-id="018d3-p105">Der Text der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="018d3-p105">The body of the message. Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="018d3-144">categories</span><span class="sxs-lookup"><span data-stu-id="018d3-144">categories</span></span>|<span data-ttu-id="018d3-145">String collection</span><span class="sxs-lookup"><span data-stu-id="018d3-145">String collection</span></span>|<span data-ttu-id="018d3-146">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="018d3-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="018d3-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="018d3-147">ccRecipients</span></span>|<span data-ttu-id="018d3-148">Empfänger-Sammlung</span><span class="sxs-lookup"><span data-stu-id="018d3-148">Recipient collection</span></span>|<span data-ttu-id="018d3-149">Die Cc:-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="018d3-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="018d3-150">from</span><span class="sxs-lookup"><span data-stu-id="018d3-150">from</span></span>|<span data-ttu-id="018d3-151">Empfänger</span><span class="sxs-lookup"><span data-stu-id="018d3-151">Recipient</span></span>|<span data-ttu-id="018d3-152">Der Postfachbesitzer und Absender der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="018d3-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="018d3-153">Muss dem tatsächlich verwendeten Postfach entsprechen.</span><span class="sxs-lookup"><span data-stu-id="018d3-153">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="018d3-154">importance</span><span class="sxs-lookup"><span data-stu-id="018d3-154">importance</span></span>|<span data-ttu-id="018d3-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="018d3-155">String</span></span>|<span data-ttu-id="018d3-p107">Wichtigkeit der Nachricht Mögliche Werte: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="018d3-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="018d3-158">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="018d3-158">inferenceClassification</span></span> | <span data-ttu-id="018d3-159">String</span><span class="sxs-lookup"><span data-stu-id="018d3-159">String</span></span> | <span data-ttu-id="018d3-p108">Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung. Mögliche Werte sind: `focused` oder `other`.</span><span class="sxs-lookup"><span data-stu-id="018d3-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="018d3-162">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="018d3-162">internetMessageId</span></span> |<span data-ttu-id="018d3-163">String</span><span class="sxs-lookup"><span data-stu-id="018d3-163">String</span></span> |<span data-ttu-id="018d3-p109">Die Nachrichten-ID im von [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) angegebenen Format. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="018d3-p109">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="018d3-166">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="018d3-166">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="018d3-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="018d3-167">Boolean</span></span>|<span data-ttu-id="018d3-168">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="018d3-168">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="018d3-169">isRead</span><span class="sxs-lookup"><span data-stu-id="018d3-169">isRead</span></span>|<span data-ttu-id="018d3-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="018d3-170">Boolean</span></span>|<span data-ttu-id="018d3-171">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="018d3-171">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="018d3-172">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="018d3-172">isReadReceiptRequested</span></span>|<span data-ttu-id="018d3-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="018d3-173">Boolean</span></span>|<span data-ttu-id="018d3-174">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="018d3-174">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="018d3-175">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="018d3-175">multiValueExtendedProperties</span></span>|<span data-ttu-id="018d3-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="018d3-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="018d3-177">Die Sammlung der für die Nachricht definierten mehrwertigen erweiterten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="018d3-177">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="018d3-178">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="018d3-178">Nullable.</span></span>|
|<span data-ttu-id="018d3-179">replyTo</span><span class="sxs-lookup"><span data-stu-id="018d3-179">replyTo</span></span>|<span data-ttu-id="018d3-180">Empfänger-Sammlung</span><span class="sxs-lookup"><span data-stu-id="018d3-180">Recipient collection</span></span>|<span data-ttu-id="018d3-181">Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="018d3-181">The email addresses to use when replying.</span></span> <span data-ttu-id="018d3-182">Kann nur aktualisiert werden, wenn isDraft = True.</span><span class="sxs-lookup"><span data-stu-id="018d3-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="018d3-183">sender</span><span class="sxs-lookup"><span data-stu-id="018d3-183">sender</span></span>|<span data-ttu-id="018d3-184">Empfänger</span><span class="sxs-lookup"><span data-stu-id="018d3-184">Recipient</span></span>|<span data-ttu-id="018d3-185">Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.</span><span class="sxs-lookup"><span data-stu-id="018d3-185">The account that is actually used to generate the message.</span></span> <span data-ttu-id="018d3-186">Kann beim Senden einer Nachricht aus einem [freigegebenen Postfach](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes) oder beim Senden einer Nachricht als[Stellvertretung](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="018d3-186">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="018d3-187">Der Wert muss auf jeden Fall dem tatsächlich verwendeten Postfach entsprechen.</span><span class="sxs-lookup"><span data-stu-id="018d3-187">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="018d3-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="018d3-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="018d3-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="018d3-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="018d3-190">Die Sammlung der für die Nachricht definierten einwertigen erweiterten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="018d3-190">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="018d3-191">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="018d3-191">Nullable.</span></span>|
|<span data-ttu-id="018d3-192">subject</span><span class="sxs-lookup"><span data-stu-id="018d3-192">subject</span></span>|<span data-ttu-id="018d3-193">String</span><span class="sxs-lookup"><span data-stu-id="018d3-193">String</span></span>|<span data-ttu-id="018d3-p114">Der Betreff der Nachricht. Kann nur aktualisiert werden, wenn IsDraft = True.</span><span class="sxs-lookup"><span data-stu-id="018d3-p114">The subject of the message. Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="018d3-196">toRecipients</span><span class="sxs-lookup"><span data-stu-id="018d3-196">toRecipients</span></span>|<span data-ttu-id="018d3-197">Empfänger-Sammlung</span><span class="sxs-lookup"><span data-stu-id="018d3-197">Recipient collection</span></span>|<span data-ttu-id="018d3-198">Die An:-Empfänger der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="018d3-198">The To recipients for the message.</span></span> |

<span data-ttu-id="018d3-199">Da die **message**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **message**-Instanzen.</span><span class="sxs-lookup"><span data-stu-id="018d3-199">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="018d3-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="018d3-200">Response</span></span>

<span data-ttu-id="018d3-201">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [message](../resources/message.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="018d3-201">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="018d3-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="018d3-202">Example</span></span>
##### <a name="request"></a><span data-ttu-id="018d3-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="018d3-203">Request</span></span>
<span data-ttu-id="018d3-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="018d3-204">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="018d3-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="018d3-205">Response</span></span>
<span data-ttu-id="018d3-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="018d3-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="018d3-209">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="018d3-209">See also</span></span>

- [<span data-ttu-id="018d3-210">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="018d3-210">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="018d3-211">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="018d3-211">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="018d3-212">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="018d3-212">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
