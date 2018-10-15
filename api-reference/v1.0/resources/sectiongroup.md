# <a name="sectiongroup-resource-type"></a><span data-ttu-id="82f66-101">sectionGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="82f66-101">sectionGroup resource type</span></span>

<span data-ttu-id="82f66-p101">Eine Abschnittsgruppe in einem OneNote-Notizbuch. Abschnittsgruppen können Abschnitte und Abschnittsgruppen enthalten.</span><span class="sxs-lookup"><span data-stu-id="82f66-p101">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82f66-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="82f66-104">JSON representation</span></span>

<span data-ttu-id="82f66-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="82f66-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectionGroup"
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
## <a name="properties"></a><span data-ttu-id="82f66-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="82f66-106">Properties</span></span>
| <span data-ttu-id="82f66-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="82f66-107">Property</span></span>     | <span data-ttu-id="82f66-108">Typ</span><span class="sxs-lookup"><span data-stu-id="82f66-108">Type</span></span>   |<span data-ttu-id="82f66-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82f66-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82f66-110">createdBy</span><span class="sxs-lookup"><span data-stu-id="82f66-110">createdBy</span></span>|[<span data-ttu-id="82f66-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="82f66-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="82f66-p102">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82f66-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="82f66-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82f66-114">createdDateTime</span></span>|<span data-ttu-id="82f66-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82f66-115">DateTimeOffset</span></span>|<span data-ttu-id="82f66-p103">Das Datum und die Uhrzeit der Erstellung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82f66-p103">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="82f66-120">id</span><span class="sxs-lookup"><span data-stu-id="82f66-120">id</span></span>|<span data-ttu-id="82f66-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82f66-121">String</span></span>|<span data-ttu-id="82f66-p104">Der eindeutige Bezeichner der Abschnittsgruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82f66-p104">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="82f66-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="82f66-124">lastModifiedBy</span></span>|[<span data-ttu-id="82f66-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="82f66-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="82f66-p105">Die Identität des Benutzers, des Geräts und der Anwendung, von der das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82f66-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="82f66-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82f66-128">lastModifiedDateTime</span></span>|<span data-ttu-id="82f66-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82f66-129">DateTimeOffset</span></span>|<span data-ttu-id="82f66-p106">Das Datum und die Uhrzeit der letzten Änderung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82f66-p106">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="82f66-134">displayName</span><span class="sxs-lookup"><span data-stu-id="82f66-134">displayName</span></span>|<span data-ttu-id="82f66-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82f66-135">String</span></span>|<span data-ttu-id="82f66-136">Der Name der Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="82f66-136">The name of the section group.</span></span>|
|<span data-ttu-id="82f66-137">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="82f66-137">sectionGroupsUrl</span></span>|<span data-ttu-id="82f66-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82f66-138">String</span></span>|<span data-ttu-id="82f66-p107">Die URL für die Navigationseigenschaft `sectionGroups`, die alle Abschnittsgruppen in der Abschnittsgruppe zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82f66-p107">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="82f66-141">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="82f66-141">sectionsUrl</span></span>|<span data-ttu-id="82f66-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82f66-142">String</span></span>|<span data-ttu-id="82f66-p108">Die URL für die Navigationseigenschaft `sections`, die alle Abschnitte in der Abschnittsgruppe zurückgibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82f66-p108">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="82f66-145">self</span><span class="sxs-lookup"><span data-stu-id="82f66-145">self</span></span>|<span data-ttu-id="82f66-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="82f66-146">String</span></span>|<span data-ttu-id="82f66-p109">Der Endpunkt, an dem Sie Details zur Abschnittsgruppe abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82f66-p109">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82f66-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="82f66-149">Relationships</span></span>
| <span data-ttu-id="82f66-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="82f66-150">Relationship</span></span> | <span data-ttu-id="82f66-151">Typ</span><span class="sxs-lookup"><span data-stu-id="82f66-151">Type</span></span>   |<span data-ttu-id="82f66-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82f66-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82f66-153">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="82f66-153">parentNotebook</span></span>|[<span data-ttu-id="82f66-154">Notizbuch</span><span class="sxs-lookup"><span data-stu-id="82f66-154">Notebook</span></span>](notebook.md)|<span data-ttu-id="82f66-p110">Das Notizbuch, das die Abschnittsgruppe enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82f66-p110">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="82f66-157">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="82f66-157">parentSectionGroup</span></span>|[<span data-ttu-id="82f66-158">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="82f66-158">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="82f66-p111">Die Abschnittsgruppe, die die Abschnittsgruppe enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82f66-p111">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="82f66-161">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="82f66-161">sectionGroups</span></span>|<span data-ttu-id="82f66-162">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="82f66-162">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="82f66-p112">Die Abschnittsgruppen im Abschnitt. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="82f66-p112">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82f66-166">Abschnitte</span><span class="sxs-lookup"><span data-stu-id="82f66-166">sections</span></span>|<span data-ttu-id="82f66-167">[OnenoteSection](section.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="82f66-167">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="82f66-p113">Die Abschnitte in der Abschnittsgruppe. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="82f66-p113">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="82f66-171">Methoden</span><span class="sxs-lookup"><span data-stu-id="82f66-171">Methods</span></span>

| <span data-ttu-id="82f66-172">Methode</span><span class="sxs-lookup"><span data-stu-id="82f66-172">Method</span></span>           | <span data-ttu-id="82f66-173">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="82f66-173">Return Type</span></span>    |<span data-ttu-id="82f66-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82f66-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82f66-175">Abschnittsgruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="82f66-175">Get section group</span></span>](../api/sectiongroup_get.md) | [<span data-ttu-id="82f66-176">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="82f66-176">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="82f66-177">Dient zum Lesen der Eigenschaften und Beziehungen der Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="82f66-177">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="82f66-178">Abschnittsgruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="82f66-178">Create section group</span></span>](../api/sectiongroup_post_sectiongroups.md) |[<span data-ttu-id="82f66-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="82f66-179">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="82f66-180">Dient zum Erstellen einer Abschnittsgruppe durch Veröffentlichung in der sectionGroups-Sammlung in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="82f66-180">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="82f66-181">Abschnittsgruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="82f66-181">List section groups</span></span>](../api/sectiongroup_list_sectiongroups.md) |<span data-ttu-id="82f66-182">[SectionGroup](sectiongroup.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="82f66-182">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="82f66-183">Dient zum Abrufen der Sammlung von Abschnittsgruppen in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="82f66-183">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="82f66-184">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="82f66-184">Create section</span></span>](../api/sectiongroup_post_sections.md) |[<span data-ttu-id="82f66-185">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="82f66-185">OnenoteSection</span></span>](section.md)| <span data-ttu-id="82f66-186">Dient zum Erstellen eines Abschnitts durch Veröffentlichung in der Abschnitts-Sammlung in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="82f66-186">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="82f66-187">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="82f66-187">List sections</span></span>](../api/sectiongroup_list_sections.md) |<span data-ttu-id="82f66-188">[OnenoteSection](section.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="82f66-188">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="82f66-189">Dient zum Abrufen einer Sammlung von Abschnitten in der angegebenen Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="82f66-189">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
