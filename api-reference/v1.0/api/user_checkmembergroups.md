# <a name="checkmembergroups"></a><span data-ttu-id="f0efc-101">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f0efc-101">checkMemberGroups</span></span>
<span data-ttu-id="f0efc-p101">Sucht nach einer Mitgliedschaft in einer angegebenenListe von Gruppen. Gibt aus der Liste diesjenigen Gruppen zurück, bei denen der Benutzer über eine direkte oder transitive Mitgliedschaft verfügt.</span><span class="sxs-lookup"><span data-stu-id="f0efc-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span> 

<span data-ttu-id="f0efc-p102">Sie können maximal 20 Gruppen pro Anforderung überprüfen. Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten kann. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="f0efc-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f0efc-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f0efc-108">Permissions</span></span>
<span data-ttu-id="f0efc-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f0efc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f0efc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f0efc-111">Permission type</span></span>      | <span data-ttu-id="f0efc-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f0efc-112">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f0efc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f0efc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f0efc-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f0efc-114">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="f0efc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f0efc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0efc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f0efc-116">Not supported.</span></span>    | 
|<span data-ttu-id="f0efc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f0efc-117">Application</span></span> | <span data-ttu-id="f0efc-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0efc-118">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f0efc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0efc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="f0efc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f0efc-120">Request headers</span></span>
| <span data-ttu-id="f0efc-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f0efc-121">Header</span></span>       | <span data-ttu-id="f0efc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f0efc-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0efc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0efc-123">Authorization</span></span>  | <span data-ttu-id="f0efc-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f0efc-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f0efc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0efc-126">Content-Type</span></span>  | <span data-ttu-id="f0efc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f0efc-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0efc-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f0efc-128">Request body</span></span>
<span data-ttu-id="f0efc-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="f0efc-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f0efc-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="f0efc-130">Parameter</span></span>    | <span data-ttu-id="f0efc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f0efc-131">Type</span></span>   |<span data-ttu-id="f0efc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0efc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0efc-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="f0efc-133">groupIds</span></span>|<span data-ttu-id="f0efc-134">String</span><span class="sxs-lookup"><span data-stu-id="f0efc-134">String</span></span>|<span data-ttu-id="f0efc-135">Ein Array von Gruppen-IDs</span><span class="sxs-lookup"><span data-stu-id="f0efc-135">An array of group ids</span></span>|

## <a name="response"></a><span data-ttu-id="f0efc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0efc-136">Response</span></span>

<span data-ttu-id="f0efc-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f0efc-137">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0efc-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f0efc-138">Example</span></span>
<span data-ttu-id="f0efc-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f0efc-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f0efc-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0efc-140">Request</span></span>
<span data-ttu-id="f0efc-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f0efc-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="f0efc-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0efc-142">Response</span></span>
<span data-ttu-id="f0efc-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f0efc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
