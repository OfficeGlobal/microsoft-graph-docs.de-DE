# <a name="create-educationclass"></a><span data-ttu-id="38ed6-101">EducationClass erstellen</span><span class="sxs-lookup"><span data-stu-id="38ed6-101">Create educationClass</span></span>

<span data-ttu-id="38ed6-102">Erstellen einer neuen Klasse.</span><span class="sxs-lookup"><span data-stu-id="38ed6-102">Create a new class library project.</span></span> <span data-ttu-id="38ed6-103">Dadurch wird auch eine universelle Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="38ed6-103">This will also create a universal group.</span></span> <span data-ttu-id="38ed6-104">Wenn Sie diese API zum Erstellen einer Klasse verwenden, werden der Gruppe spezielle Eigenschaften hinzugefügt, wie z. B. Zuweisungen und besondere Behandlung in Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="38ed6-104">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="38ed6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38ed6-105">Permissions</span></span>
<span data-ttu-id="38ed6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38ed6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="38ed6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38ed6-108">Permission type</span></span>      | <span data-ttu-id="38ed6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38ed6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38ed6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38ed6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="38ed6-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38ed6-111">Not supported.</span></span>  |
|<span data-ttu-id="38ed6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38ed6-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="38ed6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38ed6-113">Not supported.</span></span>  |
|<span data-ttu-id="38ed6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38ed6-114">Application</span></span> | <span data-ttu-id="38ed6-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ed6-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="38ed6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38ed6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="38ed6-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38ed6-117">Request headers</span></span>
| <span data-ttu-id="38ed6-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="38ed6-118">Header</span></span>       | <span data-ttu-id="38ed6-119">Wert</span><span class="sxs-lookup"><span data-stu-id="38ed6-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="38ed6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="38ed6-120">Authorization</span></span>  | <span data-ttu-id="38ed6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38ed6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="38ed6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38ed6-123">Content-Type</span></span>  | <span data-ttu-id="38ed6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="38ed6-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38ed6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38ed6-125">Request body</span></span>
<span data-ttu-id="38ed6-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [educationClass](../resources/educationclass.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="38ed6-126">In the request body, supply a JSON representation of an [invitation](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="38ed6-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="38ed6-127">Response</span></span>
<span data-ttu-id="38ed6-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38ed6-128">If successful, this method returns a `201 Created` response code and an [event](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38ed6-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38ed6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38ed6-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38ed6-130">Request</span></span>
<span data-ttu-id="38ed6-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38ed6-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```

##### <a name="response"></a><span data-ttu-id="38ed6-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="38ed6-132">Response</span></span>
<span data-ttu-id="38ed6-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="38ed6-133">The following is an example of the response.</span></span> 

><span data-ttu-id="38ed6-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="38ed6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->