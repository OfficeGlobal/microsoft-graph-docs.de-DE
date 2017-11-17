# <a name="sectiongroup-resource-type"></a><span data-ttu-id="fd497-101">sectionGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fd497-101">sectionGroup resource type</span></span>

<span data-ttu-id="fd497-p101">Eine Abschnittsgruppe in einem OneNote-Notizbuch. Abschnittsgruppen können Abschnitte und Abschnittsgruppen enthalten.</span><span class="sxs-lookup"><span data-stu-id="fd497-p101">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd497-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd497-104">JSON representation</span></span>

<span data-ttu-id="fd497-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd497-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="fd497-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd497-106">Properties</span></span>
| <span data-ttu-id="fd497-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd497-107">Property</span></span>     | <span data-ttu-id="fd497-108">Typ</span><span class="sxs-lookup"><span data-stu-id="fd497-108">Type</span></span>   |<span data-ttu-id="fd497-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd497-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd497-110">createdBy</span><span class="sxs-lookup"><span data-stu-id="fd497-110">createdBy</span></span>|[<span data-ttu-id="fd497-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="fd497-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="fd497-p102">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd497-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="fd497-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd497-114">createdDateTime</span></span>|<span data-ttu-id="fd497-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd497-115">DateTimeOffset</span></span>|<span data-ttu-id="fd497-p103">Das Datum und die Uhrzeit der Erstellung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd497-p103">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="fd497-120">id</span><span class="sxs-lookup"><span data-stu-id="fd497-120">id</span></span>|<span data-ttu-id="fd497-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fd497-121">String</span></span>|<span data-ttu-id="fd497-p104">Der eindeutige Bezeichner der Abschnittsgruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd497-p104">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="fd497-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="fd497-124">lastModifiedBy</span></span>|[<span data-ttu-id="fd497-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="fd497-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="fd497-p105">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd497-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="fd497-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd497-128">lastModifiedDateTime</span></span>|<span data-ttu-id="fd497-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd497-129">DateTimeOffset</span></span>|<span data-ttu-id="fd497-p106">Das Datum und die Uhrzeit der letzten Änderung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd497-p106">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="fd497-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fd497-134">displayName</span></span>|<span data-ttu-id="fd497-135">String</span><span class="sxs-lookup"><span data-stu-id="fd497-135">String</span></span>|<span data-ttu-id="fd497-136">Der Name der Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="fd497-136">The name of the section group.</span></span>|
|<span data-ttu-id="fd497-137">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="fd497-137">sectionGroupsUrl</span></span>|<span data-ttu-id="fd497-138">String</span><span class="sxs-lookup"><span data-stu-id="fd497-138">String</span></span>|<span data-ttu-id="fd497-p107">Die URL für die Navigationseigenschaft `sectionGroups`, die alle Abschnittsgruppen in der Abschnittsgruppe zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd497-p107">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="fd497-141">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="fd497-141">sectionsUrl</span></span>|<span data-ttu-id="fd497-142">String</span><span class="sxs-lookup"><span data-stu-id="fd497-142">String</span></span>|<span data-ttu-id="fd497-p108">Die URL für die Navigationseigenschaft `sections`, die alle Abschnitte in der Abschnittsgruppe zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd497-p108">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="fd497-145">self</span><span class="sxs-lookup"><span data-stu-id="fd497-145">self</span></span>|<span data-ttu-id="fd497-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fd497-146">String</span></span>|<span data-ttu-id="fd497-p109">Der Endpunkt, an dem Sie Details zur Abschnittsgruppe abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd497-p109">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd497-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fd497-149">Relationships</span></span>
| <span data-ttu-id="fd497-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fd497-150">Relationship</span></span> | <span data-ttu-id="fd497-151">Typ</span><span class="sxs-lookup"><span data-stu-id="fd497-151">Type</span></span>   |<span data-ttu-id="fd497-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd497-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd497-153">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="fd497-153">parentNotebook</span></span>|[<span data-ttu-id="fd497-154">Notebook</span><span class="sxs-lookup"><span data-stu-id="fd497-154">Notebook</span></span>](notebook.md)|<span data-ttu-id="fd497-p110">Das Notizbuch, das die Abschnittsgruppe enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd497-p110">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="fd497-157">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="fd497-157">parentSectionGroup</span></span>|[<span data-ttu-id="fd497-158">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="fd497-158">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="fd497-p111">Die Abschnittsgruppe, die die Abschnittsgruppe enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd497-p111">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="fd497-161">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="fd497-161">sectionGroups</span></span>|<span data-ttu-id="fd497-162">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fd497-162">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="fd497-p112">Die Abschnittsgruppen im Abschnitt. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="fd497-p112">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="fd497-166">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="fd497-166">sections</span></span>|<span data-ttu-id="fd497-167">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fd497-167">[Section](section.md) collection</span></span>|<span data-ttu-id="fd497-p113">Die Abschnitte in der Abschnittsgruppe. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="fd497-p113">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="fd497-171">Methoden</span><span class="sxs-lookup"><span data-stu-id="fd497-171">Methods</span></span>

| <span data-ttu-id="fd497-172">Methode</span><span class="sxs-lookup"><span data-stu-id="fd497-172">Method</span></span>           | <span data-ttu-id="fd497-173">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fd497-173">Return Type</span></span>    |<span data-ttu-id="fd497-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd497-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd497-175">Abschnittsgruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="fd497-175">Get section group</span></span>](../api/sectiongroup_get.md) | [<span data-ttu-id="fd497-176">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="fd497-176">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="fd497-177">Dient zum Lesen der Eigenschaften und Beziehungen der Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="fd497-177">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="fd497-178">Abschnittsgruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="fd497-178">Create section group</span></span>](../api/sectiongroup_post_sectiongroups.md) |[<span data-ttu-id="fd497-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="fd497-179">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="fd497-180">Dient zum Erstellen einer Abschnittsgruppe durch Veröffentlichung in der sectionGroups-Sammlung in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="fd497-180">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="fd497-181">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="fd497-181">List section groups</span></span>](../api/sectiongroup_list_sectiongroups.md) |<span data-ttu-id="fd497-182">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fd497-182">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="fd497-183">Dient zum Abrufen der Sammlung von Abschnittsgruppen in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="fd497-183">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="fd497-184">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="fd497-184">Create section</span></span>](../api/sectiongroup_post_sections.md) |[<span data-ttu-id="fd497-185">Section</span><span class="sxs-lookup"><span data-stu-id="fd497-185">Section</span></span>](section.md)| <span data-ttu-id="fd497-186">Dient zum Erstellen eines Abschnitts durch Veröffentlichung in der sections-Sammlung in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="fd497-186">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="fd497-187">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="fd497-187">List sections</span></span>](../api/sectiongroup_list_sections.md) |<span data-ttu-id="fd497-188">[Section](section.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fd497-188">[Section](section.md) collection</span></span>| <span data-ttu-id="fd497-189">Dient zum Abrufen einer Sammlung von Abschnitten in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="fd497-189">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
