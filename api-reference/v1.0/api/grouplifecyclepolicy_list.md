# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="38cb1-101">Auflisten von groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="38cb1-101">List groupLifecyclePolicies</span></span>

<span data-ttu-id="38cb1-102">Listet alle [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="38cb1-102">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38cb1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38cb1-103">Permissions</span></span>

<span data-ttu-id="38cb1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38cb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="38cb1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38cb1-106">Permission type</span></span>      | <span data-ttu-id="38cb1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38cb1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38cb1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38cb1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="38cb1-109">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38cb1-109">Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="38cb1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38cb1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38cb1-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38cb1-111">Not supported.</span></span>    |
|<span data-ttu-id="38cb1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38cb1-112">Application</span></span> | <span data-ttu-id="38cb1-113">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38cb1-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38cb1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38cb1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="38cb1-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="38cb1-115">Optional query parameters</span></span>
<span data-ttu-id="38cb1-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="38cb1-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38cb1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38cb1-117">Request headers</span></span>
| <span data-ttu-id="38cb1-118">Name</span><span class="sxs-lookup"><span data-stu-id="38cb1-118">Name</span></span> | <span data-ttu-id="38cb1-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38cb1-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="38cb1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="38cb1-120">Authorization</span></span> | <span data-ttu-id="38cb1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38cb1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38cb1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38cb1-123">Request body</span></span>
<span data-ttu-id="38cb1-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="38cb1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38cb1-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="38cb1-125">Response</span></span>

<span data-ttu-id="38cb1-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="38cb1-126">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38cb1-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38cb1-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="38cb1-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38cb1-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="38cb1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="38cb1-129">Response</span></span>

<span data-ttu-id="38cb1-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38cb1-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 223

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 100,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->