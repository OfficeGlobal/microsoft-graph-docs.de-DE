# <a name="list-available-drives"></a><span data-ttu-id="031da-101">Verfügbare Laufwerke auflisten</span><span class="sxs-lookup"><span data-stu-id="031da-101">List available drives</span></span>

<span data-ttu-id="031da-p101">Dient zum Abrufen der Liste der [Laufwerk](../resources/drive.md)-Ressourcen für einen Ziel-[Benutzer](../resources/user.md) oder eine Ziel-[Gruppe](../resources/group.md). Ihre App kann auch den Satz von Dokumentbibliotheken auf der SharePoint-Stammwebsite anfordern.</span><span class="sxs-lookup"><span data-stu-id="031da-p101">Retrieve the list of [Drive](../resources/drive.md) resources available for a target [User](../resources/user.md) or [Group](../resources/group.md). Your app can also request the set of document libraries on the SharePoint root site.</span></span>

## <a name="permissions"></a><span data-ttu-id="031da-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="031da-104">Permissions</span></span>

<span data-ttu-id="031da-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="031da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="031da-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="031da-107">Permission type</span></span>      | <span data-ttu-id="031da-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="031da-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="031da-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="031da-109">Delegated (work or school account)</span></span> | <span data-ttu-id="031da-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="031da-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="031da-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="031da-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="031da-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="031da-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="031da-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="031da-113">Application</span></span> | <span data-ttu-id="031da-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="031da-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="031da-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="031da-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives
GET /me/drives
GET /sites/{site-id}/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="031da-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="031da-116">Optional query parameters</span></span>

<span data-ttu-id="031da-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="031da-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="031da-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="031da-118">Request body</span></span>

<span data-ttu-id="031da-119">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="031da-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="031da-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="031da-120">Response</span></span>

<span data-ttu-id="031da-121">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Drive](../resources/drive.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="031da-121">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="031da-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="031da-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="031da-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="031da-123">Request</span></span>

<span data-ttu-id="031da-124">Hier ist ein Beispiel für die Anforderung der Laufwerke des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="031da-124">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drives"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/drives
```

##### <a name="response"></a><span data-ttu-id="031da-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="031da-125">Response</span></span>

<span data-ttu-id="031da-126">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="031da-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 579

{
  "value": [
    {
      "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
      "driveType": "business",
      "owner": {
          "user": {
              "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
              "displayName": "Ryan Gregg"
          }
      },
      "quota": {
          "deleted": 256938,
          "remaining": 1099447353539,
          "state": "normal",
          "total": 1099511627776
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="031da-127">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="031da-127">Remarks</span></span>

<span data-ttu-id="031da-p103">Die meisten Benutzer verfügen nur über eine einzige Laufwerkressource. Gruppen und einige Benutzer verfügen möglicherweise über mehrere Laufwerke.</span><span class="sxs-lookup"><span data-stu-id="031da-p103">Most users will only have a single Drive resource. Groups and some users may have multiple drive available.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/List Drives"
}-->
