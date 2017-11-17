# <a name="list-directoryroletemplates"></a><span data-ttu-id="a5fc6-101">directoryRoleTemplates auflisten</span><span class="sxs-lookup"><span data-stu-id="a5fc6-101">List directoryRoleTemplates</span></span>

<span data-ttu-id="a5fc6-102">Mit dieser API können Sie eine Liste von Objekten des Typs „directoryRoleTemplate“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="a5fc6-102">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5fc6-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a5fc6-103">Permissions</span></span>
<span data-ttu-id="a5fc6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5fc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="a5fc6-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5fc6-106">Permission type</span></span>      | <span data-ttu-id="a5fc6-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5fc6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5fc6-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5fc6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a5fc6-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5fc6-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5fc6-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5fc6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5fc6-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5fc6-111">Not supported.</span></span>    |
|<span data-ttu-id="a5fc6-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5fc6-112">Application</span></span> | <span data-ttu-id="a5fc6-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5fc6-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5fc6-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5fc6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a5fc6-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a5fc6-115">Optional query parameters</span></span>
<span data-ttu-id="a5fc6-116">Die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="a5fc6-116">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5fc6-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5fc6-117">Request headers</span></span>
| <span data-ttu-id="a5fc6-118">Name</span><span class="sxs-lookup"><span data-stu-id="a5fc6-118">Name</span></span>       | <span data-ttu-id="a5fc6-119">Typ</span><span class="sxs-lookup"><span data-stu-id="a5fc6-119">Type</span></span> | <span data-ttu-id="a5fc6-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5fc6-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5fc6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5fc6-121">Authorization</span></span>  | <span data-ttu-id="a5fc6-122">string</span><span class="sxs-lookup"><span data-stu-id="a5fc6-122">string</span></span>  | <span data-ttu-id="a5fc6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a5fc6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5fc6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5fc6-125">Request body</span></span>
<span data-ttu-id="a5fc6-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a5fc6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5fc6-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5fc6-127">Response</span></span>

<span data-ttu-id="a5fc6-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryRoleTemplate](../resources/directoryroletemplate.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5fc6-128">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5fc6-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5fc6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5fc6-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5fc6-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="a5fc6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5fc6-131">Response</span></span>
<span data-ttu-id="a5fc6-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5fc6-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
