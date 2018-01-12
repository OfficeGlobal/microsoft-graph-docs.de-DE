# <a name="update-eventmessage"></a><span data-ttu-id="b7c5b-101">eventMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b7c5b-101">Update eventmessage</span></span>

<span data-ttu-id="b7c5b-102">Dient zum Aktualisieren der Eigenschaften des [eventMessage](../resources/eventmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-102">Update the properties of eventmessage object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7c5b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b7c5b-103">Permissions</span></span>
<span data-ttu-id="b7c5b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b7c5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b7c5b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b7c5b-106">Permission type</span></span>      | <span data-ttu-id="b7c5b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b7c5b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7c5b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b7c5b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b7c5b-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7c5b-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b7c5b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b7c5b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7c5b-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7c5b-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b7c5b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b7c5b-112">Application</span></span> | <span data-ttu-id="b7c5b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7c5b-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7c5b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7c5b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b7c5b-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b7c5b-115">Request headers</span></span>
| <span data-ttu-id="b7c5b-116">Name</span><span class="sxs-lookup"><span data-stu-id="b7c5b-116">Name</span></span>       | <span data-ttu-id="b7c5b-117">Typ</span><span class="sxs-lookup"><span data-stu-id="b7c5b-117">Type</span></span> | <span data-ttu-id="b7c5b-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7c5b-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b7c5b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7c5b-119">Authorization</span></span>  | <span data-ttu-id="b7c5b-120">string</span><span class="sxs-lookup"><span data-stu-id="b7c5b-120">string</span></span>  | <span data-ttu-id="b7c5b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7c5b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7c5b-123">Content-Type</span></span> | <span data-ttu-id="b7c5b-124">string</span><span class="sxs-lookup"><span data-stu-id="b7c5b-124">string</span></span>  | <span data-ttu-id="b7c5b-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="b7c5b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b7c5b-127">Request body</span></span>
<span data-ttu-id="b7c5b-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="b7c5b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="b7c5b-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b7c5b-132">Property</span></span>     | <span data-ttu-id="b7c5b-133">Typ</span><span class="sxs-lookup"><span data-stu-id="b7c5b-133">Type</span></span>   |<span data-ttu-id="b7c5b-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7c5b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7c5b-135">categories</span><span class="sxs-lookup"><span data-stu-id="b7c5b-135">categories</span></span>|<span data-ttu-id="b7c5b-136">String</span><span class="sxs-lookup"><span data-stu-id="b7c5b-136">String</span></span>|<span data-ttu-id="b7c5b-137">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-137">The categories associated with the message.</span></span>|
|<span data-ttu-id="b7c5b-138">importance</span><span class="sxs-lookup"><span data-stu-id="b7c5b-138">importance</span></span>|<span data-ttu-id="b7c5b-139">String</span><span class="sxs-lookup"><span data-stu-id="b7c5b-139">String</span></span>|<span data-ttu-id="b7c5b-p105">Wichtigkeit der Nachricht Mögliche Werte: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="b7c5b-142">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b7c5b-142">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="b7c5b-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7c5b-143">Boolean</span></span>|<span data-ttu-id="b7c5b-144">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-144">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="b7c5b-145">isRead</span><span class="sxs-lookup"><span data-stu-id="b7c5b-145">isRead</span></span>|<span data-ttu-id="b7c5b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7c5b-146">Boolean</span></span>|<span data-ttu-id="b7c5b-147">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-147">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="b7c5b-148">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="b7c5b-148">isReadReceiptRequested</span></span>|<span data-ttu-id="b7c5b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7c5b-149">Boolean</span></span>|<span data-ttu-id="b7c5b-150">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-150">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="b7c5b-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7c5b-151">Response</span></span>

<span data-ttu-id="b7c5b-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [eventMessage](../resources/eventmessage.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-152">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7c5b-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b7c5b-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7c5b-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7c5b-154">Request</span></span>
<span data-ttu-id="b7c5b-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="b7c5b-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7c5b-156">Response</span></span>
<span data-ttu-id="b7c5b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7c5b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
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
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
