# <a name="get-directoryroletemplate"></a><span data-ttu-id="bf440-101">directoryRoleTemplate abrufen</span><span class="sxs-lookup"><span data-stu-id="bf440-101">Get directoryRoleTemplate</span></span>

<span data-ttu-id="bf440-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Objekts des Typs „directoryroletemplate“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="bf440-102">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf440-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bf440-103">Permissions</span></span>
<span data-ttu-id="bf440-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bf440-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bf440-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bf440-106">Permission type</span></span>      | <span data-ttu-id="bf440-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bf440-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf440-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bf440-108">Delegated (work or school account)</span></span> | <span data-ttu-id="bf440-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf440-109">Not supported.</span></span>    |
|<span data-ttu-id="bf440-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bf440-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf440-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf440-111">Not supported.</span></span>    |
|<span data-ttu-id="bf440-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bf440-112">Application</span></span> | <span data-ttu-id="bf440-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf440-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf440-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf440-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bf440-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bf440-115">Optional query parameters</span></span>
<span data-ttu-id="bf440-116">Die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="bf440-116">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf440-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bf440-117">Request headers</span></span>
| <span data-ttu-id="bf440-118">Name</span><span class="sxs-lookup"><span data-stu-id="bf440-118">Name</span></span>       | <span data-ttu-id="bf440-119">Typ</span><span class="sxs-lookup"><span data-stu-id="bf440-119">Type</span></span> | <span data-ttu-id="bf440-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf440-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bf440-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf440-121">Authorization</span></span>  | <span data-ttu-id="bf440-122">string</span><span class="sxs-lookup"><span data-stu-id="bf440-122">string</span></span>  | <span data-ttu-id="bf440-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bf440-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf440-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bf440-125">Request body</span></span>
<span data-ttu-id="bf440-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bf440-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf440-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf440-127">Response</span></span>

<span data-ttu-id="bf440-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryRoleTemplate](../resources/directoryroletemplate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf440-128">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bf440-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bf440-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf440-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf440-130">Request</span></span>
<span data-ttu-id="bf440-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bf440-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="bf440-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf440-132">Response</span></span>
<span data-ttu-id="bf440-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf440-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
