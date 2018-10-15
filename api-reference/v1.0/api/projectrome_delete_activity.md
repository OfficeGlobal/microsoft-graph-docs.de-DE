# <a name="delete-an-activity"></a><span data-ttu-id="87c6d-101">Aktivität löschen</span><span class="sxs-lookup"><span data-stu-id="87c6d-101">Delete an activity</span></span>

<span data-ttu-id="87c6d-102">Löschen einer vorhandenen Benutzeraktivität für Ihre App.</span><span class="sxs-lookup"><span data-stu-id="87c6d-102">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="87c6d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87c6d-103">Permissions</span></span>

<span data-ttu-id="87c6d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87c6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="87c6d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87c6d-106">Permission type</span></span>      | <span data-ttu-id="87c6d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87c6d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87c6d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87c6d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="87c6d-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="87c6d-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="87c6d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87c6d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87c6d-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="87c6d-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="87c6d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87c6d-112">Application</span></span> | <span data-ttu-id="87c6d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87c6d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87c6d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c6d-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="87c6d-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87c6d-115">Request headers</span></span>

|<span data-ttu-id="87c6d-116">Name</span><span class="sxs-lookup"><span data-stu-id="87c6d-116">Name</span></span> | <span data-ttu-id="87c6d-117">Typ</span><span class="sxs-lookup"><span data-stu-id="87c6d-117">Type</span></span> | <span data-ttu-id="87c6d-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87c6d-118">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="87c6d-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="87c6d-119">Authorization</span></span> | <span data-ttu-id="87c6d-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87c6d-120">string</span></span> | <span data-ttu-id="87c6d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87c6d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87c6d-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87c6d-123">Request body</span></span>

<span data-ttu-id="87c6d-124">Kein Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="87c6d-124">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="87c6d-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c6d-125">Response</span></span>

<span data-ttu-id="87c6d-126">Wenn die Methode erfolgreich verläuft, gibt diese den `204 No Content` Antwortcode zurück, sobald die Aktivität gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="87c6d-126">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="87c6d-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87c6d-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="87c6d-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c6d-128">Request</span></span>

<span data-ttu-id="87c6d-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87c6d-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="87c6d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c6d-130">Response</span></span>

<span data-ttu-id="87c6d-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87c6d-131">Here is an example of the response.</span></span>

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
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->