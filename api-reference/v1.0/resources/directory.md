---
title: directory-Ressourcentyp (Gelöschte Elemente)
description: . Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden. Nach 30 Tagen wird das Element dauerhaft gelöscht.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 090b9bf476fcaa928f2c6358565ef86af627b8a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966986"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="27641-105">directory-Ressourcentyp (Gelöschte Elemente)</span><span class="sxs-lookup"><span data-stu-id="27641-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="27641-106">Stellt ein gelöschtes Element im Verzeichnis dar.</span><span class="sxs-lookup"><span data-stu-id="27641-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="27641-107">Wenn ein Element gelöscht wird, wird es dem Container „Gelöschte Elemente“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="27641-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="27641-108">Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="27641-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="27641-109">Nach 30 Tagen wird das Element dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="27641-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="27641-110">Die Funktion für gelöschte Elemente wird derzeit nur für die Office 365-Ressourcen [group](group.md) und [user](users.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="27641-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="27641-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="27641-111">Methods</span></span>

| <span data-ttu-id="27641-112">Methode</span><span class="sxs-lookup"><span data-stu-id="27641-112">Method</span></span>         | <span data-ttu-id="27641-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="27641-113">Return Type</span></span> | <span data-ttu-id="27641-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27641-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="27641-115">Gelöschtes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="27641-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="27641-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="27641-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="27641-117">Ruft die Eigenschaften eines gelöschten Elements ab.</span><span class="sxs-lookup"><span data-stu-id="27641-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="27641-118">Gelöschtes Element wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="27641-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="27641-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="27641-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="27641-120">Stellt ein kürzlich gelöschtes Element wieder her.</span><span class="sxs-lookup"><span data-stu-id="27641-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="27641-121">Gelöschte Elemente auflisten</span><span class="sxs-lookup"><span data-stu-id="27641-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="27641-122">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="27641-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="27641-123">Ruft eine Liste der kürzlich gelöschten Elemente ab.</span><span class="sxs-lookup"><span data-stu-id="27641-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="27641-124">Element endgültig löschen</span><span class="sxs-lookup"><span data-stu-id="27641-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="27641-125">Keine</span><span class="sxs-lookup"><span data-stu-id="27641-125">None</span></span> | <span data-ttu-id="27641-126">Löscht ein Element endgültig.</span><span class="sxs-lookup"><span data-stu-id="27641-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="27641-127">Gelöschte Listenelemente Besitz eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="27641-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="27641-128">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="27641-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="27641-129">Enthält Directory Elemente, die einem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="27641-129">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="27641-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="27641-130">Relationships</span></span>
| <span data-ttu-id="27641-131">Beziehung</span><span class="sxs-lookup"><span data-stu-id="27641-131">Relationship</span></span> | <span data-ttu-id="27641-132">Typ</span><span class="sxs-lookup"><span data-stu-id="27641-132">Type</span></span>   |<span data-ttu-id="27641-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27641-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27641-134">deletedItems</span><span class="sxs-lookup"><span data-stu-id="27641-134">deletedItems</span></span>|<span data-ttu-id="27641-135">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="27641-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="27641-136">Kürzlich gelöschte Elemente.</span><span class="sxs-lookup"><span data-stu-id="27641-136">Recently deleted items.</span></span> <span data-ttu-id="27641-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="27641-137">Read-only.</span></span> <span data-ttu-id="27641-138">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="27641-138">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27641-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="27641-139">JSON representation</span></span>
<span data-ttu-id="27641-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="27641-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="27641-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="27641-141">Example</span></span>

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
