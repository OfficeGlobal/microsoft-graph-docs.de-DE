# <a name="check-member-groups"></a><span data-ttu-id="87643-101">Mitgliedergruppen prüfen</span><span class="sxs-lookup"><span data-stu-id="87643-101">Check member groups</span></span>

<span data-ttu-id="87643-p101">Dient zum Überprüfen der Mitgliedschaft in einer angegebenen Liste von Gruppen und gibt aus dieser Liste die Gruppen zurück, in denen das angegebene Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Diese Funktion ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="87643-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="87643-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87643-104">Permissions</span></span>
<span data-ttu-id="87643-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87643-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87643-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87643-107">Permission type</span></span>      | <span data-ttu-id="87643-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87643-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87643-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87643-109">Delegated (work or school account)</span></span> | <span data-ttu-id="87643-110">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="87643-110">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="87643-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87643-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87643-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87643-112">Not supported.</span></span>    |
|<span data-ttu-id="87643-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87643-113">Application</span></span> | <span data-ttu-id="87643-114">User.Read.All und Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="87643-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87643-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87643-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="87643-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87643-116">Request headers</span></span>
| <span data-ttu-id="87643-117">Name</span><span class="sxs-lookup"><span data-stu-id="87643-117">Name</span></span>       | <span data-ttu-id="87643-118">Typ</span><span class="sxs-lookup"><span data-stu-id="87643-118">Type</span></span> | <span data-ttu-id="87643-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87643-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="87643-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="87643-120">Authorization</span></span>  | <span data-ttu-id="87643-121">string</span><span class="sxs-lookup"><span data-stu-id="87643-121">string</span></span>  | <span data-ttu-id="87643-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87643-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87643-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87643-124">Content-Type</span></span>  | <span data-ttu-id="87643-125">application/json</span><span class="sxs-lookup"><span data-stu-id="87643-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87643-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87643-126">Request body</span></span>
<span data-ttu-id="87643-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="87643-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="87643-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="87643-128">Parameter</span></span>    | <span data-ttu-id="87643-129">Typ</span><span class="sxs-lookup"><span data-stu-id="87643-129">Type</span></span>   |<span data-ttu-id="87643-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87643-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87643-131">groupIds</span><span class="sxs-lookup"><span data-stu-id="87643-131">groupIds</span></span>|<span data-ttu-id="87643-132">String</span><span class="sxs-lookup"><span data-stu-id="87643-132">String</span></span>|<span data-ttu-id="87643-p104">Eine Sammlung mit den Objekt-IDs der Gruppen, in denen die Mitgliedschaft überprüft werden soll. Bis zu 20 Gruppen können angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="87643-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="87643-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="87643-135">Response</span></span>

<span data-ttu-id="87643-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87643-136">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87643-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87643-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="87643-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87643-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="87643-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="87643-139">Response</span></span>
<span data-ttu-id="87643-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87643-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
