---
title: Ressourcentyp contactFolder
description: Ein Ordner, der Kontakte enthält.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a4fcb5152a3d7cb5f26214cf2b0a1e4a31dc1ffb
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575870"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="6ab5f-103">Ressourcentyp contactFolder</span><span class="sxs-lookup"><span data-stu-id="6ab5f-103">contactFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ab5f-104">Ein Ordner, der Kontakte enthält.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-104">A folder that contains contacts.</span></span>

<span data-ttu-id="6ab5f-105">Diese Ressource unterstützt die Verwendung einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen einer [delta](../api/contactfolder-delta.md)-Funktion.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="6ab5f-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="6ab5f-106">Methods</span></span>

| <span data-ttu-id="6ab5f-107">Methode</span><span class="sxs-lookup"><span data-stu-id="6ab5f-107">Method</span></span>       | <span data-ttu-id="6ab5f-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6ab5f-108">Return Type</span></span>  |<span data-ttu-id="6ab5f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6ab5f-110">contactFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="6ab5f-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="6ab5f-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6ab5f-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="6ab5f-112">Dient zum Abrufen eines Kontaktordners anhand der Kontaktordner-ID.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="6ab5f-113">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6ab5f-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="6ab5f-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6ab5f-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="6ab5f-115">Dient zum Aktualisieren des contactFolder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="6ab5f-116">Löschen</span><span class="sxs-lookup"><span data-stu-id="6ab5f-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="6ab5f-117">Keine</span><span class="sxs-lookup"><span data-stu-id="6ab5f-117">None</span></span> |<span data-ttu-id="6ab5f-118">Dient zum Löschen des contactFolder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="6ab5f-119">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="6ab5f-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="6ab5f-120">[ContactFolder](contactfolder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-120">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="6ab5f-121">Dient zum Abrufen einer Sammlung von untergeordneten Ordnern unter dem angegebenen Kontaktordner.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="6ab5f-122">Untergeordneten contactFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="6ab5f-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="6ab5f-123">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6ab5f-123">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="6ab5f-124">Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="6ab5f-125">delta</span><span class="sxs-lookup"><span data-stu-id="6ab5f-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="6ab5f-126">[contact](contact.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="6ab5f-127">Dient zum Abrufen eines Satzes von Kontaktordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="6ab5f-128">Kontakte im Ordner auflisten</span><span class="sxs-lookup"><span data-stu-id="6ab5f-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="6ab5f-129">[contact](contact.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="6ab5f-130">Dient zum Abrufen einer Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers (`.../me/contacts`) oder aus dem angegebenen Kontaktordner.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="6ab5f-131">Kontakt in Ordner erstellen</span><span class="sxs-lookup"><span data-stu-id="6ab5f-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="6ab5f-132">Kontakt</span><span class="sxs-lookup"><span data-stu-id="6ab5f-132">contact</span></span>](contact.md)| <span data-ttu-id="6ab5f-133">Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="6ab5f-134">**Erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="6ab5f-134">**Extended properties**</span></span>| | |
|[<span data-ttu-id="6ab5f-135">Create single-value extended property</span><span class="sxs-lookup"><span data-stu-id="6ab5f-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="6ab5f-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6ab5f-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="6ab5f-137">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen contactFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="6ab5f-138">contactFolder mit erweiterter einwertiger Eigenschaft abrufen</span><span class="sxs-lookup"><span data-stu-id="6ab5f-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="6ab5f-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6ab5f-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="6ab5f-140">Dient zum Abrufen von contactFolders-Elementen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="6ab5f-141">Mehrwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="6ab5f-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="6ab5f-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6ab5f-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="6ab5f-143">Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen contactFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="6ab5f-144">contactFolder mit erweiterter mehrwertiger Eigenschaft abrufen</span><span class="sxs-lookup"><span data-stu-id="6ab5f-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="6ab5f-145">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6ab5f-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="6ab5f-146">Dient zum Abrufen eines contactFolders-Elements mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="6ab5f-147">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ab5f-147">Properties</span></span>
| <span data-ttu-id="6ab5f-148">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ab5f-148">Property</span></span>     | <span data-ttu-id="6ab5f-149">Typ</span><span class="sxs-lookup"><span data-stu-id="6ab5f-149">Type</span></span>   |<span data-ttu-id="6ab5f-150">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ab5f-151">displayName</span><span class="sxs-lookup"><span data-stu-id="6ab5f-151">displayName</span></span>|<span data-ttu-id="6ab5f-152">String</span><span class="sxs-lookup"><span data-stu-id="6ab5f-152">String</span></span>|<span data-ttu-id="6ab5f-153">Der Anzeigename des Ordners.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-153">The folder's display name.</span></span>|
|<span data-ttu-id="6ab5f-154">id</span><span class="sxs-lookup"><span data-stu-id="6ab5f-154">id</span></span>|<span data-ttu-id="6ab5f-155">String</span><span class="sxs-lookup"><span data-stu-id="6ab5f-155">String</span></span>|<span data-ttu-id="6ab5f-p101">Eindeutiger Bezeichner des Kontaktordners. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="6ab5f-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="6ab5f-158">parentFolderId</span></span>|<span data-ttu-id="6ab5f-159">String</span><span class="sxs-lookup"><span data-stu-id="6ab5f-159">String</span></span>|<span data-ttu-id="6ab5f-160">Die ID des übergeordneten Ordners des Ordners.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-160">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="6ab5f-161">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="6ab5f-161">wellKnownName</span></span>|<span data-ttu-id="6ab5f-162">string</span><span class="sxs-lookup"><span data-stu-id="6ab5f-162">string</span></span>|<span data-ttu-id="6ab5f-163">Der Name des Ordners, wenn der Ordner einen erkannten Ordner ist.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-163">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="6ab5f-164">Derzeit `contacts` ist die einzige erkannten Kontakteordner.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-164">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ab5f-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6ab5f-165">Relationships</span></span>
| <span data-ttu-id="6ab5f-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-166">Relationship</span></span> | <span data-ttu-id="6ab5f-167">Typ</span><span class="sxs-lookup"><span data-stu-id="6ab5f-167">Type</span></span>   |<span data-ttu-id="6ab5f-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ab5f-169">childFolders</span><span class="sxs-lookup"><span data-stu-id="6ab5f-169">childFolders</span></span>|<span data-ttu-id="6ab5f-170">[ContactFolder](contactfolder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-170">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="6ab5f-p103">Die Sammlung der untergeordneten Ordner im Ordner. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-p103">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6ab5f-175">Kontakte</span><span class="sxs-lookup"><span data-stu-id="6ab5f-175">contacts</span></span>|<span data-ttu-id="6ab5f-176">[Contact](contact.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-176">[Contact](contact.md) collection</span></span>|<span data-ttu-id="6ab5f-p104">Die Kontakte im Ordner. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-p104">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6ab5f-181">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6ab5f-181">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="6ab5f-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="6ab5f-p105">Die Sammlung erweiterter mehrwertiger Eigenschaften, die für das contactFolder-Element definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-p105">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6ab5f-186">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6ab5f-186">singleValueLegacyExtendedProperty</span></span>|<span data-ttu-id="6ab5f-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="6ab5f-p106">Die Sammlung erweiterter einwertiger Eigenschaften, die für das contactFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-p106">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ab5f-191">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ab5f-191">JSON representation</span></span>

<span data-ttu-id="6ab5f-192">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ab5f-192">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "wellKnownName": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="6ab5f-193">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="6ab5f-193">See also</span></span>

- [<span data-ttu-id="6ab5f-194">Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten</span><span class="sxs-lookup"><span data-stu-id="6ab5f-194">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="6ab5f-195">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="6ab5f-195">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contactfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
