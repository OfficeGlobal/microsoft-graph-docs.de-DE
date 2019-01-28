---
title: directoryObject-Ressourcentyp
description: Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ba2454a5eda90ec50dbd6a0c152383bb42a437d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573956"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="0c540-104">directoryObject-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0c540-104">directoryObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c540-p102">Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.</span><span class="sxs-lookup"><span data-stu-id="0c540-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="0c540-107">Diese Ressource unterstützt Folgendes:</span><span class="sxs-lookup"><span data-stu-id="0c540-107">This resource supports:</span></span>

- <span data-ttu-id="0c540-108">Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/directoryobject-delta.md)-Funktion.</span><span class="sxs-lookup"><span data-stu-id="0c540-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="0c540-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="0c540-109">Methods</span></span>

| <span data-ttu-id="0c540-110">Methode</span><span class="sxs-lookup"><span data-stu-id="0c540-110">Method</span></span>       | <span data-ttu-id="0c540-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0c540-111">Return Type</span></span>  |<span data-ttu-id="0c540-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c540-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c540-113">directoryObject abrufen</span><span class="sxs-lookup"><span data-stu-id="0c540-113">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="0c540-114">directoryObject</span><span class="sxs-lookup"><span data-stu-id="0c540-114">directoryObject</span></span>](../resources/directoryobject.md) |<span data-ttu-id="0c540-115">Dient zum Lesen der Eigenschaften des directory-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c540-115">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="0c540-116">Delete</span><span class="sxs-lookup"><span data-stu-id="0c540-116">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="0c540-117">Keine</span><span class="sxs-lookup"><span data-stu-id="0c540-117">None</span></span> |<span data-ttu-id="0c540-118">Dient zum Löschen eines directory-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c540-118">Delete a directory object.</span></span> |
|[<span data-ttu-id="0c540-119">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="0c540-119">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="0c540-120">String collection</span><span class="sxs-lookup"><span data-stu-id="0c540-120">String collection</span></span>|<span data-ttu-id="0c540-p103">Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="0c540-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="0c540-123">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="0c540-123">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="0c540-124">String collection</span><span class="sxs-lookup"><span data-stu-id="0c540-124">String collection</span></span>|<span data-ttu-id="0c540-p104">Gibt alle Gruppen zurück, in denen das Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="0c540-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="0c540-127">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="0c540-127">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="0c540-128">String collection</span><span class="sxs-lookup"><span data-stu-id="0c540-128">String collection</span></span>| <span data-ttu-id="0c540-p105">Gibt alle Gruppen und Verzeichnisrollen zurück, in denen ein Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="0c540-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="0c540-131">getByIds</span><span class="sxs-lookup"><span data-stu-id="0c540-131">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="0c540-132">[directoryObject](../resources/directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0c540-132">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="0c540-133">Dient zum Abrufen eines Satzes von Directory-Objekten basierend auf einem Satz angegebener IDs.</span><span class="sxs-lookup"><span data-stu-id="0c540-133">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="0c540-134">validateProperties</span><span class="sxs-lookup"><span data-stu-id="0c540-134">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="0c540-135">JSON</span><span class="sxs-lookup"><span data-stu-id="0c540-135">JSON</span></span>| <span data-ttu-id="0c540-136">Überprüft, ob der Anzeigename oder E-Mail-Kontoname einer Office 365-Gruppe den Benennungsrichtlinien entspricht.</span><span class="sxs-lookup"><span data-stu-id="0c540-136">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="0c540-137">delta</span><span class="sxs-lookup"><span data-stu-id="0c540-137">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="0c540-138">directoryObject-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0c540-138">directoryObject collection</span></span>| <span data-ttu-id="0c540-139">Abrufen inkrementeller Änderungen für Verzeichnisobjekte.</span><span class="sxs-lookup"><span data-stu-id="0c540-139">Get incremental changes for directory objects.</span></span> <span data-ttu-id="0c540-140">Unterstützt das Filtern nach abgeleitetem Typ.</span><span class="sxs-lookup"><span data-stu-id="0c540-140">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="0c540-141">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0c540-141">Properties</span></span>

| <span data-ttu-id="0c540-142">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c540-142">Property</span></span>   | <span data-ttu-id="0c540-143">Typ</span><span class="sxs-lookup"><span data-stu-id="0c540-143">Type</span></span> |<span data-ttu-id="0c540-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c540-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c540-145">id</span><span class="sxs-lookup"><span data-stu-id="0c540-145">id</span></span>|<span data-ttu-id="0c540-146">String</span><span class="sxs-lookup"><span data-stu-id="0c540-146">String</span></span>|<span data-ttu-id="0c540-147">Eine GUID, die der eindeutige Bezeichner für das Objekt ist, z. B. 12345678-9abc-def0-1234-56789abcde12.</span><span class="sxs-lookup"><span data-stu-id="0c540-147">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span> <span data-ttu-id="0c540-148">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="0c540-148">Key.</span></span> <span data-ttu-id="0c540-149">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0c540-149">Not nullable.</span></span> <span data-ttu-id="0c540-150">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0c540-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c540-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0c540-151">Relationships</span></span>

<span data-ttu-id="0c540-152">Keine</span><span class="sxs-lookup"><span data-stu-id="0c540-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c540-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0c540-153">JSON representation</span></span>

<span data-ttu-id="0c540-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0c540-154">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
}-->

```json
{
  "id": "string (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
