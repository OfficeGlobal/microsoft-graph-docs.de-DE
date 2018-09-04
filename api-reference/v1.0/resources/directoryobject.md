# <a name="directoryobject-resource-type"></a><span data-ttu-id="720c5-101">Ressourcentyp directoryObject</span><span class="sxs-lookup"><span data-stu-id="720c5-101">directoryObject resource type</span></span>

<span data-ttu-id="720c5-p101">Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.</span><span class="sxs-lookup"><span data-stu-id="720c5-p101">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="720c5-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="720c5-104">Methods</span></span>

| <span data-ttu-id="720c5-105">Methode</span><span class="sxs-lookup"><span data-stu-id="720c5-105">Method</span></span>       | <span data-ttu-id="720c5-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="720c5-106">Return Type</span></span>  |<span data-ttu-id="720c5-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="720c5-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="720c5-108">directoryObject abrufen</span><span class="sxs-lookup"><span data-stu-id="720c5-108">Get directoryObject</span></span>](../api/directoryobject_get.md) | [<span data-ttu-id="720c5-109">directoryObject</span><span class="sxs-lookup"><span data-stu-id="720c5-109">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="720c5-110">Dient zum Lesen der Eigenschaften des directory-Objekts.</span><span class="sxs-lookup"><span data-stu-id="720c5-110">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="720c5-111">directoryObject löschen</span><span class="sxs-lookup"><span data-stu-id="720c5-111">Delete directoryObject</span></span>](../api/directoryobject_delete.md) | <span data-ttu-id="720c5-112">Keine</span><span class="sxs-lookup"><span data-stu-id="720c5-112">None</span></span> |<span data-ttu-id="720c5-113">Dient zum Löschen eines directory-Objekts.</span><span class="sxs-lookup"><span data-stu-id="720c5-113">Delete a directory object.</span></span> |
|[<span data-ttu-id="720c5-114">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="720c5-114">checkMemberGroups</span></span>](../api/directoryobject_checkmembergroups.md)|<span data-ttu-id="720c5-115">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="720c5-115">String collection</span></span>|<span data-ttu-id="720c5-p102">Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="720c5-p102">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="720c5-118">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="720c5-118">getMemberGroups</span></span>](../api/directoryobject_getmembergroups.md)|<span data-ttu-id="720c5-119">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="720c5-119">String collection</span></span>|<span data-ttu-id="720c5-p103">Gibt alle Gruppen zurück, in denen das Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="720c5-p103">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="720c5-122">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="720c5-122">getMemberObjects</span></span>](../api/directoryobject_getmemberobjects.md)|<span data-ttu-id="720c5-123">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="720c5-123">String collection</span></span>| <span data-ttu-id="720c5-p104">Gibt alle Gruppen und Verzeichnisrollen zurück, in denen ein Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="720c5-p104">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="720c5-126">getByIds</span><span class="sxs-lookup"><span data-stu-id="720c5-126">getByIds</span></span>](../api/directoryobject_getbyids.md) | <span data-ttu-id="720c5-127">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="720c5-127">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="720c5-128">Dient zum Abrufen eines Satzes von Directory-Objekten basierend auf einem Satz angegebener IDs.</span><span class="sxs-lookup"><span data-stu-id="720c5-128">Get a set of directory objects based on a set of supplied ids.</span></span> |

## <a name="properties"></a><span data-ttu-id="720c5-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="720c5-129">Properties</span></span>

| <span data-ttu-id="720c5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="720c5-130">Property</span></span>   | <span data-ttu-id="720c5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="720c5-131">Type</span></span> |<span data-ttu-id="720c5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="720c5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="720c5-133">id</span><span class="sxs-lookup"><span data-stu-id="720c5-133">id</span></span>|<span data-ttu-id="720c5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="720c5-134">String</span></span>|<span data-ttu-id="720c5-p105">Eine GUID, die der eindeutige Bezeichner für das Objekt ist, z. B. 12345678-9abc-def0-1234-56789abcde. Key. Lässt keine Nullwerte zu. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="720c5-p105">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="720c5-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="720c5-139">Relationships</span></span>

<span data-ttu-id="720c5-140">Keine</span><span class="sxs-lookup"><span data-stu-id="720c5-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="720c5-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="720c5-141">JSON representation</span></span>

<span data-ttu-id="720c5-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="720c5-142">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
