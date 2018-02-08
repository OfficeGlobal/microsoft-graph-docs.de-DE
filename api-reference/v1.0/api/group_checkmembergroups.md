# <a name="group-checkmembergroups"></a><span data-ttu-id="337fc-101">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="337fc-101">group: checkMemberGroups</span></span>
<span data-ttu-id="337fc-p101">Sucht nach einer Mitgliedschaft in der angegebenen Liste von Gruppen. Gibt aus der Liste diejenigen Gruppen zurück, bei denen die angegebene Gruppe über eine direkte oder transitive Mitgliedschaft verfügt.</span><span class="sxs-lookup"><span data-stu-id="337fc-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span> 

<span data-ttu-id="337fc-p102">Sie können maximal 20 Gruppen pro Anforderung überprüfen. Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten kann. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="337fc-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span> 

## <a name="permissions"></a><span data-ttu-id="337fc-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="337fc-108">Permissions</span></span>
<span data-ttu-id="337fc-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="337fc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

><span data-ttu-id="337fc-111">**Hinweis:** Diese API erfordert derzeit mindestens die Berechtigung „Directory.Read.All“.</span><span class="sxs-lookup"><span data-stu-id="337fc-111">**Note:** This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="337fc-112">Bei der Verwendung der Berechtigung „Group.Read.All“ kommt es zu einem Fehler.</span><span class="sxs-lookup"><span data-stu-id="337fc-112">Using the Group.Read.All permission will return an error.</span></span> <span data-ttu-id="337fc-113">Dies ist ein bekanntes Problem.</span><span class="sxs-lookup"><span data-stu-id="337fc-113">This is a known bug.</span></span>

|<span data-ttu-id="337fc-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="337fc-114">Permission type</span></span>      | <span data-ttu-id="337fc-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="337fc-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|

<span data-ttu-id="337fc-116">|Delegiert (Geschäfts-, Schul- oder Unikonto) | *Group.Read.All*, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All | |Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="337fc-116">|Delegated (work or school account) | *Group.Read.All*, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All | |Delegated (personal Microsoft account) | Not supported.</span></span>    <span data-ttu-id="337fc-117">| |Anwendung | *Group.Read.All*, Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="337fc-117">| |Application | *Group.Read.All*, Directory.Read.All.</span></span> <span data-ttu-id="337fc-118">Directory.ReadWrite.All |</span><span class="sxs-lookup"><span data-stu-id="337fc-118">Directory.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="337fc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="337fc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="337fc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="337fc-120">Request headers</span></span>
| <span data-ttu-id="337fc-121">Name</span><span class="sxs-lookup"><span data-stu-id="337fc-121">Name</span></span>       | <span data-ttu-id="337fc-122">Typ</span><span class="sxs-lookup"><span data-stu-id="337fc-122">Type</span></span> | <span data-ttu-id="337fc-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="337fc-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="337fc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="337fc-124">Authorization</span></span>  | <span data-ttu-id="337fc-125">string</span><span class="sxs-lookup"><span data-stu-id="337fc-125">string</span></span>  | <span data-ttu-id="337fc-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="337fc-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="337fc-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="337fc-128">Request body</span></span>
<span data-ttu-id="337fc-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="337fc-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="337fc-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="337fc-130">Parameter</span></span>    | <span data-ttu-id="337fc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="337fc-131">Type</span></span>   |<span data-ttu-id="337fc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="337fc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="337fc-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="337fc-133">groupIds</span></span>|<span data-ttu-id="337fc-134">String</span><span class="sxs-lookup"><span data-stu-id="337fc-134">String</span></span>|<span data-ttu-id="337fc-135">Ein Array von Gruppen-IDs</span><span class="sxs-lookup"><span data-stu-id="337fc-135">An array of group ids</span></span>|

## <a name="response"></a><span data-ttu-id="337fc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="337fc-136">Response</span></span>

<span data-ttu-id="337fc-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="337fc-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="337fc-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="337fc-138">Example</span></span>
<span data-ttu-id="337fc-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="337fc-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="337fc-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="337fc-140">Request</span></span>
<span data-ttu-id="337fc-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="337fc-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="337fc-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="337fc-142">Response</span></span>
<span data-ttu-id="337fc-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="337fc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
