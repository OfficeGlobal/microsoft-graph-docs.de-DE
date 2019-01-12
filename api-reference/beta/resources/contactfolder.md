---
title: Ressourcentyp contactFolder
description: Ein Ordner, der Kontakte enthält.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 450c683d91eeb789c8c54b2bbfd38db695fbbba2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967546"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="48c2c-103">Ressourcentyp contactFolder</span><span class="sxs-lookup"><span data-stu-id="48c2c-103">contactFolder resource type</span></span>

> <span data-ttu-id="48c2c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="48c2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48c2c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48c2c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48c2c-106">Ein Ordner, der Kontakte enthält.</span><span class="sxs-lookup"><span data-stu-id="48c2c-106">A folder that contains contacts.</span></span>

<span data-ttu-id="48c2c-107">Diese Ressource unterstützt die Verwendung einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen einer [delta](../api/contactfolder-delta.md)-Funktion.</span><span class="sxs-lookup"><span data-stu-id="48c2c-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="48c2c-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="48c2c-108">Methods</span></span>

| <span data-ttu-id="48c2c-109">Methode</span><span class="sxs-lookup"><span data-stu-id="48c2c-109">Method</span></span>       | <span data-ttu-id="48c2c-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="48c2c-110">Return Type</span></span>  |<span data-ttu-id="48c2c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48c2c-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48c2c-112">contactFolder abrufen</span><span class="sxs-lookup"><span data-stu-id="48c2c-112">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="48c2c-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="48c2c-113">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="48c2c-114">Dient zum Abrufen eines Kontaktordners anhand der Kontaktordner-ID.</span><span class="sxs-lookup"><span data-stu-id="48c2c-114">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="48c2c-115">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="48c2c-115">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="48c2c-116">contactFolder</span><span class="sxs-lookup"><span data-stu-id="48c2c-116">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="48c2c-117">Dient zum Aktualisieren des contactFolder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="48c2c-117">Update contactFolder object.</span></span> |
|[<span data-ttu-id="48c2c-118">Löschen</span><span class="sxs-lookup"><span data-stu-id="48c2c-118">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="48c2c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="48c2c-119">None</span></span> |<span data-ttu-id="48c2c-120">Dient zum Löschen des contactFolder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="48c2c-120">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="48c2c-121">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="48c2c-121">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="48c2c-122">[ContactFolder](contactfolder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="48c2c-122">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="48c2c-123">Dient zum Abrufen einer Sammlung von untergeordneten Ordnern unter dem angegebenen Kontaktordner.</span><span class="sxs-lookup"><span data-stu-id="48c2c-123">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="48c2c-124">Untergeordneten contactFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="48c2c-124">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="48c2c-125">contactFolder</span><span class="sxs-lookup"><span data-stu-id="48c2c-125">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="48c2c-126">Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners.</span><span class="sxs-lookup"><span data-stu-id="48c2c-126">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="48c2c-127">delta</span><span class="sxs-lookup"><span data-stu-id="48c2c-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="48c2c-128">[contact](contact.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="48c2c-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="48c2c-129">Dient zum Abrufen eines Satzes von Kontaktordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.</span><span class="sxs-lookup"><span data-stu-id="48c2c-129">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="48c2c-130">Kontakte im Ordner auflisten</span><span class="sxs-lookup"><span data-stu-id="48c2c-130">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="48c2c-131">[contact](contact.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="48c2c-131">[contact](contact.md) collection</span></span>| <span data-ttu-id="48c2c-132">Dient zum Abrufen einer Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers (`.../me/contacts`) oder aus dem angegebenen Kontaktordner.</span><span class="sxs-lookup"><span data-stu-id="48c2c-132">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="48c2c-133">Kontakt in Ordner erstellen</span><span class="sxs-lookup"><span data-stu-id="48c2c-133">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="48c2c-134">Kontakt</span><span class="sxs-lookup"><span data-stu-id="48c2c-134">contact</span></span>](contact.md)| <span data-ttu-id="48c2c-135">Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.</span><span class="sxs-lookup"><span data-stu-id="48c2c-135">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="48c2c-136">**Erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="48c2c-136">**Extended properties**</span></span>| | |
|[<span data-ttu-id="48c2c-137">Create single-value extended property</span><span class="sxs-lookup"><span data-stu-id="48c2c-137">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="48c2c-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="48c2c-138">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="48c2c-139">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen contactFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="48c2c-139">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="48c2c-140">contactFolder mit erweiterter einwertiger Eigenschaft abrufen</span><span class="sxs-lookup"><span data-stu-id="48c2c-140">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="48c2c-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="48c2c-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="48c2c-142">Dient zum Abrufen von contactFolders-Elementen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`.</span><span class="sxs-lookup"><span data-stu-id="48c2c-142">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="48c2c-143">Mehrwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="48c2c-143">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="48c2c-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="48c2c-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="48c2c-145">Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen contactFolder-Element.</span><span class="sxs-lookup"><span data-stu-id="48c2c-145">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="48c2c-146">contactFolder mit erweiterter mehrwertiger Eigenschaft abrufen</span><span class="sxs-lookup"><span data-stu-id="48c2c-146">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="48c2c-147">contactFolder</span><span class="sxs-lookup"><span data-stu-id="48c2c-147">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="48c2c-148">Dient zum Abrufen eines contactFolders-Elements mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="48c2c-148">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="48c2c-149">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="48c2c-149">Properties</span></span>
| <span data-ttu-id="48c2c-150">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="48c2c-150">Property</span></span>     | <span data-ttu-id="48c2c-151">Typ</span><span class="sxs-lookup"><span data-stu-id="48c2c-151">Type</span></span>   |<span data-ttu-id="48c2c-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48c2c-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48c2c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="48c2c-153">displayName</span></span>|<span data-ttu-id="48c2c-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48c2c-154">String</span></span>|<span data-ttu-id="48c2c-155">Der Anzeigename des Ordners.</span><span class="sxs-lookup"><span data-stu-id="48c2c-155">The folder's display name.</span></span>|
|<span data-ttu-id="48c2c-156">id</span><span class="sxs-lookup"><span data-stu-id="48c2c-156">id</span></span>|<span data-ttu-id="48c2c-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48c2c-157">String</span></span>|<span data-ttu-id="48c2c-p102">Eindeutiger Bezeichner des Kontaktordners. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="48c2c-p102">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="48c2c-160">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="48c2c-160">parentFolderId</span></span>|<span data-ttu-id="48c2c-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48c2c-161">String</span></span>|<span data-ttu-id="48c2c-162">Die ID des übergeordneten Ordners des Ordners.</span><span class="sxs-lookup"><span data-stu-id="48c2c-162">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="48c2c-163">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="48c2c-163">wellKnownName</span></span>|<span data-ttu-id="48c2c-164">string</span><span class="sxs-lookup"><span data-stu-id="48c2c-164">string</span></span>|<span data-ttu-id="48c2c-165">Der Name des Ordners, wenn der Ordner einen erkannten Ordner ist.</span><span class="sxs-lookup"><span data-stu-id="48c2c-165">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="48c2c-166">Derzeit `contacts` ist die einzige erkannten Kontakteordner.</span><span class="sxs-lookup"><span data-stu-id="48c2c-166">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48c2c-167">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="48c2c-167">Relationships</span></span>
| <span data-ttu-id="48c2c-168">Beziehung</span><span class="sxs-lookup"><span data-stu-id="48c2c-168">Relationship</span></span> | <span data-ttu-id="48c2c-169">Typ</span><span class="sxs-lookup"><span data-stu-id="48c2c-169">Type</span></span>   |<span data-ttu-id="48c2c-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48c2c-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48c2c-171">childFolders</span><span class="sxs-lookup"><span data-stu-id="48c2c-171">childFolders</span></span>|<span data-ttu-id="48c2c-172">[ContactFolder](contactfolder.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="48c2c-172">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="48c2c-p104">Die Sammlung der untergeordneten Ordner im Ordner. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="48c2c-p104">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="48c2c-177">Kontakte</span><span class="sxs-lookup"><span data-stu-id="48c2c-177">contacts</span></span>|<span data-ttu-id="48c2c-178">[Contact](contact.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="48c2c-178">[Contact](contact.md) collection</span></span>|<span data-ttu-id="48c2c-p105">Die Kontakte im Ordner. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="48c2c-p105">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="48c2c-183">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="48c2c-183">multiValueExtendedProperties</span></span>|<span data-ttu-id="48c2c-184">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="48c2c-184">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="48c2c-p106">Die Sammlung erweiterter mehrwertiger Eigenschaften, die für das contactFolder-Element definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="48c2c-p106">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="48c2c-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="48c2c-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="48c2c-189">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="48c2c-189">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="48c2c-p107">Die Sammlung erweiterter einwertiger Eigenschaften, die für das contactFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="48c2c-p107">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48c2c-193">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="48c2c-193">JSON representation</span></span>

<span data-ttu-id="48c2c-194">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="48c2c-194">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
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

## <a name="see-also"></a><span data-ttu-id="48c2c-195">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="48c2c-195">See also</span></span>

- [<span data-ttu-id="48c2c-196">Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten</span><span class="sxs-lookup"><span data-stu-id="48c2c-196">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="48c2c-197">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="48c2c-197">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
