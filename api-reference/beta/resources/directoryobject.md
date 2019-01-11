---
title: directoryObject-Ressourcentyp
description: Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.
localization_priority: Priority
ms.openlocfilehash: a03ec966f966df556ab0122958b0b8f5464cf4fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889719"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="bac32-104">directoryObject-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bac32-104">directoryObject resource type</span></span>

> <span data-ttu-id="bac32-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bac32-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bac32-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bac32-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bac32-p103">Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.</span><span class="sxs-lookup"><span data-stu-id="bac32-p103">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="bac32-109">Diese Ressource unterstützt Folgendes:</span><span class="sxs-lookup"><span data-stu-id="bac32-109">This resource supports:</span></span>

- <span data-ttu-id="bac32-110">Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/directoryobject-delta.md)-Funktion.</span><span class="sxs-lookup"><span data-stu-id="bac32-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="bac32-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="bac32-111">Methods</span></span>

| <span data-ttu-id="bac32-112">Methode</span><span class="sxs-lookup"><span data-stu-id="bac32-112">Method</span></span>       | <span data-ttu-id="bac32-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bac32-113">Return Type</span></span>  |<span data-ttu-id="bac32-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bac32-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bac32-115">directoryObject abrufen</span><span class="sxs-lookup"><span data-stu-id="bac32-115">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="bac32-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="bac32-116">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="bac32-117">Dient zum Lesen der Eigenschaften des directory-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bac32-117">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="bac32-118">Delete</span><span class="sxs-lookup"><span data-stu-id="bac32-118">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="bac32-119">Keine</span><span class="sxs-lookup"><span data-stu-id="bac32-119">None</span></span> |<span data-ttu-id="bac32-120">Dient zum Löschen eines directory-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bac32-120">Delete a directory object.</span></span> |
|[<span data-ttu-id="bac32-121">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="bac32-121">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="bac32-122">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="bac32-122">String collection</span></span>|<span data-ttu-id="bac32-p104">Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="bac32-p104">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="bac32-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="bac32-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="bac32-126">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="bac32-126">String collection</span></span>|<span data-ttu-id="bac32-p105">Gibt alle Gruppen zurück, in denen das Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="bac32-p105">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="bac32-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="bac32-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="bac32-130">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="bac32-130">String collection</span></span>| <span data-ttu-id="bac32-p106">Gibt alle Gruppen und Verzeichnisrollen zurück, in denen ein Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="bac32-p106">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="bac32-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="bac32-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="bac32-134">[directoryObject](directoryobject.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bac32-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="bac32-135">Dient zum Abrufen eines Satzes von Directory-Objekten basierend auf einem Satz angegebener IDs.</span><span class="sxs-lookup"><span data-stu-id="bac32-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="bac32-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="bac32-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="bac32-137">JSON</span><span class="sxs-lookup"><span data-stu-id="bac32-137">JSON</span></span>| <span data-ttu-id="bac32-138">Anzeigenamen ein Office 365-Gruppe zu überprüfen, oder e-Mail-Spitzname naming Richtlinien entspricht.</span><span class="sxs-lookup"><span data-stu-id="bac32-138">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="bac32-139">delta</span><span class="sxs-lookup"><span data-stu-id="bac32-139">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="bac32-140">directoryObject-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bac32-140">directoryObject collection</span></span>| <span data-ttu-id="bac32-141">Rufen Sie inkrementelle Änderungen für Directory-Objekte.</span><span class="sxs-lookup"><span data-stu-id="bac32-141">Get incremental changes for directory objects.</span></span> <span data-ttu-id="bac32-142">Unterstützt das Filtern nach abgeleitete Typ.</span><span class="sxs-lookup"><span data-stu-id="bac32-142">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="bac32-143">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bac32-143">Properties</span></span>

| <span data-ttu-id="bac32-144">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bac32-144">Property</span></span>   | <span data-ttu-id="bac32-145">Typ</span><span class="sxs-lookup"><span data-stu-id="bac32-145">Type</span></span> |<span data-ttu-id="bac32-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bac32-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bac32-147">id</span><span class="sxs-lookup"><span data-stu-id="bac32-147">id</span></span>|<span data-ttu-id="bac32-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bac32-148">String</span></span>|<span data-ttu-id="bac32-149">Eine Guid, die den eindeutigen Bezeichner für das Objekt ist; beispielsweise 12345678-9abc-def0-1234-56789abcde12.</span><span class="sxs-lookup"><span data-stu-id="bac32-149">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="bac32-150">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="bac32-150">Key.</span></span> <span data-ttu-id="bac32-151">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="bac32-151">Not nullable.</span></span> <span data-ttu-id="bac32-152">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bac32-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bac32-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bac32-153">Relationships</span></span>

<span data-ttu-id="bac32-154">Keine</span><span class="sxs-lookup"><span data-stu-id="bac32-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bac32-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bac32-155">JSON representation</span></span>

<span data-ttu-id="bac32-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bac32-156">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
