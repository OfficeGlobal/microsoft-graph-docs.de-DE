# <a name="user-getmemberobjects"></a><span data-ttu-id="7ad55-101">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="7ad55-101">user: getMemberObjects</span></span>
<span data-ttu-id="7ad55-p101">Gibt alle Gruppen, Verzeichnisrollen und administrativen Einheiten zurück, bei denen der Benutzer ein Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="7ad55-p101">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ad55-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="7ad55-104">Prerequisites</span></span>
<span data-ttu-id="7ad55-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="7ad55-105">One of the following **scopes** is required to execute this API: *Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="7ad55-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ad55-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="7ad55-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ad55-107">Request headers</span></span>
| <span data-ttu-id="7ad55-108">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7ad55-108">Header</span></span>       | <span data-ttu-id="7ad55-109">Wert</span><span class="sxs-lookup"><span data-stu-id="7ad55-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ad55-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ad55-110">Authorization</span></span>  | <span data-ttu-id="7ad55-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7ad55-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7ad55-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ad55-113">Content-Type</span></span>  | <span data-ttu-id="7ad55-114">application/json</span><span class="sxs-lookup"><span data-stu-id="7ad55-114">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ad55-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ad55-115">Request body</span></span>
<span data-ttu-id="7ad55-116">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="7ad55-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7ad55-117">Parameter</span><span class="sxs-lookup"><span data-stu-id="7ad55-117">Parameter</span></span>    | <span data-ttu-id="7ad55-118">Typ</span><span class="sxs-lookup"><span data-stu-id="7ad55-118">Type</span></span>   |<span data-ttu-id="7ad55-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ad55-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ad55-120">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="7ad55-120">securityEnabledOnly</span></span>|<span data-ttu-id="7ad55-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ad55-121">Boolean</span></span>|<span data-ttu-id="7ad55-p103">**true** gibt an, dass nur Sicherheitsgruppen, in denender Benutzer Mitglied ist, zurückgegeben werden sollen; **false** gibt an, dass alle Gruppen und Verzeichnisrollen, in denen der Benutzer ein Mitglied ist, zurückgegeben werden sollen. Hinweis: Dieser Parameter darf nur auf **true** gesetzt werden, wenn diese Methode auf einen Benutzer angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="7ad55-p103">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="7ad55-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ad55-124">Response</span></span>

<span data-ttu-id="7ad55-125">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen und Verzeichnisrollen enthält, von denen der Benutzer ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="7ad55-125">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="7ad55-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ad55-126">Example</span></span>
<span data-ttu-id="7ad55-127">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="7ad55-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7ad55-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ad55-128">Request</span></span>
<span data-ttu-id="7ad55-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ad55-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="7ad55-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ad55-130">Response</span></span>
<span data-ttu-id="7ad55-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ad55-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
