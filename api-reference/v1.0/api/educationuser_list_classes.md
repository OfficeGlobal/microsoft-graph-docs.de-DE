# <a name="list-classes"></a><span data-ttu-id="2f18d-101">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="2f18d-101">List classes</span></span>

<span data-ttu-id="2f18d-102">Abrufen einer Liste von Klassenobjekten.</span><span class="sxs-lookup"><span data-stu-id="2f18d-102">Retrieve a list of chartpoints objects.</span></span> <span data-ttu-id="2f18d-103">Hinweis: Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Klassen.</span><span class="sxs-lookup"><span data-stu-id="2f18d-103">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="2f18d-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2f18d-104">Permissions</span></span>
<span data-ttu-id="2f18d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f18d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f18d-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f18d-107">Permission type</span></span>      | <span data-ttu-id="2f18d-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f18d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f18d-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f18d-109">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f18d-110">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2f18d-110">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="2f18d-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f18d-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2f18d-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f18d-112">Not supported.</span></span>  |
|<span data-ttu-id="2f18d-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f18d-113">Application</span></span> | <span data-ttu-id="2f18d-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f18d-114">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f18d-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f18d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2f18d-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2f18d-116">Optional query parameters</span></span>
<span data-ttu-id="2f18d-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f18d-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f18d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f18d-118">Request headers</span></span>
| <span data-ttu-id="2f18d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f18d-119">Header</span></span>       | <span data-ttu-id="2f18d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2f18d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f18d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f18d-121">Authorization</span></span>  | <span data-ttu-id="2f18d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f18d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f18d-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f18d-124">Request body</span></span>
<span data-ttu-id="2f18d-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2f18d-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2f18d-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f18d-126">Response</span></span>
<span data-ttu-id="2f18d-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationClass](../resources/educationclass.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f18d-127">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f18d-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f18d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f18d-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f18d-129">Request</span></span>
<span data-ttu-id="2f18d-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f18d-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="2f18d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f18d-131">Response</span></span>
<span data-ttu-id="2f18d-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f18d-132">The following is an example of the response.</span></span> 

><span data-ttu-id="2f18d-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2f18d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    } 
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->