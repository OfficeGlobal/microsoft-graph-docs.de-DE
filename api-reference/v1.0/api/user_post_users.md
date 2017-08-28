# <a name="create-user"></a><span data-ttu-id="8b8fa-101">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="8b8fa-101">Create User</span></span>

<span data-ttu-id="8b8fa-p101">Verwenden Sie diese API zum Erstellen eines neuen Benutzers. Der Anforderungstext enthält den zu erstellenden Benutzer. Sie müssen für den Benutzer mindestens die erforderlichen Eigenschaften angeben. Optional können Sie weitere schreibbare Eigenschaften festlegen.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b8fa-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b8fa-106">Permissions</span></span>
<span data-ttu-id="8b8fa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8b8fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8b8fa-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b8fa-109">Permission type</span></span>      | <span data-ttu-id="8b8fa-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b8fa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b8fa-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b8fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8b8fa-112">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b8fa-112">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8b8fa-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b8fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b8fa-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b8fa-114">Not supported.</span></span>    |
|<span data-ttu-id="8b8fa-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b8fa-115">Application</span></span> | <span data-ttu-id="8b8fa-116">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b8fa-116">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b8fa-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b8fa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="8b8fa-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b8fa-118">Request headers</span></span>
| <span data-ttu-id="8b8fa-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8b8fa-119">Header</span></span>       | <span data-ttu-id="8b8fa-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8b8fa-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b8fa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b8fa-121">Authorization</span></span>  | <span data-ttu-id="8b8fa-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8b8fa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b8fa-124">Content-Type</span></span>  | <span data-ttu-id="8b8fa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b8fa-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b8fa-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b8fa-126">Request body</span></span>
<span data-ttu-id="8b8fa-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-127">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="8b8fa-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen eines Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-128">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="8b8fa-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="8b8fa-129">Parameter</span></span> | <span data-ttu-id="8b8fa-130">Typ</span><span class="sxs-lookup"><span data-stu-id="8b8fa-130">Type</span></span> | <span data-ttu-id="8b8fa-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b8fa-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b8fa-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="8b8fa-132">accountEnabled</span></span> |<span data-ttu-id="8b8fa-133">boolean</span><span class="sxs-lookup"><span data-stu-id="8b8fa-133">boolean</span></span> |<span data-ttu-id="8b8fa-134">true, wenn das Konto aktiviert ist; andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-134">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="8b8fa-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8b8fa-135">displayName</span></span> |<span data-ttu-id="8b8fa-136">string</span><span class="sxs-lookup"><span data-stu-id="8b8fa-136">string</span></span> |<span data-ttu-id="8b8fa-137">Der Name des Benutzers, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-137">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="8b8fa-138">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="8b8fa-138">onPremisesImmutableId</span></span> |<span data-ttu-id="8b8fa-139">string</span><span class="sxs-lookup"><span data-stu-id="8b8fa-139">string</span></span> |<span data-ttu-id="8b8fa-140">Muss nur angegeben werden, wenn ein neues Benutzerkonto erstellt wird, wenn Sie eine Verbunddomäne für die UserPrincipalName-Eigenschaft (UPN) des Benutzers verwenden.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-140">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="8b8fa-141">mailNickname</span><span class="sxs-lookup"><span data-stu-id="8b8fa-141">mailNickname</span></span> |<span data-ttu-id="8b8fa-142">string</span><span class="sxs-lookup"><span data-stu-id="8b8fa-142">string</span></span> |<span data-ttu-id="8b8fa-143">Der E-Mail-Alias für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-143">The mail alias for the user.</span></span>|
|<span data-ttu-id="8b8fa-144">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="8b8fa-144">passwordProfile</span></span>|[<span data-ttu-id="8b8fa-145">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="8b8fa-145">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="8b8fa-146">Das Kennwortprofil für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-146">The password profile for the user.</span></span>|
|<span data-ttu-id="8b8fa-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b8fa-147">userPrincipalName</span></span> |<span data-ttu-id="8b8fa-148">string</span><span class="sxs-lookup"><span data-stu-id="8b8fa-148">string</span></span> |<span data-ttu-id="8b8fa-149">Der Benutzerprinzipalname (someuser@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="8b8fa-149">The user principal name (someuser@contoso.com).</span></span>|

## <a name="response"></a><span data-ttu-id="8b8fa-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b8fa-150">Response</span></span>

<span data-ttu-id="8b8fa-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-151">If successful, this method returns `201, Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b8fa-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b8fa-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b8fa-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b8fa-153">Request</span></span>
<span data-ttu-id="8b8fa-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="8b8fa-155">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-155">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8b8fa-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b8fa-156">Response</span></span>
<span data-ttu-id="8b8fa-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b8fa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
