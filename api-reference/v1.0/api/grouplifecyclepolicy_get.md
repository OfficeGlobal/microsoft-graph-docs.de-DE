# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="262b4-101">Abrufen von groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="262b4-101">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="262b4-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md)-Objekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="262b4-102">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="262b4-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="262b4-103">Permissions</span></span>

<span data-ttu-id="262b4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="262b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="262b4-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="262b4-106">Permission type</span></span>      | <span data-ttu-id="262b4-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="262b4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="262b4-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="262b4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="262b4-109">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="262b4-109">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="262b4-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="262b4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="262b4-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="262b4-111">Not supported.</span></span>    |
|<span data-ttu-id="262b4-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="262b4-112">Application</span></span> | <span data-ttu-id="262b4-113">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="262b4-113">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="262b4-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="262b4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="262b4-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="262b4-115">Optional query parameters</span></span>
<span data-ttu-id="262b4-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="262b4-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="262b4-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="262b4-117">Request headers</span></span>
| <span data-ttu-id="262b4-118">Name</span><span class="sxs-lookup"><span data-stu-id="262b4-118">Name</span></span> | <span data-ttu-id="262b4-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="262b4-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="262b4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="262b4-120">Authorization</span></span> | <span data-ttu-id="262b4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="262b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="262b4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="262b4-123">Request body</span></span>
<span data-ttu-id="262b4-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="262b4-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="262b4-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="262b4-125">Response</span></span>
<span data-ttu-id="262b4-126">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `200 OK` und ein [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="262b4-126">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="262b4-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="262b4-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="262b4-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="262b4-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="262b4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="262b4-129">Response</span></span>

<span data-ttu-id="262b4-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="262b4-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->