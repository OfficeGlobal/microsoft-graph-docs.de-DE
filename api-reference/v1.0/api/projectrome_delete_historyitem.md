# <a name="delete-a-historyitem"></a><span data-ttu-id="42091-101">Löschen eines historyItem</span><span class="sxs-lookup"><span data-stu-id="42091-101">Delete a historyItem</span></span>

<span data-ttu-id="42091-102">Löschen eines vorhandenen Verlaufselements für eine vorhandene Benutzer-Aktivität.</span><span class="sxs-lookup"><span data-stu-id="42091-102">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="42091-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="42091-103">Permissions</span></span>

<span data-ttu-id="42091-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="42091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="42091-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="42091-106">Permission type</span></span>      | <span data-ttu-id="42091-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="42091-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42091-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="42091-108">Delegated (work or school account)</span></span> | <span data-ttu-id="42091-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="42091-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="42091-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="42091-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42091-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="42091-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="42091-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="42091-112">Application</span></span> | <span data-ttu-id="42091-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42091-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42091-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="42091-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="42091-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="42091-115">Request headers</span></span>

|<span data-ttu-id="42091-116">Name</span><span class="sxs-lookup"><span data-stu-id="42091-116">Name</span></span> | <span data-ttu-id="42091-117">Typ</span><span class="sxs-lookup"><span data-stu-id="42091-117">Type</span></span> | <span data-ttu-id="42091-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42091-118">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="42091-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="42091-119">Authorization</span></span> | <span data-ttu-id="42091-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42091-120">string</span></span> | <span data-ttu-id="42091-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="42091-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42091-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="42091-123">Request body</span></span>

<span data-ttu-id="42091-124">Kein Anfragetext.</span><span class="sxs-lookup"><span data-stu-id="42091-124">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="42091-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="42091-125">Response</span></span>

<span data-ttu-id="42091-126">Wenn der Vorgang erfolgreich war, gibt dieses VErfahren den `204 No Content` Antwortcode, wenn das Verlaufselement gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="42091-126">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="42091-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="42091-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="42091-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="42091-128">Request</span></span>

<span data-ttu-id="42091-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="42091-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```

##### <a name="response"></a><span data-ttu-id="42091-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="42091-130">Response</span></span>

<span data-ttu-id="42091-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="42091-131">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->