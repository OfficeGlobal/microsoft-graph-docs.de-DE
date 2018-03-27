# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="51104-101">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="51104-101">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="51104-102">Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu.</span><span class="sxs-lookup"><span data-stu-id="51104-102">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="51104-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="51104-103">Permissions</span></span>

<span data-ttu-id="51104-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="51104-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="51104-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51104-106">Permission type</span></span>      | <span data-ttu-id="51104-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51104-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51104-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51104-108">Delegated (work or school account)</span></span> | <span data-ttu-id="51104-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51104-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="51104-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51104-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51104-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51104-111">Not supported.</span></span>    |
|<span data-ttu-id="51104-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51104-112">Application</span></span> | <span data-ttu-id="51104-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51104-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51104-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51104-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="51104-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51104-115">Request headers</span></span>

| <span data-ttu-id="51104-116">Name</span><span class="sxs-lookup"><span data-stu-id="51104-116">Name</span></span> | <span data-ttu-id="51104-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51104-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="51104-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="51104-118">Authorization</span></span> | <span data-ttu-id="51104-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="51104-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51104-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51104-121">Content-Type</span></span>  | <span data-ttu-id="51104-122">application/json</span><span class="sxs-lookup"><span data-stu-id="51104-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="51104-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51104-123">Request body</span></span>
<span data-ttu-id="51104-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="51104-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="51104-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="51104-125">Parameter</span></span> | <span data-ttu-id="51104-126">Typ</span><span class="sxs-lookup"><span data-stu-id="51104-126">Type</span></span> | <span data-ttu-id="51104-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51104-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="51104-128">groupId</span><span class="sxs-lookup"><span data-stu-id="51104-128">groupId</span></span>|<span data-ttu-id="51104-129">Guid</span><span class="sxs-lookup"><span data-stu-id="51104-129">Guid</span></span>| <span data-ttu-id="51104-130">Die ID der Gruppe, der die Richtlinie hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="51104-130">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="51104-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="51104-131">Response</span></span>

<span data-ttu-id="51104-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51104-132">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="51104-133">Wenn die Gruppe zur Richtlinie hinzugefügt wird, wird der Wert **true** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51104-133">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="51104-134">Andernfalls wird der Wert **false** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51104-134">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="51104-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51104-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="51104-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51104-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="51104-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="51104-137">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->