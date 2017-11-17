# <a name="get-entity"></a><span data-ttu-id="cbd57-101">Entität abrufen</span><span class="sxs-lookup"><span data-stu-id="cbd57-101">Get entity</span></span>

<span data-ttu-id="cbd57-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Entitätsobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="cbd57-102">Retrieve the properties and relationships of entity object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cbd57-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cbd57-103">Permissions</span></span>
<span data-ttu-id="cbd57-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cbd57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cbd57-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cbd57-106">Permission type</span></span>      | <span data-ttu-id="cbd57-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cbd57-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbd57-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cbd57-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cbd57-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbd57-109">Not supported.</span></span>    |
|<span data-ttu-id="cbd57-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cbd57-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbd57-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbd57-111">Not supported.</span></span>    |
|<span data-ttu-id="cbd57-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cbd57-112">Application</span></span> | <span data-ttu-id="cbd57-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbd57-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbd57-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbd57-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http

```
## <a name="optional-query-parameters"></a><span data-ttu-id="cbd57-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cbd57-115">Optional query parameters</span></span>
<span data-ttu-id="cbd57-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cbd57-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cbd57-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cbd57-117">Request headers</span></span>
| <span data-ttu-id="cbd57-118">Name</span><span class="sxs-lookup"><span data-stu-id="cbd57-118">Name</span></span>       | <span data-ttu-id="cbd57-119">Typ</span><span class="sxs-lookup"><span data-stu-id="cbd57-119">Type</span></span> | <span data-ttu-id="cbd57-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbd57-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cbd57-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbd57-121">Authorization</span></span>  | <span data-ttu-id="cbd57-122">string</span><span class="sxs-lookup"><span data-stu-id="cbd57-122">string</span></span>  | <span data-ttu-id="cbd57-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cbd57-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbd57-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cbd57-125">Request body</span></span>
<span data-ttu-id="cbd57-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cbd57-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbd57-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbd57-127">Response</span></span>

<span data-ttu-id="cbd57-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [entity](../resources/entity.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbd57-128">If successful, this method returns a `200 OK` response code and [entity](../resources/entity.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cbd57-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cbd57-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbd57-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbd57-130">Request</span></span>
<span data-ttu-id="cbd57-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cbd57-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_entity"
}-->
```http

```
##### <a name="response"></a><span data-ttu-id="cbd57-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbd57-132">Response</span></span>
<span data-ttu-id="cbd57-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbd57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get entity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
