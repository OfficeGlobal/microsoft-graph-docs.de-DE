# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="8d653-101">directory-Ressourcentyp (Gelöschte Elemente)</span><span class="sxs-lookup"><span data-stu-id="8d653-101">directory resource type (deleted items)</span></span>

<span data-ttu-id="8d653-102">Stellt ein gelöschtes Element im Verzeichnis dar.</span><span class="sxs-lookup"><span data-stu-id="8d653-102">Represents a deleted item in the directory.</span></span> <span data-ttu-id="8d653-103">Wenn ein Element gelöscht wird, wird es dem Container „Gelöschte Elemente“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="8d653-103">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="8d653-104">Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="8d653-104">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="8d653-105">Nach 30 Tagen wird das Element dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="8d653-105">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="8d653-106">Die Funktion für gelöschte Elemente wird derzeit nur für die Office 365-Ressourcen [group](group.md) und [user](users.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d653-106">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8d653-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="8d653-107">Methods</span></span>

| <span data-ttu-id="8d653-108">Methode</span><span class="sxs-lookup"><span data-stu-id="8d653-108">Method</span></span>         | <span data-ttu-id="8d653-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8d653-109">Return Type</span></span> | <span data-ttu-id="8d653-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d653-110">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="8d653-111">Gelöschtes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="8d653-111">Get deleted item</span></span>](../api/directory_deleteditems_get.md) | [<span data-ttu-id="8d653-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="8d653-112">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="8d653-113">Ruft die Eigenschaften eines gelöschten Elements ab.</span><span class="sxs-lookup"><span data-stu-id="8d653-113">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="8d653-114">Gelöschtes Element wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="8d653-114">Restore deleted item</span></span>](../api/directory_deleteditems_restore.md) |[<span data-ttu-id="8d653-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="8d653-115">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="8d653-116">Stellt ein kürzlich gelöschtes Element wieder her.</span><span class="sxs-lookup"><span data-stu-id="8d653-116">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="8d653-117">Gelöschte Elemente auflisten</span><span class="sxs-lookup"><span data-stu-id="8d653-117">List deleted items</span></span>](../api/directory_deleteditems_list.md) |<span data-ttu-id="8d653-118">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8d653-118">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="8d653-119">Ruft eine Liste der kürzlich gelöschten Elemente ab.</span><span class="sxs-lookup"><span data-stu-id="8d653-119">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="8d653-120">Element endgültig löschen</span><span class="sxs-lookup"><span data-stu-id="8d653-120">Permanently delete an item</span></span>](../api/directory_deleteditems_delete.md) | <span data-ttu-id="8d653-121">Keine</span><span class="sxs-lookup"><span data-stu-id="8d653-121">None</span></span> | <span data-ttu-id="8d653-122">Löscht ein Element endgültig.</span><span class="sxs-lookup"><span data-stu-id="8d653-122">Permanently deletes an item.</span></span> |
|<span data-ttu-id="8d653-123">[Gelöschte Listenelemente im Besitz eines Benutzers](../api/directory_deleteditems_user_owned.md)</span><span class="sxs-lookup"><span data-stu-id="8d653-123">Added [List deleted items owned by a user](../api/directory_deleteditems_user_owned.md) action to directory (deleted items) resource</span></span> | <span data-ttu-id="8d653-124">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8d653-124">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="8d653-125">Enthält Directory Elemente, die einem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="8d653-125">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8d653-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8d653-126">Relationships</span></span>
| <span data-ttu-id="8d653-127">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8d653-127">Relationship</span></span> | <span data-ttu-id="8d653-128">Typ</span><span class="sxs-lookup"><span data-stu-id="8d653-128">Type</span></span>   |<span data-ttu-id="8d653-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d653-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d653-130">deleteditems</span><span class="sxs-lookup"><span data-stu-id="8d653-130">deleteditems</span></span>|<span data-ttu-id="8d653-131">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8d653-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="8d653-132">Kürzlich gelöschte Elemente.</span><span class="sxs-lookup"><span data-stu-id="8d653-132">Recently deleted items.</span></span> <span data-ttu-id="8d653-133">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8d653-133">Read-only.</span></span> <span data-ttu-id="8d653-134">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8d653-134">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d653-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8d653-135">JSON representation</span></span>
<span data-ttu-id="8d653-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8d653-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="8d653-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d653-137">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->