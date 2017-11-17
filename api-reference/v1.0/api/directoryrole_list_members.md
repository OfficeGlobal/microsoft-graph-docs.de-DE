# <a name="list-members"></a><span data-ttu-id="19a3d-101">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="19a3d-101">List members</span></span>

<span data-ttu-id="19a3d-p101">Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="19a3d-p101">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="19a3d-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="19a3d-104">Permissions</span></span>
<span data-ttu-id="19a3d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="19a3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="19a3d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19a3d-107">Permission type</span></span>      | <span data-ttu-id="19a3d-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19a3d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19a3d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19a3d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="19a3d-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19a3d-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19a3d-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19a3d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a3d-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19a3d-112">Not supported.</span></span>    |
|<span data-ttu-id="19a3d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19a3d-113">Application</span></span> | <span data-ttu-id="19a3d-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19a3d-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19a3d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19a3d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="19a3d-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="19a3d-116">Optional query parameters</span></span>
<span data-ttu-id="19a3d-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="19a3d-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="19a3d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19a3d-118">Request headers</span></span>
| <span data-ttu-id="19a3d-119">Name</span><span class="sxs-lookup"><span data-stu-id="19a3d-119">Name</span></span>       | <span data-ttu-id="19a3d-120">Typ</span><span class="sxs-lookup"><span data-stu-id="19a3d-120">Type</span></span> | <span data-ttu-id="19a3d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19a3d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="19a3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a3d-122">Authorization</span></span>  | <span data-ttu-id="19a3d-123">string</span><span class="sxs-lookup"><span data-stu-id="19a3d-123">string</span></span>  | <span data-ttu-id="19a3d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="19a3d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19a3d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19a3d-126">Request body</span></span>
<span data-ttu-id="19a3d-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="19a3d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19a3d-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="19a3d-128">Response</span></span>

<span data-ttu-id="19a3d-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19a3d-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19a3d-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19a3d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19a3d-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19a3d-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="19a3d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="19a3d-132">Response</span></span>
<span data-ttu-id="19a3d-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19a3d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->