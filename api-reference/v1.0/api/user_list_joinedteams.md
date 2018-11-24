# <a name="list-joinedteams"></a><span data-ttu-id="70108-101">Liste joinedTeams</span><span class="sxs-lookup"><span data-stu-id="70108-101">List joinedTeams</span></span>



<span data-ttu-id="70108-102">Rufen Sie die [Teams](../resources/team.md) in Microsoft-Teams, die der Benutzer ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="70108-102">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="70108-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="70108-103">Permissions</span></span>
<span data-ttu-id="70108-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="70108-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="70108-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70108-106">Permission type</span></span>      | <span data-ttu-id="70108-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70108-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70108-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70108-108">Delegated (work or school account)</span></span> | <span data-ttu-id="70108-109">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70108-109">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="70108-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70108-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70108-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70108-111">Not supported.</span></span>    |
|<span data-ttu-id="70108-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70108-112">Application</span></span> | <span data-ttu-id="70108-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70108-113">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="70108-114">Mit delegiert Benutzerberechtigungen funktioniert diese Operation nur für "me" Benutzer.</span><span class="sxs-lookup"><span data-stu-id="70108-114">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="70108-115">Bei den Anwendungsberechtigungen funktioniert dies für alle Benutzer durch bestimmte Benutzer-Id angeben. ("me" ist alias nicht mit den Anwendungsberechtigungen unterstützt)</span><span class="sxs-lookup"><span data-stu-id="70108-115">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="70108-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70108-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70108-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="70108-117">Optional query parameters</span></span>
<span data-ttu-id="70108-118">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) werden derzeit nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70108-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70108-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70108-119">Request headers</span></span>
| <span data-ttu-id="70108-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="70108-120">Header</span></span>       | <span data-ttu-id="70108-121">Wert</span><span class="sxs-lookup"><span data-stu-id="70108-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70108-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70108-122">Authorization</span></span>  | <span data-ttu-id="70108-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="70108-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="70108-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70108-125">Accept</span></span>  | <span data-ttu-id="70108-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70108-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70108-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70108-127">Request body</span></span>
<span data-ttu-id="70108-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="70108-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70108-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="70108-129">Response</span></span>

<span data-ttu-id="70108-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [group](../resources/group.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70108-130">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70108-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70108-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70108-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70108-132">Request</span></span>
<span data-ttu-id="70108-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70108-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="70108-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="70108-134">Response</span></span>
<span data-ttu-id="70108-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70108-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="70108-138">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="70108-138">See also</span></span>
[<span data-ttu-id="70108-139">Listen Sie alle teams</span><span class="sxs-lookup"><span data-stu-id="70108-139">List all teams</span></span>](../../../concepts/teams_list_all_teams.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
