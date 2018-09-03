# <a name="get-schemaextension"></a><span data-ttu-id="5846d-101">schemaExtension abrufen</span><span class="sxs-lookup"><span data-stu-id="5846d-101">Get schemaExtension</span></span>
<span data-ttu-id="5846d-102">Mit dieser API können Sie die Eigenschaften der angegebenen Definition des Typs [schemaExtension](../resources/schemaextension.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="5846d-102">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="5846d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5846d-103">Permissions</span></span>
<span data-ttu-id="5846d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5846d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="5846d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5846d-106">Permission type</span></span>      | <span data-ttu-id="5846d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5846d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5846d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5846d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5846d-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5846d-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5846d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5846d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5846d-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5846d-111">Not supported.</span></span>    |
|<span data-ttu-id="5846d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5846d-112">Application</span></span> | <span data-ttu-id="5846d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5846d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5846d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5846d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5846d-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5846d-115">Optional query parameters</span></span>
<span data-ttu-id="5846d-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5846d-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5846d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5846d-117">Request headers</span></span>
| <span data-ttu-id="5846d-118">Name</span><span class="sxs-lookup"><span data-stu-id="5846d-118">Name</span></span>      |<span data-ttu-id="5846d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5846d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5846d-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5846d-120">Authorization</span></span>  | <span data-ttu-id="5846d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5846d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5846d-123">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="5846d-123">Content-Type</span></span>   | <span data-ttu-id="5846d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5846d-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5846d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5846d-125">Request body</span></span>
<span data-ttu-id="5846d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5846d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5846d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5846d-127">Response</span></span>

<span data-ttu-id="5846d-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [schemaExtension](../resources/schemaextension.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5846d-128">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5846d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5846d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5846d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5846d-130">Request</span></span>
<span data-ttu-id="5846d-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5846d-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="5846d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5846d-132">Response</span></span>
<span data-ttu-id="5846d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5846d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id":"graphlearn_test",
    "description": "Yet another test schema",
    "targetTypes": [
        "User", "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "testName",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="5846d-136">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5846d-136">See also</span></span>

- [<span data-ttu-id="5846d-137">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5846d-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="5846d-138">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="5846d-138">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->