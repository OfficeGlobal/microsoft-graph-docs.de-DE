# <a name="get-educationclass"></a><span data-ttu-id="8c2be-101">EducationClass abrufen</span><span class="sxs-lookup"><span data-stu-id="8c2be-101">Get educationClass</span></span>

<span data-ttu-id="8c2be-102">Abrufen einer Klasse aus dem System.</span><span class="sxs-lookup"><span data-stu-id="8c2be-102">Retrieve a class from the system.</span></span> <span data-ttu-id="8c2be-103">Eine Klasse ist eine universelle Gruppe mit einer speziellen Eigenschaft, die dem System anzeigt, dass die Gruppe eine Klasse darstellt.</span><span class="sxs-lookup"><span data-stu-id="8c2be-103">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="8c2be-104">Gruppenmitglieder stellen die Kursteilnehmer dar. Gruppenadministratoren stellen die Lehrer in der Klasse dar.</span><span class="sxs-lookup"><span data-stu-id="8c2be-104">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="8c2be-105">Wenn Sie das delegierte Token verwenden, werden dem Benutzer nur Klassen angezeigt, in denen er Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="8c2be-105">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c2be-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8c2be-106">Permissions</span></span>
<span data-ttu-id="8c2be-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8c2be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c2be-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c2be-109">Permission type</span></span>      | <span data-ttu-id="8c2be-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c2be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c2be-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c2be-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="8c2be-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="8c2be-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="8c2be-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c2be-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8c2be-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c2be-114">Not supported</span></span>  |
|<span data-ttu-id="8c2be-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c2be-115">Application</span></span> | <span data-ttu-id="8c2be-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c2be-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8c2be-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c2be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8c2be-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8c2be-118">Optional query parameters</span></span>
<span data-ttu-id="8c2be-119">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8c2be-119">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c2be-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c2be-120">Request headers</span></span>
| <span data-ttu-id="8c2be-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8c2be-121">Header</span></span>       | <span data-ttu-id="8c2be-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8c2be-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c2be-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8c2be-123">Authorization</span></span>  | <span data-ttu-id="8c2be-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8c2be-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c2be-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c2be-126">Request body</span></span>
<span data-ttu-id="8c2be-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8c2be-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8c2be-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c2be-128">Response</span></span>
<span data-ttu-id="8c2be-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c2be-129">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c2be-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c2be-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c2be-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c2be-131">Request</span></span>
<span data-ttu-id="8c2be-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c2be-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="8c2be-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c2be-133">Response</span></span>
<span data-ttu-id="8c2be-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8c2be-134">The following is an example of the response.</span></span> 

><span data-ttu-id="8c2be-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8c2be-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->