---
title: directoryObject-Ressourcentyp
description: Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.
ms.openlocfilehash: 0981584bb86b71d06e29de4efc379c84bacac51d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019722"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="bb0f9-104">directoryObject-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bb0f9-104">directoryObject resource type</span></span>

<span data-ttu-id="bb0f9-p102">Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.</span><span class="sxs-lookup"><span data-stu-id="bb0f9-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="bb0f9-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="bb0f9-107">Methods</span></span>

| <span data-ttu-id="bb0f9-108">Methode</span><span class="sxs-lookup"><span data-stu-id="bb0f9-108">Method</span></span>       | <span data-ttu-id="bb0f9-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bb0f9-109">Return Type</span></span>  |<span data-ttu-id="bb0f9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb0f9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb0f9-111">directoryObject abrufen</span><span class="sxs-lookup"><span data-stu-id="bb0f9-111">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="bb0f9-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="bb0f9-112">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="bb0f9-113">Dient zum Lesen der Eigenschaften des directory-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb0f9-113">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="bb0f9-114">directoryObject löschen</span><span class="sxs-lookup"><span data-stu-id="bb0f9-114">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="bb0f9-115">Keine</span><span class="sxs-lookup"><span data-stu-id="bb0f9-115">None</span></span> |<span data-ttu-id="bb0f9-116">Dient zum Löschen eines directory-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb0f9-116">Delete a directory object.</span></span> |
|[<span data-ttu-id="bb0f9-117">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="bb0f9-117">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="bb0f9-118">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="bb0f9-118">String collection</span></span>|<span data-ttu-id="bb0f9-p103">Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="bb0f9-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="bb0f9-121">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="bb0f9-121">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="bb0f9-122">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="bb0f9-122">String collection</span></span>|<span data-ttu-id="bb0f9-p104">Gibt alle Gruppen zurück, in denen das Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="bb0f9-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="bb0f9-125">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="bb0f9-125">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="bb0f9-126">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="bb0f9-126">String collection</span></span>| <span data-ttu-id="bb0f9-p105">Gibt alle Gruppen und Verzeichnisrollen zurück, in denen ein Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="bb0f9-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="bb0f9-129">getByIds</span><span class="sxs-lookup"><span data-stu-id="bb0f9-129">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="bb0f9-130">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bb0f9-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="bb0f9-131">Dient zum Abrufen eines Satzes von Directory-Objekten basierend auf einem Satz angegebener IDs.</span><span class="sxs-lookup"><span data-stu-id="bb0f9-131">Get a set of directory objects based on a set of supplied ids.</span></span> |

## <a name="properties"></a><span data-ttu-id="bb0f9-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb0f9-132">Properties</span></span>

| <span data-ttu-id="bb0f9-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb0f9-133">Property</span></span>   | <span data-ttu-id="bb0f9-134">Typ</span><span class="sxs-lookup"><span data-stu-id="bb0f9-134">Type</span></span> |<span data-ttu-id="bb0f9-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb0f9-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb0f9-136">id</span><span class="sxs-lookup"><span data-stu-id="bb0f9-136">id</span></span>|<span data-ttu-id="bb0f9-137">String</span><span class="sxs-lookup"><span data-stu-id="bb0f9-137">String</span></span>|<span data-ttu-id="bb0f9-p106">Eine GUID, die der eindeutige Bezeichner für das Objekt ist, z. B. 12345678-9abc-def0-1234-56789abcde. Key. Lässt keine Nullwerte zu. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bb0f9-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb0f9-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bb0f9-142">Relationships</span></span>

<span data-ttu-id="bb0f9-143">Keine</span><span class="sxs-lookup"><span data-stu-id="bb0f9-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bb0f9-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bb0f9-144">JSON representation</span></span>

<span data-ttu-id="bb0f9-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bb0f9-145">Here is a JSON representation of the resource</span></span>

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
