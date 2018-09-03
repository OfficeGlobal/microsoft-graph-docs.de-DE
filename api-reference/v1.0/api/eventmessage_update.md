# <a name="update-eventmessage"></a><span data-ttu-id="01042-101">eventMessage aktualisieren</span><span class="sxs-lookup"><span data-stu-id="01042-101">Update eventMessage</span></span>

<span data-ttu-id="01042-102">Dient zum Aktualisieren der Eigenschaften des [eventMessage](../resources/eventmessage.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="01042-102">Update the properties of an [eventMessage](../resources/eventmessage.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="01042-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="01042-103">Permissions</span></span>
<span data-ttu-id="01042-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01042-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01042-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="01042-106">Permission type</span></span>      | <span data-ttu-id="01042-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="01042-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01042-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="01042-108">Delegated (work or school account)</span></span> | <span data-ttu-id="01042-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01042-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="01042-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="01042-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01042-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01042-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="01042-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="01042-112">Application</span></span> | <span data-ttu-id="01042-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01042-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="01042-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="01042-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="01042-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="01042-115">Request headers</span></span>
| <span data-ttu-id="01042-116">Name</span><span class="sxs-lookup"><span data-stu-id="01042-116">Name</span></span>       | <span data-ttu-id="01042-117">Typ</span><span class="sxs-lookup"><span data-stu-id="01042-117">Type</span></span> | <span data-ttu-id="01042-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01042-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01042-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="01042-119">Authorization</span></span>  | <span data-ttu-id="01042-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01042-120">string</span></span>  | <span data-ttu-id="01042-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="01042-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01042-123">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="01042-123">Content-Type</span></span> | <span data-ttu-id="01042-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01042-124">string</span></span>  | <span data-ttu-id="01042-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="01042-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="01042-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="01042-127">Request body</span></span>
<span data-ttu-id="01042-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben. Schreibbare/Aktualisierbare Eigenschaften:</span><span class="sxs-lookup"><span data-stu-id="01042-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="01042-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="01042-132">Property</span></span>     | <span data-ttu-id="01042-133">Typ</span><span class="sxs-lookup"><span data-stu-id="01042-133">Type</span></span>   |<span data-ttu-id="01042-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01042-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01042-135">Kategorien</span><span class="sxs-lookup"><span data-stu-id="01042-135">categories</span></span>|<span data-ttu-id="01042-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01042-136">String</span></span>|<span data-ttu-id="01042-137">Die Kategorien, die mit der Nachricht verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="01042-137">The categories associated with the message.</span></span>|
|<span data-ttu-id="01042-138">Wichtigkeit</span><span class="sxs-lookup"><span data-stu-id="01042-138">importance</span></span>|<span data-ttu-id="01042-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="01042-139">String</span></span>|<span data-ttu-id="01042-140">Die Wichtigkeit der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="01042-140">The importance of the message: , , .</span></span> <span data-ttu-id="01042-141">Die möglichen Werte sind: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="01042-141">The possible values are `Low`, `Normal`, `High`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="01042-142">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="01042-142">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="01042-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="01042-143">Boolean</span></span>|<span data-ttu-id="01042-144">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="01042-144">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="01042-145">isRead</span><span class="sxs-lookup"><span data-stu-id="01042-145">isRead</span></span>|<span data-ttu-id="01042-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="01042-146">Boolean</span></span>|<span data-ttu-id="01042-147">Gibt an, ob die Nachricht gelesen wurde.</span><span class="sxs-lookup"><span data-stu-id="01042-147">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="01042-148">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="01042-148">isReadReceiptRequested</span></span>|<span data-ttu-id="01042-149">Boolesch</span><span class="sxs-lookup"><span data-stu-id="01042-149">Boolean</span></span>|<span data-ttu-id="01042-150">Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="01042-150">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="01042-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="01042-151">Response</span></span>

<span data-ttu-id="01042-152">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [eventMessage](../resources/eventmessage.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01042-152">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01042-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="01042-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01042-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="01042-154">Request</span></span>
<span data-ttu-id="01042-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="01042-155">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="01042-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="01042-156">Response</span></span>
<span data-ttu-id="01042-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01042-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
