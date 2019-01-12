---
title: Ressourcentyp contactFolder
description: Ein Ordner, der Kontakte enthält.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6cf4d6ed75427dce527ced6cb64d0cdcb9afed99
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949045"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="66fdf-103">Ressourcentyp contactFolder</span><span class="sxs-lookup"><span data-stu-id="66fdf-103">contactFolder resource type</span></span>

<span data-ttu-id="66fdf-104">Ein Ordner, der Kontakte enthält.</span><span class="sxs-lookup"><span data-stu-id="66fdf-104">A folder that contains contacts.</span></span>

<span data-ttu-id="66fdf-105">Diese Ressource unterstützt die Verwendung einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen einer [delta](../api/contactfolder-delta.md)-Funktion.</span><span class="sxs-lookup"><span data-stu-id="66fdf-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="66fdf-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="66fdf-106">Methods</span></span>

| <span data-ttu-id="66fdf-107">Methode</span><span class="sxs-lookup"><span data-stu-id="66fdf-107">Method</span></span>       | <span data-ttu-id="66fdf-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="66fdf-108">Return Type</span></span>  |<span data-ttu-id="66fdf-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66fdf-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="66fdf-110">contactFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="66fdf-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="66fdf-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="66fdf-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="66fdf-112">Dient zum Abrufen eines Kontaktordners anhand der Kontaktordner-ID.</span><span class="sxs-lookup"><span data-stu-id="66fdf-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="66fdf-113">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="66fdf-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="66fdf-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="66fdf-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="66fdf-115">Dient zum Aktualisieren des contactFolder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="66fdf-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="66fdf-116">Löschen</span><span class="sxs-lookup"><span data-stu-id="66fdf-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="66fdf-117">Keine</span><span class="sxs-lookup"><span data-stu-id="66fdf-117">None</span></span> |<span data-ttu-id="66fdf-118">Dient zum Löschen des contactFolder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="66fdf-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="66fdf-119">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="66fdf-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="66fdf-120">[ContactFolder](contactfolder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="66fdf-120">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="66fdf-121">Dient zum Abrufen einer Sammlung von untergeordneten Ordnern unter dem angegebenen Kontaktordner.</span><span class="sxs-lookup"><span data-stu-id="66fdf-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="66fdf-122">Untergeordneten contactFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="66fdf-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="66fdf-123">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="66fdf-123">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="66fdf-124">Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners.</span><span class="sxs-lookup"><span data-stu-id="66fdf-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="66fdf-125">delta</span><span class="sxs-lookup"><span data-stu-id="66fdf-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="66fdf-126">[contact](contact.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="66fdf-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="66fdf-127">Dient zum Abrufen eines Satzes von Kontaktordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.</span><span class="sxs-lookup"><span data-stu-id="66fdf-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="66fdf-128">Kontakte im Ordner auflisten</span><span class="sxs-lookup"><span data-stu-id="66fdf-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="66fdf-129">[Contact](contact.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="66fdf-129">[Contact](contact.md) collection</span></span>| <span data-ttu-id="66fdf-130">Dient zum Abrufen einer Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers (`.../me/contacts`) oder aus dem angegebenen Kontaktordner.</span><span class="sxs-lookup"><span data-stu-id="66fdf-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="66fdf-131">Kontakt in Ordner erstellen</span><span class="sxs-lookup"><span data-stu-id="66fdf-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="66fdf-132">Kontakt</span><span class="sxs-lookup"><span data-stu-id="66fdf-132">Contact</span></span>](contact.md)| <span data-ttu-id="66fdf-133">Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.</span><span class="sxs-lookup"><span data-stu-id="66fdf-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="66fdf-134">Create single-value extended property</span><span class="sxs-lookup"><span data-stu-id="66fdf-134">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="66fdf-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="66fdf-135">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="66fdf-136">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen contactFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="66fdf-136">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="66fdf-137">contactFolder mit erweiterter einwertiger Eigenschaft abrufen</span><span class="sxs-lookup"><span data-stu-id="66fdf-137">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="66fdf-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="66fdf-138">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="66fdf-139">Dient zum Abrufen von contactFolders-Elementen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="66fdf-139">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="66fdf-140">Mehrwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="66fdf-140">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="66fdf-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="66fdf-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="66fdf-142">Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen contactFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="66fdf-142">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="66fdf-143">contactFolder mit erweiterter mehrwertiger Eigenschaft abrufen</span><span class="sxs-lookup"><span data-stu-id="66fdf-143">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="66fdf-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="66fdf-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="66fdf-145">Dient zum Abrufen eines contactFolders-Elements mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="66fdf-145">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="66fdf-146">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66fdf-146">Properties</span></span>
| <span data-ttu-id="66fdf-147">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66fdf-147">Property</span></span>     | <span data-ttu-id="66fdf-148">Typ</span><span class="sxs-lookup"><span data-stu-id="66fdf-148">Type</span></span>   |<span data-ttu-id="66fdf-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66fdf-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66fdf-150">displayName</span><span class="sxs-lookup"><span data-stu-id="66fdf-150">displayName</span></span>|<span data-ttu-id="66fdf-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66fdf-151">String</span></span>|<span data-ttu-id="66fdf-152">Der Anzeigename des Ordners.</span><span class="sxs-lookup"><span data-stu-id="66fdf-152">The folder's display name.</span></span>|
|<span data-ttu-id="66fdf-153">id</span><span class="sxs-lookup"><span data-stu-id="66fdf-153">id</span></span>|<span data-ttu-id="66fdf-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66fdf-154">String</span></span>|<span data-ttu-id="66fdf-p101">Eindeutiger Bezeichner des Kontaktordners. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="66fdf-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="66fdf-157">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="66fdf-157">parentFolderId</span></span>|<span data-ttu-id="66fdf-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66fdf-158">String</span></span>|<span data-ttu-id="66fdf-159">Die ID des übergeordneten Ordners des Ordners.</span><span class="sxs-lookup"><span data-stu-id="66fdf-159">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66fdf-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="66fdf-160">Relationships</span></span>
| <span data-ttu-id="66fdf-161">Beziehung</span><span class="sxs-lookup"><span data-stu-id="66fdf-161">Relationship</span></span> | <span data-ttu-id="66fdf-162">Typ</span><span class="sxs-lookup"><span data-stu-id="66fdf-162">Type</span></span>   |<span data-ttu-id="66fdf-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66fdf-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66fdf-164">childFolders</span><span class="sxs-lookup"><span data-stu-id="66fdf-164">childFolders</span></span>|<span data-ttu-id="66fdf-165">[ContactFolder](contactfolder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="66fdf-165">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="66fdf-p102">Die Sammlung der untergeordneten Ordner im Ordner. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="66fdf-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="66fdf-170">Kontakte</span><span class="sxs-lookup"><span data-stu-id="66fdf-170">contacts</span></span>|<span data-ttu-id="66fdf-171">[Contact](contact.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="66fdf-171">[Contact](contact.md) collection</span></span>|<span data-ttu-id="66fdf-p103">Die Kontakte im Ordner. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="66fdf-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="66fdf-176">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="66fdf-176">multiValueExtendedProperties</span></span>|<span data-ttu-id="66fdf-177">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="66fdf-177">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="66fdf-p104">Die Sammlung erweiterter mehrwertiger Eigenschaften, die für das contactFolder-Element definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="66fdf-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="66fdf-181">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="66fdf-181">singleValueExtendedProperties</span></span>|<span data-ttu-id="66fdf-182">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="66fdf-182">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="66fdf-p105">Die Sammlung erweiterter einwertiger Eigenschaften, die für das contactFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="66fdf-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66fdf-186">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66fdf-186">JSON representation</span></span>

<span data-ttu-id="66fdf-187">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66fdf-187">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.contactFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "navigability": "single",
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="66fdf-188">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="66fdf-188">See also</span></span>

- [<span data-ttu-id="66fdf-189">Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten</span><span class="sxs-lookup"><span data-stu-id="66fdf-189">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="66fdf-190">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="66fdf-190">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
