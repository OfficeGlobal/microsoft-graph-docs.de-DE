# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="176b7-101">Löschen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="176b7-101">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="176b7-102">Löscht [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="176b7-102">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="176b7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="176b7-103">Permissions</span></span>

<span data-ttu-id="176b7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="176b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="176b7-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="176b7-106">Permission type</span></span>      | <span data-ttu-id="176b7-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="176b7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="176b7-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="176b7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="176b7-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="176b7-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="176b7-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="176b7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="176b7-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="176b7-111">Not supported.</span></span>    |
|<span data-ttu-id="176b7-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="176b7-112">Application</span></span> | <span data-ttu-id="176b7-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="176b7-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="176b7-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="176b7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="176b7-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="176b7-115">Request headers</span></span>

| <span data-ttu-id="176b7-116">Name</span><span class="sxs-lookup"><span data-stu-id="176b7-116">Name</span></span> | <span data-ttu-id="176b7-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="176b7-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="176b7-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="176b7-118">Authorization</span></span> | <span data-ttu-id="176b7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="176b7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="176b7-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="176b7-121">Content-Type</span></span>  | <span data-ttu-id="176b7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="176b7-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="176b7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="176b7-123">Request body</span></span>
<span data-ttu-id="176b7-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="176b7-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="176b7-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="176b7-125">Response</span></span>

<span data-ttu-id="176b7-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="176b7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="176b7-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="176b7-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="176b7-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="176b7-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="176b7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="176b7-130">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->