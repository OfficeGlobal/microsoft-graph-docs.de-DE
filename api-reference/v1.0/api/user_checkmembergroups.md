# <a name="checkmembergroups"></a><span data-ttu-id="5fb03-101">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="5fb03-101">checkMemberGroups</span></span>
<span data-ttu-id="5fb03-p101">Sucht nach einer Mitgliedschaft in einer angegebenenListe von Gruppen. Gibt aus der Liste diesjenigen Gruppen zurück, bei denen der Benutzer über eine direkte oder transitive Mitgliedschaft verfügt.</span><span class="sxs-lookup"><span data-stu-id="5fb03-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span> 

<span data-ttu-id="5fb03-p102">Sie können maximal 20 Gruppen pro Anforderung überprüfen. Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten kann. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="5fb03-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5fb03-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5fb03-108">Permissions</span></span>
<span data-ttu-id="5fb03-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5fb03-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

><span data-ttu-id="5fb03-111">**Hinweis:** Diese API erfordert derzeit mindestens die Berechtigung „Directory.Read.All“.</span><span class="sxs-lookup"><span data-stu-id="5fb03-111">**Note:** This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="5fb03-112">Bei der Verwendung der Berechtigungen „User.Read.All“ oder „User.ReadWrite.All“ wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5fb03-112">Using the User.Read.All or User.ReadWrite.All permissions will return an error.</span></span> <span data-ttu-id="5fb03-113">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="5fb03-113">This is a known bug.</span></span>

|<span data-ttu-id="5fb03-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5fb03-114">Permission type</span></span>      | <span data-ttu-id="5fb03-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5fb03-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fb03-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5fb03-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5fb03-117">*User.Read.All*, *User.ReadWrite.All*, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5fb03-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5fb03-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5fb03-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fb03-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fb03-119">Not supported.</span></span>    |
|<span data-ttu-id="5fb03-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5fb03-120">Application</span></span> | <span data-ttu-id="5fb03-121">*User.Read.All*, *User.ReadWrite.All*, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fb03-121">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fb03-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fb03-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="5fb03-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5fb03-123">Request headers</span></span>
| <span data-ttu-id="5fb03-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5fb03-124">Header</span></span>       | <span data-ttu-id="5fb03-125">Wert</span><span class="sxs-lookup"><span data-stu-id="5fb03-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5fb03-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fb03-126">Authorization</span></span>  | <span data-ttu-id="5fb03-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5fb03-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5fb03-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5fb03-129">Content-Type</span></span>  | <span data-ttu-id="5fb03-130">application/json</span><span class="sxs-lookup"><span data-stu-id="5fb03-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5fb03-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5fb03-131">Request body</span></span>
<span data-ttu-id="5fb03-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="5fb03-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5fb03-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="5fb03-133">Parameter</span></span>    | <span data-ttu-id="5fb03-134">Typ</span><span class="sxs-lookup"><span data-stu-id="5fb03-134">Type</span></span>   |<span data-ttu-id="5fb03-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5fb03-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fb03-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="5fb03-136">groupIds</span></span>|<span data-ttu-id="5fb03-137">String</span><span class="sxs-lookup"><span data-stu-id="5fb03-137">String</span></span>|<span data-ttu-id="5fb03-138">Ein Array von Gruppen-IDs</span><span class="sxs-lookup"><span data-stu-id="5fb03-138">An array of group ids</span></span>|

## <a name="response"></a><span data-ttu-id="5fb03-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fb03-139">Response</span></span>

<span data-ttu-id="5fb03-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5fb03-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fb03-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5fb03-141">Example</span></span>
<span data-ttu-id="5fb03-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5fb03-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5fb03-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fb03-143">Request</span></span>
<span data-ttu-id="5fb03-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5fb03-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5fb03-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fb03-145">Response</span></span>
<span data-ttu-id="5fb03-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5fb03-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
