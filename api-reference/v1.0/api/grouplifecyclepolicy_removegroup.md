# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="eb7a7-101">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="eb7a7-101">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="eb7a7-102">Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="eb7a7-102">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb7a7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eb7a7-103">Permissions</span></span>

<span data-ttu-id="eb7a7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb7a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb7a7-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb7a7-106">Permission type</span></span>      | <span data-ttu-id="eb7a7-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb7a7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb7a7-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb7a7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="eb7a7-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb7a7-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb7a7-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb7a7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb7a7-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb7a7-111">Not supported.</span></span>    |
|<span data-ttu-id="eb7a7-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb7a7-112">Application</span></span> | <span data-ttu-id="eb7a7-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb7a7-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb7a7-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb7a7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="eb7a7-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb7a7-115">Request headers</span></span>

| <span data-ttu-id="eb7a7-116">Name</span><span class="sxs-lookup"><span data-stu-id="eb7a7-116">Name</span></span> | <span data-ttu-id="eb7a7-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb7a7-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="eb7a7-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb7a7-118">Authorization</span></span> | <span data-ttu-id="eb7a7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eb7a7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb7a7-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb7a7-121">Content-Type</span></span>  | <span data-ttu-id="eb7a7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="eb7a7-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb7a7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb7a7-123">Request body</span></span>
<span data-ttu-id="eb7a7-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="eb7a7-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eb7a7-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="eb7a7-125">Parameter</span></span> | <span data-ttu-id="eb7a7-126">Typ</span><span class="sxs-lookup"><span data-stu-id="eb7a7-126">Type</span></span> | <span data-ttu-id="eb7a7-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb7a7-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="eb7a7-128">groupId</span><span class="sxs-lookup"><span data-stu-id="eb7a7-128">groupId</span></span>|<span data-ttu-id="eb7a7-129">Guid</span><span class="sxs-lookup"><span data-stu-id="eb7a7-129">Guid</span></span>| <span data-ttu-id="eb7a7-130">Die ID der Gruppe, die aus der Richtlinie entfernt werden soll.</span><span class="sxs-lookup"><span data-stu-id="eb7a7-130">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="eb7a7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb7a7-131">Response</span></span>

<span data-ttu-id="eb7a7-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb7a7-132">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="eb7a7-133">Wenn die Gruppe aus der Richtlinie entfernt wird, wird der Wert **true** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb7a7-133">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="eb7a7-134">Andernfalls wird der Wert **false** im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb7a7-134">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="eb7a7-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb7a7-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eb7a7-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb7a7-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="eb7a7-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb7a7-137">Response</span></span>
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
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->