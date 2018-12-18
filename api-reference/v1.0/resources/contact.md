---
title: Ressourcentyp contact
description: Ein Kontakt ist ein Element in Outlook, in dem Sie Informationen über die Personen und Organisationen, mit denen Sie kommunizieren, organisieren und speichern können. Kontakte sind in Kontaktordnern enthalten.
author: angelgolfer-ms
ms.openlocfilehash: 13eb3b1e3f88c5018031176cffbcc89a038073ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334972"
---
# <a name="contact-resource-type"></a><span data-ttu-id="78d7d-104">Ressourcentyp contact</span><span class="sxs-lookup"><span data-stu-id="78d7d-104">contact resource type</span></span>

<span data-ttu-id="78d7d-p102">Ein Kontakt ist ein Element in Outlook, in dem Sie Informationen über die Personen und Organisationen, mit denen Sie kommunizieren, organisieren und speichern können. Kontakte sind in Kontaktordnern enthalten.</span><span class="sxs-lookup"><span data-stu-id="78d7d-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="78d7d-107">Diese Ressource unterstützt Folgendes:</span><span class="sxs-lookup"><span data-stu-id="78d7d-107">This resource supports:</span></span>

- <span data-ttu-id="78d7d-108">Hinzufügen von Ihren eigenen Daten zu benutzerdefinierten Eigenschaften als [Extensions](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="78d7d-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="78d7d-109">Abonnieren von [Benachrichtigungen zu ändern](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="78d7d-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="78d7d-110">Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/contact-delta.md)-Funktion.</span><span class="sxs-lookup"><span data-stu-id="78d7d-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="78d7d-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="78d7d-111">Methods</span></span>

