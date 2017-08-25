# <a name="group-checkmembergroups"></a><span data-ttu-id="bcadb-101">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="bcadb-101">group: checkMemberGroups</span></span>
<span data-ttu-id="bcadb-p101">Sucht nach einer Mitgliedschaft in der angegebenen Liste von Gruppen. Gibt aus der Liste diejenigen Gruppen zurück, bei denen die angegebene Gruppe über eine direkte oder transitive Mitgliedschaft verfügt.</span><span class="sxs-lookup"><span data-stu-id="bcadb-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span> 

<span data-ttu-id="bcadb-p102">Sie können maximal 20 Gruppen pro Anforderung überprüfen. Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten kann. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="bcadb-p102">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span> 

## <a name="permissions"></a><span data-ttu-id="bcadb-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bcadb-108">Permissions</span></span>
<span data-ttu-id="bcadb-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bcadb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bcadb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bcadb-111">Permission type</span></span>      | <span data-ttu-id="bcadb-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bcadb-112">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="bcadb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bcadb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bcadb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bcadb-114">Not supported.</span></span>    | 
|<span data-ttu-id="bcadb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bcadb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcadb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bcadb-116">Not supported.</span></span>    | 
|<span data-ttu-id="bcadb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bcadb-117">Application</span></span> | <span data-ttu-id="bcadb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bcadb-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bcadb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bcadb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="bcadb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bcadb-120">Request headers</span></span>
| <span data-ttu-id="bcadb-121">Name</span><span class="sxs-lookup"><span data-stu-id="bcadb-121">Name</span></span>       | <span data-ttu-id="bcadb-122">Typ</span><span class="sxs-lookup"><span data-stu-id="bcadb-122">Type</span></span> | <span data-ttu-id="bcadb-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bcadb-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bcadb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcadb-124">Authorization</span></span>  | <span data-ttu-id="bcadb-125">string</span><span class="sxs-lookup"><span data-stu-id="bcadb-125">string</span></span>  | <span data-ttu-id="bcadb-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bcadb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcadb-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bcadb-128">Request body</span></span>
<span data-ttu-id="bcadb-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="bcadb-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bcadb-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="bcadb-130">Parameter</span></span>    | <span data-ttu-id="bcadb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bcadb-131">Type</span></span>   |<span data-ttu-id="bcadb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bcadb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcadb-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="bcadb-133">groupIds</span></span>|<span data-ttu-id="bcadb-134">String</span><span class="sxs-lookup"><span data-stu-id="bcadb-134">String</span></span>|<span data-ttu-id="bcadb-135">Ein Array von Gruppen-IDs</span><span class="sxs-lookup"><span data-stu-id="bcadb-135">An array of group ids</span></span>|

## <a name="response"></a><span data-ttu-id="bcadb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="bcadb-136">Response</span></span>

<span data-ttu-id="bcadb-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bcadb-137">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcadb-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bcadb-138">Example</span></span>
<span data-ttu-id="bcadb-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="bcadb-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bcadb-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bcadb-140">Request</span></span>
<span data-ttu-id="bcadb-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bcadb-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="bcadb-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="bcadb-142">Response</span></span>
<span data-ttu-id="bcadb-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bcadb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
