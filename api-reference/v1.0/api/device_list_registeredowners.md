# <a name="list-registeredowners"></a><span data-ttu-id="7b21d-101">registeredOwners auflisten</span><span class="sxs-lookup"><span data-stu-id="7b21d-101">List registeredOwners</span></span>

<span data-ttu-id="7b21d-102">Dient zum Abrufen einer Liste von Benutzern, die registrierte Besitzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="7b21d-102">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="7b21d-103">Ein registrierter Besitzer ist der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat.</span><span class="sxs-lookup"><span data-stu-id="7b21d-103">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="7b21d-104">Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="7b21d-104">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="7b21d-105">Derzeit kann jeweils nur ein Besitzer vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="7b21d-105">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b21d-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7b21d-106">Permissions</span></span>
<span data-ttu-id="7b21d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b21d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="7b21d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b21d-109">Permission type</span></span>      | <span data-ttu-id="7b21d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b21d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b21d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b21d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b21d-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b21d-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b21d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b21d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b21d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b21d-114">Not supported.</span></span>    |
|<span data-ttu-id="7b21d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b21d-115">Application</span></span> | <span data-ttu-id="7b21d-116">Device.ReadWrite.All and User.ReadBasic.All oder Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b21d-116">Device.ReadWrite.All and User.ReadBasic.All or Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b21d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b21d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b21d-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7b21d-118">Optional query parameters</span></span>
<span data-ttu-id="7b21d-119">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b21d-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7b21d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b21d-120">Request headers</span></span>
| <span data-ttu-id="7b21d-121">Name</span><span class="sxs-lookup"><span data-stu-id="7b21d-121">Name</span></span>       | <span data-ttu-id="7b21d-122">Typ</span><span class="sxs-lookup"><span data-stu-id="7b21d-122">Type</span></span> | <span data-ttu-id="7b21d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b21d-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7b21d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b21d-124">Authorization</span></span>  | <span data-ttu-id="7b21d-125">string</span><span class="sxs-lookup"><span data-stu-id="7b21d-125">string</span></span>  | <span data-ttu-id="7b21d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7b21d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b21d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b21d-128">Request body</span></span>
<span data-ttu-id="7b21d-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7b21d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b21d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b21d-130">Response</span></span>

<span data-ttu-id="7b21d-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b21d-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7b21d-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b21d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b21d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b21d-133">Request</span></span>
<span data-ttu-id="7b21d-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b21d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="7b21d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b21d-135">Response</span></span>
<span data-ttu-id="7b21d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b21d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->