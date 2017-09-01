# <a name="get-member-objects"></a><span data-ttu-id="58994-101">Mitgliedsobjekte abrufen</span><span class="sxs-lookup"><span data-stu-id="58994-101">Get member objects</span></span>

 <span data-ttu-id="58994-p101">Gibt alle Gruppen und Verzeichnisrollen zurück, in denen ein Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Diese Funktion ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="58994-p101">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="58994-104">Hinweis: Nur Benutzer können Verzeichnisrollen angehören.</span><span class="sxs-lookup"><span data-stu-id="58994-104">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="58994-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="58994-105">Permissions</span></span>
<span data-ttu-id="58994-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="58994-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58994-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58994-108">Permission type</span></span>      | <span data-ttu-id="58994-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58994-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58994-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58994-110">Delegated (work or school account)</span></span> | <span data-ttu-id="58994-111">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="58994-111">User.ReadBasic.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="58994-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58994-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58994-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58994-113">Not supported.</span></span>    |
|<span data-ttu-id="58994-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58994-114">Application</span></span> | <span data-ttu-id="58994-115">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="58994-115">User.ReadBasic.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58994-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58994-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="58994-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58994-117">Request headers</span></span>
| <span data-ttu-id="58994-118">Name</span><span class="sxs-lookup"><span data-stu-id="58994-118">Name</span></span>       | <span data-ttu-id="58994-119">Typ</span><span class="sxs-lookup"><span data-stu-id="58994-119">Type</span></span> | <span data-ttu-id="58994-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58994-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="58994-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58994-121">Authorization</span></span>  | <span data-ttu-id="58994-122">string</span><span class="sxs-lookup"><span data-stu-id="58994-122">string</span></span>  | <span data-ttu-id="58994-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="58994-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58994-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58994-125">Content-Type</span></span>  | <span data-ttu-id="58994-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58994-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="58994-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58994-127">Request body</span></span>
<span data-ttu-id="58994-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="58994-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58994-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="58994-129">Parameter</span></span>    | <span data-ttu-id="58994-130">Typ</span><span class="sxs-lookup"><span data-stu-id="58994-130">Type</span></span>   |<span data-ttu-id="58994-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58994-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58994-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="58994-132">securityEnabledOnly</span></span>|<span data-ttu-id="58994-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="58994-133">Boolean</span></span>| <span data-ttu-id="58994-p104">**true** gibt an, dass nur Sicherheitsgruppen, in denen die Person Mitglied ist, zurückgegeben werden sollen; **falsch** gibt an, dass alle Gruppen und Verzeichnisrollen, in denen die Person ein Mitglied ist, zurückgegeben werden sollen. **Hinweis**: Die Funktion kann nur für einen Benutzer aufgerufen werden, wenn der Parameter **true** lautet.</span><span class="sxs-lookup"><span data-stu-id="58994-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="58994-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="58994-136">Response</span></span>

<span data-ttu-id="58994-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58994-137">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58994-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58994-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="58994-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58994-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="58994-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="58994-140">Response</span></span>
<span data-ttu-id="58994-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58994-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
