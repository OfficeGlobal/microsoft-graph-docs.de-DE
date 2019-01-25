---
title: directory-Ressourcentyp (Gelöschte Elemente)
description: . Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden. Nach 30 Tagen wird das Element dauerhaft gelöscht.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 22c5b959f87b6178fa406bc4fd5d00ad52e5cf55
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517484"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="09c2f-105">directory-Ressourcentyp (Gelöschte Elemente)</span><span class="sxs-lookup"><span data-stu-id="09c2f-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09c2f-106">Stellt ein gelöschtes Element im Verzeichnis dar.</span><span class="sxs-lookup"><span data-stu-id="09c2f-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="09c2f-107">Wenn ein Element gelöscht wird, wird es dem Container „Gelöschte Elemente“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="09c2f-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="09c2f-108">Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="09c2f-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="09c2f-109">Nach 30 Tagen wird das Element dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="09c2f-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="09c2f-110">Die Funktion für gelöschte Elemente wird derzeit nur für die Office 365-Ressourcen [group](group.md) und [user](users.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09c2f-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="09c2f-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="09c2f-111">Methods</span></span>

| <span data-ttu-id="09c2f-112">Methode</span><span class="sxs-lookup"><span data-stu-id="09c2f-112">Method</span></span>         | <span data-ttu-id="09c2f-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="09c2f-113">Return Type</span></span> | <span data-ttu-id="09c2f-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09c2f-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="09c2f-115">Gelöschtes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="09c2f-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="09c2f-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="09c2f-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="09c2f-117">Ruft die Eigenschaften eines gelöschten Elements ab.</span><span class="sxs-lookup"><span data-stu-id="09c2f-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="09c2f-118">Gelöschtes Element wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="09c2f-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="09c2f-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="09c2f-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="09c2f-120">Stellt ein kürzlich gelöschtes Element wieder her.</span><span class="sxs-lookup"><span data-stu-id="09c2f-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="09c2f-121">Gelöschte Elemente auflisten</span><span class="sxs-lookup"><span data-stu-id="09c2f-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="09c2f-122">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="09c2f-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="09c2f-123">Ruft eine Liste der kürzlich gelöschten Elemente ab.</span><span class="sxs-lookup"><span data-stu-id="09c2f-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="09c2f-124">Element endgültig löschen</span><span class="sxs-lookup"><span data-stu-id="09c2f-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="09c2f-125">Keine</span><span class="sxs-lookup"><span data-stu-id="09c2f-125">None</span></span> | <span data-ttu-id="09c2f-126">Löscht ein Element endgültig.</span><span class="sxs-lookup"><span data-stu-id="09c2f-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="09c2f-127">Gelöschte Listenelemente Besitz eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="09c2f-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="09c2f-128">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="09c2f-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="09c2f-129">Enthält Directory Elemente, die einem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="09c2f-129">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="09c2f-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="09c2f-130">Properties</span></span>
| <span data-ttu-id="09c2f-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="09c2f-131">Property</span></span>   | <span data-ttu-id="09c2f-132">Typ</span><span class="sxs-lookup"><span data-stu-id="09c2f-132">Type</span></span> |<span data-ttu-id="09c2f-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09c2f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09c2f-134">id</span><span class="sxs-lookup"><span data-stu-id="09c2f-134">id</span></span>|<span data-ttu-id="09c2f-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09c2f-135">String</span></span>| <span data-ttu-id="09c2f-136">Ein eindeutiger Bezeichner für das Objekt, z. B. 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="09c2f-136">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="09c2f-137">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="09c2f-137">Key.</span></span> <span data-ttu-id="09c2f-138">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="09c2f-138">Not nullable.</span></span> <span data-ttu-id="09c2f-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="09c2f-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09c2f-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="09c2f-140">Relationships</span></span>
| <span data-ttu-id="09c2f-141">Beziehung</span><span class="sxs-lookup"><span data-stu-id="09c2f-141">Relationship</span></span> | <span data-ttu-id="09c2f-142">Typ</span><span class="sxs-lookup"><span data-stu-id="09c2f-142">Type</span></span>   |<span data-ttu-id="09c2f-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09c2f-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09c2f-144">deleteditems</span><span class="sxs-lookup"><span data-stu-id="09c2f-144">deleteditems</span></span>|<span data-ttu-id="09c2f-145">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="09c2f-145">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="09c2f-146">Kürzlich gelöschte Elemente.</span><span class="sxs-lookup"><span data-stu-id="09c2f-146">Recently deleted items.</span></span> <span data-ttu-id="09c2f-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="09c2f-147">Read-only.</span></span> <span data-ttu-id="09c2f-148">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="09c2f-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09c2f-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="09c2f-149">JSON representation</span></span>
<span data-ttu-id="09c2f-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="09c2f-150">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
