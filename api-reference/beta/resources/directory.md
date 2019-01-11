---
title: directory-Ressourcentyp (Gelöschte Elemente)
description: . Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden. Nach 30 Tagen wird das Element dauerhaft gelöscht.
localization_priority: Normal
ms.openlocfilehash: 20685f2d9d61726d170744efb5fd2abb571fe934
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834447"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="d1576-105">directory-Ressourcentyp (Gelöschte Elemente)</span><span class="sxs-lookup"><span data-stu-id="d1576-105">directory resource type (deleted items)</span></span>

> <span data-ttu-id="d1576-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d1576-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1576-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1576-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1576-108">Stellt ein gelöschtes Element im Verzeichnis dar.</span><span class="sxs-lookup"><span data-stu-id="d1576-108">Represents a deleted item in the directory.</span></span> <span data-ttu-id="d1576-109">Wenn ein Element gelöscht wird, wird es dem Container „Gelöschte Elemente“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d1576-109">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="d1576-110">Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="d1576-110">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="d1576-111">Nach 30 Tagen wird das Element dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="d1576-111">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="d1576-112">Die Funktion für gelöschte Elemente wird derzeit nur für die Office 365-Ressourcen [group](group.md) und [user](users.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1576-112">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d1576-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="d1576-113">Methods</span></span>

| <span data-ttu-id="d1576-114">Methode</span><span class="sxs-lookup"><span data-stu-id="d1576-114">Method</span></span>         | <span data-ttu-id="d1576-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d1576-115">Return Type</span></span> | <span data-ttu-id="d1576-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1576-116">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="d1576-117">Gelöschtes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="d1576-117">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="d1576-118">directoryObject</span><span class="sxs-lookup"><span data-stu-id="d1576-118">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="d1576-119">Ruft die Eigenschaften eines gelöschten Elements ab.</span><span class="sxs-lookup"><span data-stu-id="d1576-119">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="d1576-120">Gelöschtes Element wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="d1576-120">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="d1576-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="d1576-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="d1576-122">Stellt ein kürzlich gelöschtes Element wieder her.</span><span class="sxs-lookup"><span data-stu-id="d1576-122">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="d1576-123">Gelöschte Elemente auflisten</span><span class="sxs-lookup"><span data-stu-id="d1576-123">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="d1576-124">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d1576-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d1576-125">Ruft eine Liste der kürzlich gelöschten Elemente ab.</span><span class="sxs-lookup"><span data-stu-id="d1576-125">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="d1576-126">Element endgültig löschen</span><span class="sxs-lookup"><span data-stu-id="d1576-126">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="d1576-127">Keine</span><span class="sxs-lookup"><span data-stu-id="d1576-127">None</span></span> | <span data-ttu-id="d1576-128">Löscht ein Element endgültig.</span><span class="sxs-lookup"><span data-stu-id="d1576-128">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="d1576-129">Gelöschte Listenelemente Besitz eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="d1576-129">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="d1576-130">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d1576-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="d1576-131">Enthält Directory Elemente, die einem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="d1576-131">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="d1576-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1576-132">Properties</span></span>
| <span data-ttu-id="d1576-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1576-133">Property</span></span>   | <span data-ttu-id="d1576-134">Typ</span><span class="sxs-lookup"><span data-stu-id="d1576-134">Type</span></span> |<span data-ttu-id="d1576-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1576-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1576-136">id</span><span class="sxs-lookup"><span data-stu-id="d1576-136">id</span></span>|<span data-ttu-id="d1576-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1576-137">String</span></span>| <span data-ttu-id="d1576-138">Ein eindeutiger Bezeichner für das Objekt, z. B. 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="d1576-138">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="d1576-139">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="d1576-139">Key.</span></span> <span data-ttu-id="d1576-140">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="d1576-140">Not nullable.</span></span> <span data-ttu-id="d1576-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1576-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1576-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d1576-142">Relationships</span></span>
| <span data-ttu-id="d1576-143">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d1576-143">Relationship</span></span> | <span data-ttu-id="d1576-144">Typ</span><span class="sxs-lookup"><span data-stu-id="d1576-144">Type</span></span>   |<span data-ttu-id="d1576-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1576-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1576-146">deleteditems</span><span class="sxs-lookup"><span data-stu-id="d1576-146">deleteditems</span></span>|<span data-ttu-id="d1576-147">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d1576-147">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d1576-148">Kürzlich gelöschte Elemente.</span><span class="sxs-lookup"><span data-stu-id="d1576-148">Recently deleted items.</span></span> <span data-ttu-id="d1576-149">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1576-149">Read-only.</span></span> <span data-ttu-id="d1576-150">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="d1576-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1576-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1576-151">JSON representation</span></span>
<span data-ttu-id="d1576-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d1576-152">Here is a JSON representation of the resource.</span></span>

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
