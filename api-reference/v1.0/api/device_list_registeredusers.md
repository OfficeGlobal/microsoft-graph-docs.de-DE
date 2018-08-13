# <a name="list-registeredusers"></a><span data-ttu-id="064b1-101">registeredUsers auflisten</span><span class="sxs-lookup"><span data-stu-id="064b1-101">List registeredUsers</span></span>

<span data-ttu-id="064b1-102">Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="064b1-102">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="064b1-103">Für mit der Cloud verknüpfte Geräte und registrierte persönliche Geräte werden registrierte Benutzer bei der Registrierung auf den gleichen Wert wie registrierte Besitzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="064b1-103">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="064b1-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="064b1-104">Permissions</span></span>
<span data-ttu-id="064b1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="064b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="064b1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="064b1-107">Permission type</span></span>      | <span data-ttu-id="064b1-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="064b1-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="064b1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="064b1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="064b1-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="064b1-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="064b1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="064b1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="064b1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="064b1-112">Not supported.</span></span>    |
|<span data-ttu-id="064b1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="064b1-113">Application</span></span> | <span data-ttu-id="064b1-114">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="064b1-114">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="064b1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="064b1-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="064b1-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="064b1-116">Optional query parameters</span></span>
<span data-ttu-id="064b1-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="064b1-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="064b1-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="064b1-118">Request headers</span></span>
| <span data-ttu-id="064b1-119">Name</span><span class="sxs-lookup"><span data-stu-id="064b1-119">Name</span></span>       | <span data-ttu-id="064b1-120">Typ</span><span class="sxs-lookup"><span data-stu-id="064b1-120">Type</span></span> | <span data-ttu-id="064b1-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="064b1-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="064b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="064b1-122">Authorization</span></span>  | <span data-ttu-id="064b1-123">string</span><span class="sxs-lookup"><span data-stu-id="064b1-123">string</span></span>  | <span data-ttu-id="064b1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="064b1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="064b1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="064b1-126">Request body</span></span>
<span data-ttu-id="064b1-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="064b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="064b1-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="064b1-128">Response</span></span>

<span data-ttu-id="064b1-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="064b1-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="064b1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="064b1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="064b1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="064b1-131">Request</span></span>
<span data-ttu-id="064b1-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="064b1-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="064b1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="064b1-133">Response</span></span>
<span data-ttu-id="064b1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="064b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->