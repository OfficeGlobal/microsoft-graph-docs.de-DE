# <a name="user-getmembergroups"></a><span data-ttu-id="61899-101">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="61899-101">user: getMemberGroups</span></span>
<span data-ttu-id="61899-p101">Gibt alle Gruppen zurück, bei denen der Benutzer Mitglied ist. Die Überprüfung ist transitiv; im Gegensatz zum Lesen der Navigationseigenschaft [memberOf](../api/user_list_memberof.md), die nur die Gruppen zurückgibt, von denen der Benutzer ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="61899-p101">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user_list_memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="61899-p102">Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Die maximale Anzahl von Gruppen, die jede Anfrage zurückgeben kann, ist 2046. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten können. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="61899-p102">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>
## <a name="permissions"></a><span data-ttu-id="61899-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="61899-108">Permissions</span></span>
<span data-ttu-id="61899-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="61899-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

><span data-ttu-id="61899-111">**Hinweis:** Diese API erfordert derzeit mindestens die Berechtigung „Directory.Read.All“.</span><span class="sxs-lookup"><span data-stu-id="61899-111">**Note:** This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="61899-112">Bei der Verwendung der Berechtigung „Group.Read.All“ alleine oder in Kombination mit einer Benutzerberechtigung wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61899-112">Using the Group.Read.All permission, either alone or in combination with a User permission, will return an error.</span></span> <span data-ttu-id="61899-113">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="61899-113">This is a known bug.</span></span>

|<span data-ttu-id="61899-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61899-114">Permission type</span></span>      | <span data-ttu-id="61899-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61899-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61899-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61899-116">Delegated (work or school account)</span></span> | <span data-ttu-id="61899-117">*User.Read and Group.Read.All*, *User.ReadBasic.All and Group.Read.All*, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="61899-117">User.Read and Group.Read.All, User.ReadBasic.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="61899-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61899-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61899-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61899-119">Not supported.</span></span>    |
|<span data-ttu-id="61899-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61899-120">Application</span></span> | <span data-ttu-id="61899-121">*Group.Read.All*, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61899-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61899-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61899-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="61899-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61899-123">Request headers</span></span>
| <span data-ttu-id="61899-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="61899-124">Header</span></span>       | <span data-ttu-id="61899-125">Wert</span><span class="sxs-lookup"><span data-stu-id="61899-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="61899-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="61899-126">Authorization</span></span>  | <span data-ttu-id="61899-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="61899-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="61899-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61899-129">Content-Type</span></span>  | <span data-ttu-id="61899-130">application/json</span><span class="sxs-lookup"><span data-stu-id="61899-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61899-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61899-131">Request body</span></span>
<span data-ttu-id="61899-132">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="61899-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="61899-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="61899-133">Parameter</span></span>    | <span data-ttu-id="61899-134">Typ</span><span class="sxs-lookup"><span data-stu-id="61899-134">Type</span></span>   |<span data-ttu-id="61899-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61899-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61899-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="61899-136">securityEnabledOnly</span></span>|<span data-ttu-id="61899-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61899-137">Boolean</span></span>|<span data-ttu-id="61899-p106">**true** gibt an, dass nur Sicherheitsgruppen, in denen der Benutzer Mitglied ist, zurückgegeben werden sollen; **false** gibt an, dass alle Gruppen, von denen der Benutzer ein Mitglied ist, zurückgegeben werden sollen. Hinweis: Dieser Parameter darf nur auf **true** gesetzt werden, wenn diese Methode auf einen Benutzer angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="61899-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="61899-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="61899-140">Response</span></span>

<span data-ttu-id="61899-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen enthält, von denen der Benutzer ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="61899-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="61899-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61899-142">Example</span></span>
<span data-ttu-id="61899-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="61899-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="61899-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61899-144">Request</span></span>
<span data-ttu-id="61899-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61899-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="61899-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="61899-146">Response</span></span>
<span data-ttu-id="61899-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61899-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
