# <a name="list-educationclasses"></a><span data-ttu-id="170b9-101">EducationClasses auflisten</span><span class="sxs-lookup"><span data-stu-id="170b9-101">List educationClasses</span></span>

<span data-ttu-id="170b9-102">Abrufen einer Liste von Klassen im Besitz einer Schule.</span><span class="sxs-lookup"><span data-stu-id="170b9-102">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="170b9-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="170b9-103">Permissions</span></span>
<span data-ttu-id="170b9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="170b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="170b9-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="170b9-106">Permission type</span></span>      | <span data-ttu-id="170b9-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="170b9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="170b9-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="170b9-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="170b9-109">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="170b9-109">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="170b9-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="170b9-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="170b9-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="170b9-111">Not supported.</span></span>  |
|<span data-ttu-id="170b9-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="170b9-112">Application</span></span> | <span data-ttu-id="170b9-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170b9-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="170b9-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="170b9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="170b9-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="170b9-115">Optional query parameters</span></span>
<span data-ttu-id="170b9-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="170b9-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="170b9-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="170b9-117">Request headers</span></span>
| <span data-ttu-id="170b9-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="170b9-118">Header</span></span>       | <span data-ttu-id="170b9-119">Wert</span><span class="sxs-lookup"><span data-stu-id="170b9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="170b9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="170b9-120">Authorization</span></span>  | <span data-ttu-id="170b9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="170b9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="170b9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="170b9-123">Request body</span></span>
<span data-ttu-id="170b9-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="170b9-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="170b9-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="170b9-125">Response</span></span>
<span data-ttu-id="170b9-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [educationClass](../resources/educationclass.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="170b9-126">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="170b9-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="170b9-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="170b9-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="170b9-128">Request</span></span>
<span data-ttu-id="170b9-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="170b9-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
##### <a name="response"></a><span data-ttu-id="170b9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="170b9-130">Response</span></span>
<span data-ttu-id="170b9-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="170b9-131">The following is an example of the response.</span></span> 

><span data-ttu-id="170b9-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="170b9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
