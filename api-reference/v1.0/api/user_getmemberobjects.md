# <a name="user-getmemberobjects"></a><span data-ttu-id="05451-101">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="05451-101">user: getMemberObjects</span></span>
<span data-ttu-id="05451-p101">Gibt alle Gruppen, Verzeichnisrollen und administrativen Einheiten zurück, bei denen der Benutzer ein Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="05451-p101">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="05451-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="05451-104">Permissions</span></span>
<span data-ttu-id="05451-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="05451-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="05451-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="05451-107">Permission type</span></span>      | <span data-ttu-id="05451-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="05451-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05451-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="05451-109">Delegated (work or school account)</span></span> | <span data-ttu-id="05451-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05451-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05451-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="05451-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05451-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="05451-112">Not supported.</span></span>    |
|<span data-ttu-id="05451-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="05451-113">Application</span></span> | <span data-ttu-id="05451-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05451-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05451-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="05451-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="05451-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="05451-116">Request headers</span></span>
| <span data-ttu-id="05451-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="05451-117">Header</span></span>       | <span data-ttu-id="05451-118">Wert</span><span class="sxs-lookup"><span data-stu-id="05451-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="05451-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="05451-119">Authorization</span></span>  | <span data-ttu-id="05451-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="05451-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="05451-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05451-122">Content-Type</span></span>  | <span data-ttu-id="05451-123">application/json</span><span class="sxs-lookup"><span data-stu-id="05451-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="05451-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="05451-124">Request body</span></span>
<span data-ttu-id="05451-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="05451-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="05451-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="05451-126">Parameter</span></span>    | <span data-ttu-id="05451-127">Typ</span><span class="sxs-lookup"><span data-stu-id="05451-127">Type</span></span>   |<span data-ttu-id="05451-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="05451-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05451-129">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="05451-129">securityEnabledOnly</span></span>|<span data-ttu-id="05451-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="05451-130">Boolean</span></span>|<span data-ttu-id="05451-p104">**true** gibt an, dass nur Sicherheitsgruppen, in denender Benutzer Mitglied ist, zurückgegeben werden sollen; **false** gibt an, dass alle Gruppen und Verzeichnisrollen, in denen der Benutzer ein Mitglied ist, zurückgegeben werden sollen. Hinweis: Dieser Parameter darf nur auf **true** gesetzt werden, wenn diese Methode auf einen Benutzer angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="05451-p104">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="05451-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="05451-133">Response</span></span>

<span data-ttu-id="05451-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen und Verzeichnisrollen enthält, von denen der Benutzer ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="05451-134">If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="05451-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="05451-135">Example</span></span>
<span data-ttu-id="05451-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="05451-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="05451-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="05451-137">Request</span></span>
<span data-ttu-id="05451-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="05451-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="05451-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="05451-139">Response</span></span>
<span data-ttu-id="05451-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="05451-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
