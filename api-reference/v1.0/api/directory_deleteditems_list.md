# <a name="list-deleted-items"></a><span data-ttu-id="9defb-101">Gelöschte Elemente auflisten</span><span class="sxs-lookup"><span data-stu-id="9defb-101">List deleted items</span></span>

<span data-ttu-id="9defb-102">Abrufen einer Liste kürzlich gelöschter Elemente aus den [gelöschten Elementen](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="9defb-102">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="9defb-103">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9defb-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="9defb-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9defb-104">Permissions</span></span>
<span data-ttu-id="9defb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9defb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="9defb-107">Für Benutzer:</span><span class="sxs-lookup"><span data-stu-id="9defb-107">For users:</span></span>

|<span data-ttu-id="9defb-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9defb-108">Permission type</span></span>      | <span data-ttu-id="9defb-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9defb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9defb-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9defb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9defb-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9defb-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9defb-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9defb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9defb-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9defb-113">Not supported.</span></span> |
|<span data-ttu-id="9defb-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9defb-114">Application</span></span> | <span data-ttu-id="9defb-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9defb-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="9defb-116">Für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="9defb-116">For groups:</span></span>

|<span data-ttu-id="9defb-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9defb-117">Permission type</span></span>      | <span data-ttu-id="9defb-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9defb-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9defb-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9defb-119">Delegated (work or school account)</span></span> | <span data-ttu-id="9defb-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9defb-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9defb-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9defb-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9defb-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9defb-122">Not supported.</span></span>    |
|<span data-ttu-id="9defb-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9defb-123">Application</span></span> | <span data-ttu-id="9defb-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9defb-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9defb-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9defb-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="9defb-126">Diese API unterstützt derzeit das Abrufen von Objekttypen von Gruppen (microsoft.graph.group) oder Benutzern (microsoft.graph.user) aus den gelöschten Elementen.</span><span class="sxs-lookup"><span data-stu-id="9defb-126">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="9defb-127">Der Typ wird als ein erforderlicher Bestandteil der URI angegeben.</span><span class="sxs-lookup"><span data-stu-id="9defb-127">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="9defb-128">Aufrufen von GET/Verzeichnis/wird DeletedItems ohne einen Typ nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9defb-128">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="9defb-129">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9defb-129">Optional query parameters</span></span>
<span data-ttu-id="9defb-130">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9defb-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9defb-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9defb-131">Request headers</span></span>
| <span data-ttu-id="9defb-132">Name</span><span class="sxs-lookup"><span data-stu-id="9defb-132">Name</span></span>      |<span data-ttu-id="9defb-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9defb-133">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9defb-134">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9defb-134">Authorization</span></span>  | <span data-ttu-id="9defb-135">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="9defb-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="9defb-136">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9defb-136">Accept</span></span>  | <span data-ttu-id="9defb-137">application/json</span><span class="sxs-lookup"><span data-stu-id="9defb-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9defb-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9defb-138">Request body</span></span>
<span data-ttu-id="9defb-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9defb-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9defb-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9defb-140">Response</span></span>

<span data-ttu-id="9defb-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9defb-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9defb-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9defb-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9defb-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9defb-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="9defb-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="9defb-144">Response</span></span>
<span data-ttu-id="9defb-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9defb-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->