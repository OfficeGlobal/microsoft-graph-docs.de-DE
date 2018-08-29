# <a name="get-member-groups"></a><span data-ttu-id="9776e-101">Mitgliedergruppen abrufen</span><span class="sxs-lookup"><span data-stu-id="9776e-101">Get member groups</span></span>

<span data-ttu-id="9776e-p101">Gibt alle Gruppen zurück, in denen das angegebene Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Diese Funktion ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="9776e-p101">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="9776e-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9776e-104">Permissions</span></span>
<span data-ttu-id="9776e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9776e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9776e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9776e-107">Permission type</span></span>      | <span data-ttu-id="9776e-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9776e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9776e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9776e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9776e-110">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9776e-110">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="9776e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9776e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9776e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9776e-112">Not supported.</span></span>    |
|<span data-ttu-id="9776e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9776e-113">Application</span></span> | <span data-ttu-id="9776e-114">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9776e-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9776e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9776e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="9776e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9776e-116">Request headers</span></span>
| <span data-ttu-id="9776e-117">Name</span><span class="sxs-lookup"><span data-stu-id="9776e-117">Name</span></span>       | <span data-ttu-id="9776e-118">Typ</span><span class="sxs-lookup"><span data-stu-id="9776e-118">Type</span></span> | <span data-ttu-id="9776e-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9776e-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9776e-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9776e-120">Authorization</span></span>  | <span data-ttu-id="9776e-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9776e-121">string</span></span>  | <span data-ttu-id="9776e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9776e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9776e-124">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="9776e-124">Content-Type</span></span>   | <span data-ttu-id="9776e-125">string</span><span class="sxs-lookup"><span data-stu-id="9776e-125">string</span></span>  | <span data-ttu-id="9776e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9776e-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9776e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9776e-127">Request body</span></span>
<span data-ttu-id="9776e-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9776e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9776e-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="9776e-129">Parameter</span></span>    | <span data-ttu-id="9776e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9776e-130">Type</span></span>   |<span data-ttu-id="9776e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9776e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9776e-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="9776e-132">securityEnabledOnly</span></span>|<span data-ttu-id="9776e-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="9776e-133">Boolean</span></span>| <span data-ttu-id="9776e-p104">**true** gibt an, dass nur Sicherheitsgruppen, in denen die Person Mitglied ist, zurückgegeben werden sollen; **falsch** gibt an, dass alle Gruppen und Verzeichnisrollen, in denen die Person ein Mitglied ist, zurückgegeben werden sollen. **Hinweis**: Die Funktion kann nur für einen Benutzer aufgerufen werden, wenn der Parameter **true** lautet.</span><span class="sxs-lookup"><span data-stu-id="9776e-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="9776e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9776e-136">Response</span></span>

<span data-ttu-id="9776e-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9776e-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9776e-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9776e-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9776e-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9776e-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="9776e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9776e-140">Response</span></span>
<span data-ttu-id="9776e-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9776e-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
