# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="22049-101">Erstellen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="22049-101">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="22049-102">Erstellt ein neues [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="22049-102">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="22049-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="22049-103">Permissions</span></span>

<span data-ttu-id="22049-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="22049-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="22049-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22049-106">Permission type</span></span>      | <span data-ttu-id="22049-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22049-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22049-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22049-108">Delegated (work or school account)</span></span> | <span data-ttu-id="22049-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22049-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="22049-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22049-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22049-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22049-111">Not supported.</span></span>    |
|<span data-ttu-id="22049-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22049-112">Application</span></span> | <span data-ttu-id="22049-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22049-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22049-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22049-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="22049-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22049-115">Request headers</span></span>

| <span data-ttu-id="22049-116">Name</span><span class="sxs-lookup"><span data-stu-id="22049-116">Name</span></span> | <span data-ttu-id="22049-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="22049-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="22049-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="22049-118">Authorization</span></span> | <span data-ttu-id="22049-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="22049-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="22049-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="22049-121">Content-Type</span></span>  | <span data-ttu-id="22049-122">application/json</span><span class="sxs-lookup"><span data-stu-id="22049-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="22049-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22049-123">Request body</span></span>
<span data-ttu-id="22049-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="22049-124">In the request body, supply a JSON representation of [plannerPlan](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="22049-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="22049-125">Response</span></span>

<span data-ttu-id="22049-126">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `201 Created` und ein [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="22049-126">If successful, this method returns a `201 Created` response code and [profilePhoto](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22049-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22049-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="22049-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22049-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="22049-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="22049-129">In the request body, supply a JSON representation of [plannerPlan](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="22049-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="22049-130">Response</span></span>

<span data-ttu-id="22049-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22049-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->