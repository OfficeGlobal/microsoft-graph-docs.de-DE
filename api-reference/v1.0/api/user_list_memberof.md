# <a name="list-memberof"></a><span data-ttu-id="483ff-101">memberOf auflisten</span><span class="sxs-lookup"><span data-stu-id="483ff-101">List memberOf</span></span>

<span data-ttu-id="483ff-102">Mit dieser API können Sie die [Gruppen](../resources/group.md) und [Verzeichnisrollen](../resources/directoryrole.md) abrufen, denen ein Benutzer als direktes Mitglied zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="483ff-102">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="483ff-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="483ff-103">Permissions</span></span>
<span data-ttu-id="483ff-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="483ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="483ff-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="483ff-106">Permission type</span></span>      | <span data-ttu-id="483ff-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="483ff-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="483ff-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="483ff-108">Delegated (work or school account)</span></span> | <span data-ttu-id="483ff-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="483ff-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="483ff-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="483ff-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="483ff-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="483ff-111">Not supported.</span></span>    |
|<span data-ttu-id="483ff-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="483ff-112">Application</span></span> | <span data-ttu-id="483ff-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483ff-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="483ff-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="483ff-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="483ff-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="483ff-115">Optional query parameters</span></span>
<span data-ttu-id="483ff-p102">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort. $filter wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="483ff-p102">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response. $filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="483ff-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="483ff-118">Request headers</span></span>
| <span data-ttu-id="483ff-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="483ff-119">Header</span></span>       | <span data-ttu-id="483ff-120">Wert</span><span class="sxs-lookup"><span data-stu-id="483ff-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="483ff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="483ff-121">Authorization</span></span>  | <span data-ttu-id="483ff-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="483ff-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="483ff-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="483ff-124">Accept</span></span>  | <span data-ttu-id="483ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="483ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="483ff-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="483ff-126">Request body</span></span>
<span data-ttu-id="483ff-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="483ff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="483ff-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="483ff-128">Response</span></span>

<span data-ttu-id="483ff-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="483ff-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="483ff-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="483ff-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="483ff-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="483ff-131">Request</span></span>
<span data-ttu-id="483ff-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="483ff-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="483ff-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="483ff-133">Response</span></span>
<span data-ttu-id="483ff-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="483ff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
