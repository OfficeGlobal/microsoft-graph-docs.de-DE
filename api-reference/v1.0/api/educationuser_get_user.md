# <a name="get-user"></a><span data-ttu-id="1bb3e-101">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="1bb3e-101">Get user</span></span>

<span data-ttu-id="1bb3e-102">Abrufen des einfachen Verzeichnis-**Benutzers**, der diesem **educationUser** entspricht.</span><span class="sxs-lookup"><span data-stu-id="1bb3e-102">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="1bb3e-103">**Hinweis:** Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Schulen.</span><span class="sxs-lookup"><span data-stu-id="1bb3e-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="1bb3e-104">Verwenden Sie in diesem Fall die Ressource `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="1bb3e-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bb3e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1bb3e-105">Permissions</span></span>
<span data-ttu-id="1bb3e-106">Zum Aufrufen dieser API ist eine Kombination von Berechtigungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1bb3e-106">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="1bb3e-107">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1bb3e-107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1bb3e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1bb3e-108">Permission type</span></span>      | <span data-ttu-id="1bb3e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1bb3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bb3e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1bb3e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1bb3e-111">Eine aus EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write sowie entweder Directory.Read.All oder User.Read</span><span class="sxs-lookup"><span data-stu-id="1bb3e-111">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="1bb3e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1bb3e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1bb3e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1bb3e-113">Not supported.</span></span>  |
|<span data-ttu-id="1bb3e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1bb3e-114">Application</span></span> | <span data-ttu-id="1bb3e-115">EduRoster.Read.All, EduRoster.ReadWrite.All und Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bb3e-115">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="1bb3e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bb3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="1bb3e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1bb3e-117">Request headers</span></span>
| <span data-ttu-id="1bb3e-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1bb3e-118">Header</span></span>       | <span data-ttu-id="1bb3e-119">Wert</span><span class="sxs-lookup"><span data-stu-id="1bb3e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1bb3e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bb3e-120">Authorization</span></span>  | <span data-ttu-id="1bb3e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1bb3e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bb3e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1bb3e-123">Request body</span></span>
<span data-ttu-id="1bb3e-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1bb3e-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1bb3e-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bb3e-125">Response</span></span>
<span data-ttu-id="1bb3e-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bb3e-126">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bb3e-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1bb3e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bb3e-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bb3e-128">Request</span></span>
<span data-ttu-id="1bb3e-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1bb3e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/user
```
##### <a name="response"></a><span data-ttu-id="1bb3e-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bb3e-130">Response</span></span>
<span data-ttu-id="1bb3e-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1bb3e-131">The following is an example of the response.</span></span> 

><span data-ttu-id="1bb3e-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1bb3e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

<!-- uuid: FC4AAF57-A0ED-4899-B104-A8B89B72AD5A
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->