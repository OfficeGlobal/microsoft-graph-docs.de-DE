# <a name="restore-deleted-item"></a><span data-ttu-id="bac61-101">Gelöschtes Element wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="bac61-101">Restore deleted item</span></span>

<span data-ttu-id="bac61-102">Stellt ein kürzlich gelöschtes Element aus den [gelöschten Elementen](../resources/directory.md) wieder her.</span><span class="sxs-lookup"><span data-stu-id="bac61-102">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="bac61-103">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bac61-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="bac61-104">Wenn ein Element versehentlich gelöscht wurde, können es vollständig wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="bac61-104">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="bac61-105">Ein kürzlich gelöschtes Element bleibt bis zu 30 Tage verfügbar.</span><span class="sxs-lookup"><span data-stu-id="bac61-105">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="bac61-106">Nach 30 Tagen wird das Element dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="bac61-106">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="bac61-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bac61-107">Permissions</span></span>
<span data-ttu-id="bac61-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bac61-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="bac61-110">Für Benutzer:</span><span class="sxs-lookup"><span data-stu-id="bac61-110">For users:</span></span>

|<span data-ttu-id="bac61-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bac61-111">Permission type</span></span>      | <span data-ttu-id="bac61-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bac61-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bac61-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bac61-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bac61-114">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bac61-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="bac61-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bac61-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bac61-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bac61-116">Not supported.</span></span> |
|<span data-ttu-id="bac61-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bac61-117">Application</span></span> | <span data-ttu-id="bac61-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bac61-118">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="bac61-119">Für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="bac61-119">For groups:</span></span>

|<span data-ttu-id="bac61-120">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bac61-120">Permission type</span></span>      | <span data-ttu-id="bac61-121">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bac61-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bac61-122">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bac61-122">Delegated (work or school account)</span></span> | <span data-ttu-id="bac61-123">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bac61-123">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="bac61-124">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bac61-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bac61-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bac61-125">Not supported.</span></span>    |
|<span data-ttu-id="bac61-126">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bac61-126">Application</span></span> | <span data-ttu-id="bac61-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bac61-127">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bac61-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bac61-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="bac61-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bac61-129">Request headers</span></span>
| <span data-ttu-id="bac61-130">Name</span><span class="sxs-lookup"><span data-stu-id="bac61-130">Name</span></span>       | <span data-ttu-id="bac61-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bac61-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bac61-132">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="bac61-132">Authorization</span></span>  | <span data-ttu-id="bac61-133">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="bac61-133">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="bac61-134">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bac61-134">Accept</span></span> | <span data-ttu-id="bac61-135">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="bac61-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bac61-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bac61-136">Request body</span></span>
<span data-ttu-id="bac61-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bac61-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bac61-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="bac61-138">Response</span></span>

<span data-ttu-id="bac61-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bac61-139">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bac61-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bac61-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bac61-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bac61-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="bac61-142">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bac61-142">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bac61-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="bac61-143">Response</span></span>
<span data-ttu-id="bac61-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bac61-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
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
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->