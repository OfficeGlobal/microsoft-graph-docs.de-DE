# <a name="get-deleted-item"></a><span data-ttu-id="2ff1e-101">Gelöschtes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="2ff1e-101">Get deleted item</span></span>

<span data-ttu-id="2ff1e-102">Abrufen der Eigenschaften eines kürzlich gelöschten Elements aus den [gelöschten Elementen](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="2ff1e-102">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="2ff1e-103">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ff1e-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ff1e-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2ff1e-104">Permissions</span></span>
<span data-ttu-id="2ff1e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ff1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="2ff1e-107">Für Benutzer:</span><span class="sxs-lookup"><span data-stu-id="2ff1e-107">For users:</span></span>

|<span data-ttu-id="2ff1e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2ff1e-108">Permission type</span></span>      | <span data-ttu-id="2ff1e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2ff1e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ff1e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2ff1e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2ff1e-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ff1e-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2ff1e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2ff1e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ff1e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ff1e-113">Not supported.</span></span> |
|<span data-ttu-id="2ff1e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2ff1e-114">Application</span></span> | <span data-ttu-id="2ff1e-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ff1e-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="2ff1e-116">Für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="2ff1e-116">For groups:</span></span>

|<span data-ttu-id="2ff1e-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2ff1e-117">Permission type</span></span>      | <span data-ttu-id="2ff1e-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2ff1e-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ff1e-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2ff1e-119">Delegated (work or school account)</span></span> | <span data-ttu-id="2ff1e-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ff1e-120">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2ff1e-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2ff1e-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ff1e-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ff1e-122">Not supported.</span></span>    |
|<span data-ttu-id="2ff1e-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2ff1e-123">Application</span></span> | <span data-ttu-id="2ff1e-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ff1e-124">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ff1e-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ff1e-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ff1e-126">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2ff1e-126">Optional query parameters</span></span>
<span data-ttu-id="2ff1e-127">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2ff1e-127">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ff1e-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2ff1e-128">Request headers</span></span>
| <span data-ttu-id="2ff1e-129">Name</span><span class="sxs-lookup"><span data-stu-id="2ff1e-129">Name</span></span>      |<span data-ttu-id="2ff1e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ff1e-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2ff1e-131">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2ff1e-131">Authorization</span></span>  | <span data-ttu-id="2ff1e-132">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="2ff1e-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="2ff1e-133">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2ff1e-133">Accept</span></span>  | <span data-ttu-id="2ff1e-134">application/json</span><span class="sxs-lookup"><span data-stu-id="2ff1e-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ff1e-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2ff1e-135">Request body</span></span>
<span data-ttu-id="2ff1e-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2ff1e-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ff1e-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ff1e-137">Response</span></span>

<span data-ttu-id="2ff1e-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ff1e-138">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2ff1e-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2ff1e-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ff1e-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ff1e-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="2ff1e-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ff1e-141">Response</span></span>
<span data-ttu-id="2ff1e-p102">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ff1e-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->