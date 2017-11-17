# <a name="group-getmembergroups"></a><span data-ttu-id="09486-101">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="09486-101">group: getMemberGroups</span></span>
<span data-ttu-id="09486-p101">Gibt alle Gruppen zurück, bei denen die Gruppe Mitglied ist von. Die Überprüfung ist transitiv; im Gegensatz zum Lesen der Navigationseigenschaft [Mitglied](../api/group_list_memberof.md), die nur die Gruppen zurückgibt, deren direktes Mitglied die Gruppe ist.</span><span class="sxs-lookup"><span data-stu-id="09486-p101">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group_list_memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="09486-p102">Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Die maximale Anzahl von Gruppen, die jede Anfrage zurückgeben kann, ist 2046. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten können. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.</span><span class="sxs-lookup"><span data-stu-id="09486-p102">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="09486-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="09486-108">Permissions</span></span>
<span data-ttu-id="09486-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="09486-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="09486-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09486-111">Permission type</span></span>      | <span data-ttu-id="09486-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09486-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09486-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09486-113">Delegated (work or school account)</span></span> | <span data-ttu-id="09486-114">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09486-114">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="09486-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09486-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09486-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09486-116">Not supported.</span></span>    |
|<span data-ttu-id="09486-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09486-117">Application</span></span> | <span data-ttu-id="09486-118">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09486-118">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09486-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09486-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="09486-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09486-120">Request headers</span></span>
| <span data-ttu-id="09486-121">Name</span><span class="sxs-lookup"><span data-stu-id="09486-121">Name</span></span>       | <span data-ttu-id="09486-122">Typ</span><span class="sxs-lookup"><span data-stu-id="09486-122">Type</span></span> | <span data-ttu-id="09486-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09486-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="09486-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="09486-124">Authorization</span></span>  | <span data-ttu-id="09486-125">string</span><span class="sxs-lookup"><span data-stu-id="09486-125">string</span></span>  | <span data-ttu-id="09486-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="09486-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09486-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09486-128">Request body</span></span>
<span data-ttu-id="09486-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="09486-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09486-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="09486-130">Parameter</span></span>    | <span data-ttu-id="09486-131">Typ</span><span class="sxs-lookup"><span data-stu-id="09486-131">Type</span></span>   |<span data-ttu-id="09486-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09486-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09486-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="09486-133">securityEnabledOnly</span></span>|<span data-ttu-id="09486-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="09486-134">Boolean</span></span>|<span data-ttu-id="09486-p105">Festgelegt auf **false**. Die Option, dass nur Gruppen mit aktivierter Sicherheit zurückgegeben werden, wird nur für Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09486-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="09486-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="09486-137">Response</span></span>

<span data-ttu-id="09486-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Zeichenfolgensammlung im Antworttext zurückgegeben, der die IDs der Gruppen enthält, von denen die Gruppe ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="09486-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="09486-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09486-139">Example</span></span>
<span data-ttu-id="09486-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="09486-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="09486-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09486-141">Request</span></span>
<span data-ttu-id="09486-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09486-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

##### <a name="response"></a><span data-ttu-id="09486-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="09486-143">Response</span></span>
<span data-ttu-id="09486-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09486-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