| <span data-ttu-id="78d7d-112">Methode</span><span class="sxs-lookup"><span data-stu-id="78d7d-112">Method</span></span>       | <span data-ttu-id="78d7d-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="78d7d-113">Return Type</span></span>  |<span data-ttu-id="78d7d-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78d7d-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="78d7d-115">Kontakt abrufen</span><span class="sxs-lookup"><span data-stu-id="78d7d-115">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="78d7d-116">Kontakt</span><span class="sxs-lookup"><span data-stu-id="78d7d-116">contact</span></span>](contact.md) |<span data-ttu-id="78d7d-117">Dient zum Lesen der Eigenschaften und der Beziehungen des Kontaktobjekts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-117">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="78d7d-118">Erstellen</span><span class="sxs-lookup"><span data-stu-id="78d7d-118">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="78d7d-119">Kontakt</span><span class="sxs-lookup"><span data-stu-id="78d7d-119">contact</span></span>](contact.md) |<span data-ttu-id="78d7d-120">Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Kontaktendpunkt eines anderen Kontaktordners.</span><span class="sxs-lookup"><span data-stu-id="78d7d-120">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="78d7d-121">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="78d7d-121">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="78d7d-122">Kontakt</span><span class="sxs-lookup"><span data-stu-id="78d7d-122">contact</span></span>](contact.md) |<span data-ttu-id="78d7d-123">Dient zum Aktualisieren des Kontaktobjekts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-123">Update contact object.</span></span> |
|[<span data-ttu-id="78d7d-124">Löschen</span><span class="sxs-lookup"><span data-stu-id="78d7d-124">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="78d7d-125">Keine</span><span class="sxs-lookup"><span data-stu-id="78d7d-125">None</span></span> |<span data-ttu-id="78d7d-126">Dient zum Löschen des Kontaktobjekts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-126">Delete contact object.</span></span> |
|[<span data-ttu-id="78d7d-127">delta</span><span class="sxs-lookup"><span data-stu-id="78d7d-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="78d7d-128">[contact](contact.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="78d7d-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="78d7d-129">Dient zum Abrufen eines Satzes von Kontakten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.</span><span class="sxs-lookup"><span data-stu-id="78d7d-129">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="78d7d-130">**Offene Erweiterungen**</span><span class="sxs-lookup"><span data-stu-id="78d7d-130">**Open extensions**</span></span>| | |
|[<span data-ttu-id="78d7d-131">Offene Erweiterung erstellen</span><span class="sxs-lookup"><span data-stu-id="78d7d-131">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="78d7d-132">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="78d7d-132">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="78d7d-133">Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.</span><span class="sxs-lookup"><span data-stu-id="78d7d-133">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="78d7d-134">Offene Erweiterung abrufen</span><span class="sxs-lookup"><span data-stu-id="78d7d-134">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="78d7d-135">[openTypeExtension](opentypeextension.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="78d7d-135">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="78d7d-136">Ruft ein offenes Erweiterungsobjekt oder Objekte basierend auf ihrem Namen oder vollqualifizierten Namen ab.</span><span class="sxs-lookup"><span data-stu-id="78d7d-136">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="78d7d-137">**Schemaerweiterungen**</span><span class="sxs-lookup"><span data-stu-id="78d7d-137">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="78d7d-138">Schemaerweiterungswerte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="78d7d-138">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="78d7d-139">Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.</span><span class="sxs-lookup"><span data-stu-id="78d7d-139">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="78d7d-140">**Erweiterte Eigenschaften**</span><span class="sxs-lookup"><span data-stu-id="78d7d-140">**Extended properties**</span></span>| | |
|[<span data-ttu-id="78d7d-141">Einwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="78d7d-141">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="78d7d-142">Kontakt</span><span class="sxs-lookup"><span data-stu-id="78d7d-142">contact</span></span>](contact.md)  |<span data-ttu-id="78d7d-143">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen Kontakt.</span><span class="sxs-lookup"><span data-stu-id="78d7d-143">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="78d7d-144">Ereignis mit erweiterter einwertiger Eigenschaft abrufen</span><span class="sxs-lookup"><span data-stu-id="78d7d-144">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="78d7d-145">Kontakt</span><span class="sxs-lookup"><span data-stu-id="78d7d-145">contact</span></span>](contact.md) | <span data-ttu-id="78d7d-146">Ruft mithilfe von `$expand` oder `$filter` Kontakte mit einer bestimmten einwertigen erweiterten Eigenschaft ab.</span><span class="sxs-lookup"><span data-stu-id="78d7d-146">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="78d7d-147">Erweiterte mehrwertige Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="78d7d-147">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="78d7d-148">Kontakt</span><span class="sxs-lookup"><span data-stu-id="78d7d-148">contact</span></span>](contact.md) | <span data-ttu-id="78d7d-149">Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen Kontakt.</span><span class="sxs-lookup"><span data-stu-id="78d7d-149">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="78d7d-150">Ereignis mit erweiterter mehrwertiger Eigenschaft abrufen</span><span class="sxs-lookup"><span data-stu-id="78d7d-150">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="78d7d-151">Kontakt</span><span class="sxs-lookup"><span data-stu-id="78d7d-151">contact</span></span>](contact.md) | <span data-ttu-id="78d7d-152">Dient zum Abrufen eines Kontakts mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="78d7d-152">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="78d7d-153">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78d7d-153">Properties</span></span>
| <span data-ttu-id="78d7d-154">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78d7d-154">Property</span></span>     | <span data-ttu-id="78d7d-155">Typ</span><span class="sxs-lookup"><span data-stu-id="78d7d-155">Type</span></span>   |<span data-ttu-id="78d7d-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78d7d-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78d7d-157">assistantName</span><span class="sxs-lookup"><span data-stu-id="78d7d-157">assistantName</span></span>|<span data-ttu-id="78d7d-158">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-158">String</span></span>|<span data-ttu-id="78d7d-159">Der Name des Assistenten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-159">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="78d7d-160">birthday</span><span class="sxs-lookup"><span data-stu-id="78d7d-160">birthday</span></span>|<span data-ttu-id="78d7d-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78d7d-161">DateTimeOffset</span></span>|<span data-ttu-id="78d7d-p103">Das Geburtsdatum des Kontakts. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="78d7d-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="78d7d-165">businessAddress</span><span class="sxs-lookup"><span data-stu-id="78d7d-165">businessAddress</span></span>|[<span data-ttu-id="78d7d-166">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="78d7d-166">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="78d7d-167">Die Geschäftsadresse des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-167">The contact's business address.</span></span>|
|<span data-ttu-id="78d7d-168">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="78d7d-168">businessHomePage</span></span>|<span data-ttu-id="78d7d-169">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-169">String</span></span>|<span data-ttu-id="78d7d-170">Die geschäftliche Homepage des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-170">The business home page of the contact.</span></span>|
|<span data-ttu-id="78d7d-171">businessPhones</span><span class="sxs-lookup"><span data-stu-id="78d7d-171">businessPhones</span></span>|<span data-ttu-id="78d7d-172">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="78d7d-172">String collection</span></span>|<span data-ttu-id="78d7d-173">Die geschäftlichen Telefonnummern des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-173">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="78d7d-174">categories</span><span class="sxs-lookup"><span data-stu-id="78d7d-174">categories</span></span>|<span data-ttu-id="78d7d-175">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="78d7d-175">String collection</span></span>|<span data-ttu-id="78d7d-176">Die Kategorien, die mit dem Kontakt verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="78d7d-176">The categories associated with the contact.</span></span>|
|<span data-ttu-id="78d7d-177">changeKey</span><span class="sxs-lookup"><span data-stu-id="78d7d-177">changeKey</span></span>|<span data-ttu-id="78d7d-178">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-178">String</span></span>|<span data-ttu-id="78d7d-p104">Gibt die Version des Kontakts an. Jedes Mal, wenn der Kontakt geändert wird, wird auch die Eigenschaft „changeKey“ geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.</span><span class="sxs-lookup"><span data-stu-id="78d7d-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="78d7d-182">children</span><span class="sxs-lookup"><span data-stu-id="78d7d-182">children</span></span>|<span data-ttu-id="78d7d-183">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="78d7d-183">String collection</span></span>|<span data-ttu-id="78d7d-184">Die Namen der Kinder des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-184">The names of the contact's children.</span></span>|
|<span data-ttu-id="78d7d-185">companyName</span><span class="sxs-lookup"><span data-stu-id="78d7d-185">companyName</span></span>|<span data-ttu-id="78d7d-186">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-186">String</span></span>|<span data-ttu-id="78d7d-187">Der Name des Unternehmens des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-187">The name of the contact's company.</span></span>|
|<span data-ttu-id="78d7d-188">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78d7d-188">createdDateTime</span></span>|<span data-ttu-id="78d7d-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78d7d-189">DateTimeOffset</span></span>|<span data-ttu-id="78d7d-p105">Der Zeitpunkt, zu dem der Kontakt erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="78d7d-p105">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="78d7d-193">Abteilung</span><span class="sxs-lookup"><span data-stu-id="78d7d-193">department</span></span>|<span data-ttu-id="78d7d-194">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-194">String</span></span>|<span data-ttu-id="78d7d-195">Die Abteilung des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-195">The contact's department.</span></span>|
|<span data-ttu-id="78d7d-196">displayName</span><span class="sxs-lookup"><span data-stu-id="78d7d-196">displayName</span></span>|<span data-ttu-id="78d7d-197">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-197">String</span></span>|<span data-ttu-id="78d7d-198">Der Anzeigename des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-198">The contact's display name.</span></span> <span data-ttu-id="78d7d-199">Sie können den Anzeigenamen in einem Vorgang [Erstellen](../api/user-post-contacts.md) oder [Aktualisieren](../api/contact-update.md) angeben.</span><span class="sxs-lookup"><span data-stu-id="78d7d-199">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="78d7d-200">Beachten Sie, dass es sich bei spätere Aktualisierungen mit anderen Eigenschaften verursachen einen automatisch generierten Wert den Wert DisplayName überschrieben, den Sie angegeben haben.</span><span class="sxs-lookup"><span data-stu-id="78d7d-200">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="78d7d-201">Um einen bereits vorhandenen Wert zu erhalten, immer als schließen Sie DisplayName in einem Vorgang [zu aktualisieren ein](../api/contact-update.md) .</span><span class="sxs-lookup"><span data-stu-id="78d7d-201">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="78d7d-202">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="78d7d-202">emailAddresses</span></span>|<span data-ttu-id="78d7d-203">[EmailAddress](emailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="78d7d-203">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="78d7d-204">Die E-Mail-Adressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-204">The contact's email addresses.</span></span>|
|<span data-ttu-id="78d7d-205">fileAs</span><span class="sxs-lookup"><span data-stu-id="78d7d-205">fileAs</span></span>|<span data-ttu-id="78d7d-206">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-206">String</span></span>|<span data-ttu-id="78d7d-207">Der Name, unter dem der Kontakt abgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="78d7d-207">The name the contact is filed under.</span></span>|
|<span data-ttu-id="78d7d-208">generation</span><span class="sxs-lookup"><span data-stu-id="78d7d-208">generation</span></span>|<span data-ttu-id="78d7d-209">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-209">String</span></span>|<span data-ttu-id="78d7d-210">Die Generation des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-210">The contact's generation.</span></span>|
|<span data-ttu-id="78d7d-211">givenName</span><span class="sxs-lookup"><span data-stu-id="78d7d-211">givenName</span></span>|<span data-ttu-id="78d7d-212">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-212">String</span></span>|<span data-ttu-id="78d7d-213">Der Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-213">The contact's given name.</span></span>|
|<span data-ttu-id="78d7d-214">homeAddress</span><span class="sxs-lookup"><span data-stu-id="78d7d-214">homeAddress</span></span>|[<span data-ttu-id="78d7d-215">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="78d7d-215">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="78d7d-216">Die Privatadresse des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-216">The contact's home address.</span></span>|
|<span data-ttu-id="78d7d-217">homePhones</span><span class="sxs-lookup"><span data-stu-id="78d7d-217">homePhones</span></span>|<span data-ttu-id="78d7d-218">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="78d7d-218">String collection</span></span>|<span data-ttu-id="78d7d-219">Die privaten Telefonnummern des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-219">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="78d7d-220">id</span><span class="sxs-lookup"><span data-stu-id="78d7d-220">id</span></span>|<span data-ttu-id="78d7d-221">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-221">String</span></span>|<span data-ttu-id="78d7d-p107">Eindeutiger Bezeichner für den Kontakt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="78d7d-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="78d7d-224">imAddresses</span><span class="sxs-lookup"><span data-stu-id="78d7d-224">imAddresses</span></span>|<span data-ttu-id="78d7d-225">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="78d7d-225">String collection</span></span>|<span data-ttu-id="78d7d-226">Instant Messaging Chatadressen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-226">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="78d7d-227">initials</span><span class="sxs-lookup"><span data-stu-id="78d7d-227">initials</span></span>|<span data-ttu-id="78d7d-228">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-228">String</span></span>|<span data-ttu-id="78d7d-229">Die Initialen des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-229">The contact's initials.</span></span>|
|<span data-ttu-id="78d7d-230">jobTitle</span><span class="sxs-lookup"><span data-stu-id="78d7d-230">jobTitle</span></span>|<span data-ttu-id="78d7d-231">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-231">String</span></span>|<span data-ttu-id="78d7d-232">Die Position des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-232">The contact’s job title.</span></span>|
|<span data-ttu-id="78d7d-233">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78d7d-233">lastModifiedDateTime</span></span>|<span data-ttu-id="78d7d-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78d7d-234">DateTimeOffset</span></span>|<span data-ttu-id="78d7d-p108">Der Zeitpunkt, zu dem der Kontakt geändert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="78d7d-p108">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="78d7d-238">manager</span><span class="sxs-lookup"><span data-stu-id="78d7d-238">manager</span></span>|<span data-ttu-id="78d7d-239">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-239">String</span></span>|<span data-ttu-id="78d7d-240">Der Name des Vorgesetzten des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-240">The name of the contact's manager.</span></span>
|<span data-ttu-id="78d7d-241">middleName</span><span class="sxs-lookup"><span data-stu-id="78d7d-241">middleName</span></span>|<span data-ttu-id="78d7d-242">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-242">String</span></span>|<span data-ttu-id="78d7d-243">Der zweite Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-243">The contact's middle name.</span></span>|
|<span data-ttu-id="78d7d-244">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="78d7d-244">mobilePhone</span></span>|<span data-ttu-id="78d7d-245">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-245">String</span></span>|<span data-ttu-id="78d7d-246">Die Mobiltelefonnummer des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-246">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="78d7d-247">nickName</span><span class="sxs-lookup"><span data-stu-id="78d7d-247">nickName</span></span>|<span data-ttu-id="78d7d-248">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-248">String</span></span>|<span data-ttu-id="78d7d-249">Der Spitzname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-249">The contact's nickname.</span></span>|
|<span data-ttu-id="78d7d-250">officeLocation</span><span class="sxs-lookup"><span data-stu-id="78d7d-250">officeLocation</span></span>|<span data-ttu-id="78d7d-251">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-251">String</span></span>|<span data-ttu-id="78d7d-252">Der Bürostandort des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-252">The location of the contact's office.</span></span>|
|<span data-ttu-id="78d7d-253">otherAddress</span><span class="sxs-lookup"><span data-stu-id="78d7d-253">otherAddress</span></span>|[<span data-ttu-id="78d7d-254">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="78d7d-254">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="78d7d-255">Weitere Adressen für den Kontakt.</span><span class="sxs-lookup"><span data-stu-id="78d7d-255">Other addresses for the contact.</span></span>|
|<span data-ttu-id="78d7d-256">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="78d7d-256">parentFolderId</span></span>|<span data-ttu-id="78d7d-257">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-257">String</span></span>|<span data-ttu-id="78d7d-258">Die ID des übergeordneten Ordners des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-258">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="78d7d-259">personalNotes</span><span class="sxs-lookup"><span data-stu-id="78d7d-259">personalNotes</span></span>|<span data-ttu-id="78d7d-260">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-260">String</span></span>|<span data-ttu-id="78d7d-261">Die Notizen des Benutzers zu dem Kontakt.</span><span class="sxs-lookup"><span data-stu-id="78d7d-261">The user's notes about the contact.</span></span>|
|<span data-ttu-id="78d7d-262">profession</span><span class="sxs-lookup"><span data-stu-id="78d7d-262">profession</span></span>|<span data-ttu-id="78d7d-263">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-263">String</span></span>|<span data-ttu-id="78d7d-264">Der Beruf des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-264">The contact's profession.</span></span>|
|<span data-ttu-id="78d7d-265">spouseName</span><span class="sxs-lookup"><span data-stu-id="78d7d-265">spouseName</span></span>|<span data-ttu-id="78d7d-266">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="78d7d-266">String</span></span>|<span data-ttu-id="78d7d-267">Der Name des Ehepartners/Partners des Kontakts</span><span class="sxs-lookup"><span data-stu-id="78d7d-267">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="78d7d-268">surname</span><span class="sxs-lookup"><span data-stu-id="78d7d-268">surname</span></span>|<span data-ttu-id="78d7d-269">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-269">String</span></span>|<span data-ttu-id="78d7d-270">Der Nachname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-270">The contact's surname.</span></span>|
|<span data-ttu-id="78d7d-271">title</span><span class="sxs-lookup"><span data-stu-id="78d7d-271">title</span></span>|<span data-ttu-id="78d7d-272">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-272">String</span></span>|<span data-ttu-id="78d7d-273">Der Titel des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-273">The contact's title.</span></span>|
|<span data-ttu-id="78d7d-274">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="78d7d-274">yomiCompanyName</span></span>|<span data-ttu-id="78d7d-275">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-275">String</span></span>|<span data-ttu-id="78d7d-276">Der phonetische japanische Firmenname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-276">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="78d7d-277">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="78d7d-277">yomiGivenName</span></span>|<span data-ttu-id="78d7d-278">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-278">String</span></span>|<span data-ttu-id="78d7d-279">Der phonetische japanische Vorname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-279">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="78d7d-280">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="78d7d-280">yomiSurname</span></span>|<span data-ttu-id="78d7d-281">String</span><span class="sxs-lookup"><span data-stu-id="78d7d-281">String</span></span>|<span data-ttu-id="78d7d-282">Der phonetische japanische Nachname des Kontakts.</span><span class="sxs-lookup"><span data-stu-id="78d7d-282">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78d7d-283">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="78d7d-283">Relationships</span></span>
| <span data-ttu-id="78d7d-284">Beziehung</span><span class="sxs-lookup"><span data-stu-id="78d7d-284">Relationship</span></span> | <span data-ttu-id="78d7d-285">Typ</span><span class="sxs-lookup"><span data-stu-id="78d7d-285">Type</span></span>   |<span data-ttu-id="78d7d-286">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78d7d-286">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78d7d-287">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="78d7d-287">extensions</span></span>|<span data-ttu-id="78d7d-288">[extension](extension.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="78d7d-288">[extension](extension.md) collection</span></span>|<span data-ttu-id="78d7d-p109">Die Sammlung der für den Kontakt definierten offenen Erweiterungen. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="78d7d-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="78d7d-292">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="78d7d-292">multiValueExtendedProperties</span></span>|<span data-ttu-id="78d7d-293">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="78d7d-293">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="78d7d-p110">Die Sammlung erweiterter mehrwertiger Eigenschaften, die für den Kontakt definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="78d7d-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="78d7d-297">Foto</span><span class="sxs-lookup"><span data-stu-id="78d7d-297">photo</span></span>|[<span data-ttu-id="78d7d-298">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="78d7d-298">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="78d7d-p111">Optionales Kontaktbild. Sie können für einen Kontakt ein Foto abrufen oder einstellen.</span><span class="sxs-lookup"><span data-stu-id="78d7d-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="78d7d-301">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="78d7d-301">singleValueExtendedProperties</span></span>|<span data-ttu-id="78d7d-302">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="78d7d-302">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="78d7d-p112">Die Sammlung erweiterter einwertiger Eigenschaften, die für den Kontakt definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="78d7d-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78d7d-306">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="78d7d-306">JSON representation</span></span>

<span data-ttu-id="78d7d-307">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="78d7d-307">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact",
  "@odata.annotations": [
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "businessAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHomePage": "string",
  "businessPhones": ["string"],
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.emailAddress"}],
  "fileAs": "string",
  "generation": "string",
  "givenName": "string",
  "homeAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "homePhones": ["string"],
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "mobilePhone": "string",
  "nickName": "string",
  "officeLocation": "string",
  "otherAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "parentFolderId": "string",
  "personalNotes": "string",
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string",

  "photo": { "@odata.type": "microsoft.graph.profilePhoto" }
}

```

## <a name="see-also"></a><span data-ttu-id="78d7d-308">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="78d7d-308">See also</span></span>

- [<span data-ttu-id="78d7d-309">Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten</span><span class="sxs-lookup"><span data-stu-id="78d7d-309">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="78d7d-310">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="78d7d-310">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="78d7d-311">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="78d7d-311">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="78d7d-312">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="78d7d-312">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="78d7d-313">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="78d7d-313">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
