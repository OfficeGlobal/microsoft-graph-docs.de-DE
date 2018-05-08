# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="8e006-101">directory-Ressourcentyp (Gelöschte Elemente)</span><span class="sxs-lookup"><span data-stu-id="8e006-101">directory resource type (deleted items)</span></span>

<span data-ttu-id="8e006-102">Stellt ein gelöschtes Element im Verzeichnis dar.</span><span class="sxs-lookup"><span data-stu-id="8e006-102">Represents a deleted item in the directory.</span></span> <span data-ttu-id="8e006-103">Wenn ein Element gelöscht wird, wird es dem Container „Gelöschte Elemente“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="8e006-103">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="8e006-104">Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="8e006-104">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="8e006-105">Nach 30 Tagen wird das Element dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="8e006-105">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="8e006-106">Die Funktion für gelöschte Elemente wird derzeit nur für die Office 365-Ressourcen [group](group.md) und [user](users.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e006-106">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8e006-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="8e006-107">Methods</span></span>

| <span data-ttu-id="8e006-108">Methode</span><span class="sxs-lookup"><span data-stu-id="8e006-108">Method</span></span>         | <span data-ttu-id="8e006-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8e006-109">Return Type</span></span> | <span data-ttu-id="8e006-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e006-110">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="8e006-111">Gelöschtes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="8e006-111">Get deleted item</span></span>](../api/directory_deleteditems_get.md) | [<span data-ttu-id="8e006-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="8e006-112">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="8e006-113">Ruft die Eigenschaften eines gelöschten Elements ab.</span><span class="sxs-lookup"><span data-stu-id="8e006-113">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="8e006-114">Gelöschtes Element wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="8e006-114">Restore deleted item</span></span>](../api/directory_deleteditems_restore.md) |[<span data-ttu-id="8e006-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="8e006-115">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="8e006-116">Stellt ein kürzlich gelöschtes Element wieder her.</span><span class="sxs-lookup"><span data-stu-id="8e006-116">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="8e006-117">Gelöschte Elemente auflisten</span><span class="sxs-lookup"><span data-stu-id="8e006-117">List deleted items</span></span>](../api/directory_deleteditems_list.md) |<span data-ttu-id="8e006-118">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8e006-118">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="8e006-119">Ruft eine Liste der kürzlich gelöschten Elemente ab.</span><span class="sxs-lookup"><span data-stu-id="8e006-119">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="8e006-120">Element endgültig löschen</span><span class="sxs-lookup"><span data-stu-id="8e006-120">Permanently delete an item</span></span>](../api/directory_deleteditems_delete.md) | <span data-ttu-id="8e006-121">Keine</span><span class="sxs-lookup"><span data-stu-id="8e006-121">None</span></span> | <span data-ttu-id="8e006-122">Löscht ein Element endgültig.</span><span class="sxs-lookup"><span data-stu-id="8e006-122">Permanently deletes an item.</span></span> |

## <a name="properties"></a><span data-ttu-id="8e006-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8e006-123">Properties</span></span>
| <span data-ttu-id="8e006-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e006-124">Property</span></span>   | <span data-ttu-id="8e006-125">Typ</span><span class="sxs-lookup"><span data-stu-id="8e006-125">Type</span></span> |<span data-ttu-id="8e006-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e006-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e006-127">id</span><span class="sxs-lookup"><span data-stu-id="8e006-127">id</span></span>|<span data-ttu-id="8e006-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e006-128">String</span></span>| <span data-ttu-id="8e006-129">Ein eindeutiger Bezeichner für das Objekt, z. B. 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="8e006-129">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span> <span data-ttu-id="8e006-130">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="8e006-130">Key</span></span> <span data-ttu-id="8e006-131">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8e006-131">Not nullable.</span></span> <span data-ttu-id="8e006-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8e006-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e006-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8e006-133">Relationships</span></span>
| <span data-ttu-id="8e006-134">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8e006-134">Relationship</span></span> | <span data-ttu-id="8e006-135">Typ</span><span class="sxs-lookup"><span data-stu-id="8e006-135">Type</span></span>   |<span data-ttu-id="8e006-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e006-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e006-137">deleteditems</span><span class="sxs-lookup"><span data-stu-id="8e006-137">deleteditems</span></span>|<span data-ttu-id="8e006-138">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8e006-138">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="8e006-139">Kürzlich gelöschte Elemente.</span><span class="sxs-lookup"><span data-stu-id="8e006-139">Recently deleted items.</span></span> <span data-ttu-id="8e006-140">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8e006-140">Read-only.</span></span> <span data-ttu-id="8e006-141">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8e006-141">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e006-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8e006-142">JSON representation</span></span>
<span data-ttu-id="8e006-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8e006-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
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