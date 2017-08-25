# <a name="update-conversationthread"></a><span data-ttu-id="0e38d-101">conversationThread aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0e38d-101">Update conversationthread</span></span>

<span data-ttu-id="0e38d-102">Mit dieser API können Sie Threads sperren oder entsperren und so steuern, ob weiterhin in ihnen gepostet werden darf.</span><span class="sxs-lookup"><span data-stu-id="0e38d-102">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e38d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0e38d-103">Permissions</span></span>
<span data-ttu-id="0e38d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e38d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0e38d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e38d-106">Permission type</span></span>      | <span data-ttu-id="0e38d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e38d-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="0e38d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e38d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0e38d-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e38d-109">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="0e38d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e38d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e38d-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e38d-111">Not supported.</span></span>    | 
|<span data-ttu-id="0e38d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e38d-112">Application</span></span> | <span data-ttu-id="0e38d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e38d-113">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0e38d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e38d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0e38d-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e38d-115">Request headers</span></span>
| <span data-ttu-id="0e38d-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0e38d-116">Header</span></span>       | <span data-ttu-id="0e38d-117">Wert</span><span class="sxs-lookup"><span data-stu-id="0e38d-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e38d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e38d-118">Authorization</span></span>  | <span data-ttu-id="0e38d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e38d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0e38d-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e38d-121">Content-Type</span></span>  | <span data-ttu-id="0e38d-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="0e38d-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e38d-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e38d-124">Request body</span></span>
<span data-ttu-id="0e38d-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="0e38d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e38d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e38d-128">Property</span></span>     | <span data-ttu-id="0e38d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0e38d-129">Type</span></span>   |<span data-ttu-id="0e38d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e38d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e38d-131">isLocked</span><span class="sxs-lookup"><span data-stu-id="0e38d-131">isLocked</span></span>|<span data-ttu-id="0e38d-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e38d-132">Boolean</span></span>|<span data-ttu-id="0e38d-p105">Zeigt an, ob der Thread gesperrt ist. Mit `true` werden Beiträge verhindert.</span><span class="sxs-lookup"><span data-stu-id="0e38d-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="0e38d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e38d-135">Response</span></span>

<span data-ttu-id="0e38d-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e38d-136">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e38d-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e38d-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e38d-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e38d-138">Request</span></span>
<span data-ttu-id="0e38d-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e38d-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
##### <a name="response"></a><span data-ttu-id="0e38d-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e38d-140">Response</span></span>
<span data-ttu-id="0e38d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e38d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "isLocked": true 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
