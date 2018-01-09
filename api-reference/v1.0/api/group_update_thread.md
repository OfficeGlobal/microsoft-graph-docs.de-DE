# <a name="update-conversation-thread"></a><span data-ttu-id="28373-101">Unterhaltungsthread aktualisieren</span><span class="sxs-lookup"><span data-stu-id="28373-101">Update conversation thread</span></span>
<span data-ttu-id="28373-102">Aktualisieren eines [Thread](../resources/conversationthread.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="28373-102">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="28373-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="28373-103">Permissions</span></span>
<span data-ttu-id="28373-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="28373-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="28373-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28373-106">Permission type</span></span>      | <span data-ttu-id="28373-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28373-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28373-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28373-108">Delegated (work or school account)</span></span> | <span data-ttu-id="28373-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28373-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="28373-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28373-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28373-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28373-111">Not supported.</span></span>    |
|<span data-ttu-id="28373-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28373-112">Application</span></span> | <span data-ttu-id="28373-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28373-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28373-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28373-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="28373-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28373-115">Request headers</span></span>
| <span data-ttu-id="28373-116">Name</span><span class="sxs-lookup"><span data-stu-id="28373-116">Name</span></span>       | <span data-ttu-id="28373-117">Typ</span><span class="sxs-lookup"><span data-stu-id="28373-117">Type</span></span> | <span data-ttu-id="28373-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28373-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="28373-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="28373-119">Authorization</span></span>  | <span data-ttu-id="28373-120">string</span><span class="sxs-lookup"><span data-stu-id="28373-120">string</span></span>  | <span data-ttu-id="28373-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="28373-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28373-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28373-123">Request body</span></span>
<span data-ttu-id="28373-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="28373-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="28373-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="28373-127">Response</span></span>
<span data-ttu-id="28373-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28373-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="28373-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28373-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="28373-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28373-130">Request</span></span>
<span data-ttu-id="28373-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28373-131">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="28373-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="28373-132">Response</span></span>
<span data-ttu-id="28373-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="28373-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->