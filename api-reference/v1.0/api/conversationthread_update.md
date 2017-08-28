# <a name="update-conversationthread"></a><span data-ttu-id="3197f-101">conversationThread aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3197f-101">Update conversationthread</span></span>

<span data-ttu-id="3197f-102">Mit dieser API können Sie Threads sperren oder entsperren und so steuern, ob weiterhin in ihnen gepostet werden darf.</span><span class="sxs-lookup"><span data-stu-id="3197f-102">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="3197f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3197f-103">Permissions</span></span>
<span data-ttu-id="3197f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3197f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3197f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3197f-106">Permission type</span></span>      | <span data-ttu-id="3197f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3197f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3197f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3197f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3197f-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3197f-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3197f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3197f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3197f-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3197f-111">Not supported.</span></span>    |
|<span data-ttu-id="3197f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3197f-112">Application</span></span> | <span data-ttu-id="3197f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3197f-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3197f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3197f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3197f-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3197f-115">Request headers</span></span>
| <span data-ttu-id="3197f-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3197f-116">Header</span></span>       | <span data-ttu-id="3197f-117">Wert</span><span class="sxs-lookup"><span data-stu-id="3197f-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3197f-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="3197f-118">Authorization</span></span>  | <span data-ttu-id="3197f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3197f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3197f-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3197f-121">Content-Type</span></span>  | <span data-ttu-id="3197f-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="3197f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3197f-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3197f-124">Request body</span></span>
<span data-ttu-id="3197f-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="3197f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3197f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3197f-128">Property</span></span>     | <span data-ttu-id="3197f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3197f-129">Type</span></span>   |<span data-ttu-id="3197f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3197f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3197f-131">isLocked</span><span class="sxs-lookup"><span data-stu-id="3197f-131">isLocked</span></span>|<span data-ttu-id="3197f-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="3197f-132">Boolean</span></span>|<span data-ttu-id="3197f-p105">Zeigt an, ob der Thread gesperrt ist. Mit `true` werden Beiträge verhindert.</span><span class="sxs-lookup"><span data-stu-id="3197f-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="3197f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3197f-135">Response</span></span>

<span data-ttu-id="3197f-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3197f-136">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3197f-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3197f-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3197f-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3197f-138">Request</span></span>
<span data-ttu-id="3197f-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3197f-139">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3197f-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="3197f-140">Response</span></span>
<span data-ttu-id="3197f-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3197f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
