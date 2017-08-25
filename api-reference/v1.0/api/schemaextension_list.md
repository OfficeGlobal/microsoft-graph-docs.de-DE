# <a name="list-schemaextensions"></a><span data-ttu-id="66528-101">schemaExtensions auflisten</span><span class="sxs-lookup"><span data-stu-id="66528-101">List schemaExtensions</span></span>

<span data-ttu-id="66528-102">Dient zum Abrufen einer Liste von [schemaExtension](../resources/schemaextension.md)-Objekten, die von beliebigen Apps erstellt wurden, die Sie im aktuellen Mandanten besitzen (kann **InDevelopment**, **Available** oder **Deprecated** sein), sowie aller anderen Schemaerweiterungen im Besitz von anderen Apps, die als **Available** gekennzeichnet sind.</span><span class="sxs-lookup"><span data-stu-id="66528-102">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="66528-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="66528-103">Permissions</span></span>
<span data-ttu-id="66528-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="66528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="66528-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66528-106">Permission type</span></span>      | <span data-ttu-id="66528-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66528-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="66528-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66528-108">Delegated (work or school account)</span></span> | <span data-ttu-id="66528-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66528-109">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="66528-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66528-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66528-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66528-111">Not supported.</span></span>    | 
|<span data-ttu-id="66528-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66528-112">Application</span></span> | <span data-ttu-id="66528-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66528-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="66528-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66528-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66528-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="66528-115">Optional query parameters</span></span>
<span data-ttu-id="66528-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="66528-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66528-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66528-117">Request headers</span></span>
| <span data-ttu-id="66528-118">Name</span><span class="sxs-lookup"><span data-stu-id="66528-118">Name</span></span>      |<span data-ttu-id="66528-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66528-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66528-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="66528-120">Authorization</span></span>  | <span data-ttu-id="66528-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="66528-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66528-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66528-123">Content-Type</span></span>   | <span data-ttu-id="66528-124">application/json</span><span class="sxs-lookup"><span data-stu-id="66528-124">application/json</span></span> | 

## <a name="request-body"></a><span data-ttu-id="66528-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66528-125">Request body</span></span>
<span data-ttu-id="66528-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="66528-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66528-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="66528-127">Response</span></span>

<span data-ttu-id="66528-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [schemaExtension](../resources/schemaextension.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66528-128">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66528-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66528-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66528-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66528-130">Request</span></span>
<span data-ttu-id="66528-131">Im folgenden Beispiel wird gezeigt, wie Sie unter allen zugänglichen Erweiterungen nach einer bestimmten Erweiterung suchen, indem Sie nach ihrer eindeutigen **ID** filtern.</span><span class="sxs-lookup"><span data-stu-id="66528-131">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="66528-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="66528-132">Response</span></span>
<span data-ttu-id="66528-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66528-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
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
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="66528-136">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="66528-136">See also</span></span>

- [<span data-ttu-id="66528-137">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="66528-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="66528-138">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="66528-138">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->