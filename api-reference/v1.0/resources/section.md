# <a name="section-resource-type"></a><span data-ttu-id="2843e-101">section-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2843e-101">section resource type</span></span>

<span data-ttu-id="2843e-p101">Ein Abschnitt in einem OneNote-Notizbuch. Abschnitte können Seiten enthalten.</span><span class="sxs-lookup"><span data-stu-id="2843e-p101">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2843e-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2843e-104">JSON representation</span></span>

<span data-ttu-id="2843e-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2843e-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="2843e-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2843e-106">Properties</span></span>
| <span data-ttu-id="2843e-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2843e-107">Property</span></span>     | <span data-ttu-id="2843e-108">Typ</span><span class="sxs-lookup"><span data-stu-id="2843e-108">Type</span></span>   |<span data-ttu-id="2843e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2843e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2843e-110">erstellt von</span><span class="sxs-lookup"><span data-stu-id="2843e-110">createdBy</span></span>|[<span data-ttu-id="2843e-111">Identität Set</span><span class="sxs-lookup"><span data-stu-id="2843e-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="2843e-p102">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2843e-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2843e-114">erstelltes Datum und Uhrzeit</span><span class="sxs-lookup"><span data-stu-id="2843e-114">createdDateTime</span></span>|<span data-ttu-id="2843e-115">Datum Uhrzeit Offset</span><span class="sxs-lookup"><span data-stu-id="2843e-115">DateTimeOffset</span></span>|<span data-ttu-id="2843e-p103">Das Datum und die Uhrzeit der Erstellung des Abschnitts. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2843e-p103">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2843e-120">id</span><span class="sxs-lookup"><span data-stu-id="2843e-120">id</span></span>|<span data-ttu-id="2843e-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2843e-121">String</span></span>|<span data-ttu-id="2843e-p104">Der eindeutige Bezeichner des Abschnitts.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2843e-p104">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="2843e-124">ist Standard</span><span class="sxs-lookup"><span data-stu-id="2843e-124">isDefault</span></span>|<span data-ttu-id="2843e-125">Boolesch</span><span class="sxs-lookup"><span data-stu-id="2843e-125">Boolean</span></span>|<span data-ttu-id="2843e-p105">Gibt an, ob dies der Standardabschnitt des Benutzers ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2843e-p105">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="2843e-128">zuletzt geändert durch</span><span class="sxs-lookup"><span data-stu-id="2843e-128">lastModifiedBy</span></span>|[<span data-ttu-id="2843e-129">Identität Set</span><span class="sxs-lookup"><span data-stu-id="2843e-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="2843e-p106">Die Identität des Benutzers, des Geräts und der Anwendung, von der das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2843e-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2843e-132">zuletzt geänderte Datum und Uhrzeit</span><span class="sxs-lookup"><span data-stu-id="2843e-132">lastModifiedDateTime</span></span>|<span data-ttu-id="2843e-133">Datum Uhrzeit Offset</span><span class="sxs-lookup"><span data-stu-id="2843e-133">DateTimeOffset</span></span>|<span data-ttu-id="2843e-p107">Das Datum und die Uhrzeit der letzten Änderung des Abschnitts. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2843e-p107">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2843e-138">links</span><span class="sxs-lookup"><span data-stu-id="2843e-138">links</span></span>|[<span data-ttu-id="2843e-139"> Abschnitt Links</span><span class="sxs-lookup"><span data-stu-id="2843e-139">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="2843e-p108">Links zum Öffnen des Abschnitts. Der Link `oneNoteClientURL` öffnet den Abschnitt im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet den Abschnitt in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="2843e-p108">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="2843e-143">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="2843e-143">displayName</span></span>|<span data-ttu-id="2843e-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2843e-144">String</span></span>|<span data-ttu-id="2843e-145">Der Name des Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="2843e-145">The name of the section.</span></span> |
|<span data-ttu-id="2843e-146">Seiten Url</span><span class="sxs-lookup"><span data-stu-id="2843e-146">pagesUrl</span></span>|<span data-ttu-id="2843e-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2843e-147">String</span></span>|<span data-ttu-id="2843e-p109">Der Endpunkt `pages`, an dem Sie Details für alle Seiten im Abschnitt abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2843e-p109">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="2843e-150">selbst</span><span class="sxs-lookup"><span data-stu-id="2843e-150">self</span></span>|<span data-ttu-id="2843e-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2843e-151">String</span></span>|<span data-ttu-id="2843e-p110">Der Endpunkt, an dem Sie Details zum Abschnitt abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2843e-p110">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2843e-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2843e-154">Relationships</span></span>
| <span data-ttu-id="2843e-155">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2843e-155">Relationship</span></span> | <span data-ttu-id="2843e-156">Typ</span><span class="sxs-lookup"><span data-stu-id="2843e-156">Type</span></span>   |<span data-ttu-id="2843e-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2843e-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2843e-158">seiten</span><span class="sxs-lookup"><span data-stu-id="2843e-158">pages</span></span>|<span data-ttu-id="2843e-159">[OnenoteSeite](page.md) Sammlung</span><span class="sxs-lookup"><span data-stu-id="2843e-159">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="2843e-p111">Die Sammlung von der Seiten im Abschnitt. Schreibgeschützt. Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="2843e-p111">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="2843e-163">Eltern Notizbuch</span><span class="sxs-lookup"><span data-stu-id="2843e-163">parentNotebook</span></span>|[<span data-ttu-id="2843e-164">Notizbuch</span><span class="sxs-lookup"><span data-stu-id="2843e-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="2843e-p112">Das Notizbuch, das den Abschnitt enthält.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2843e-p112">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="2843e-167">Eltern Abschnittsgruppe</span><span class="sxs-lookup"><span data-stu-id="2843e-167">parentSectionGroup</span></span>|[<span data-ttu-id="2843e-168">Abschnittsgruppe</span><span class="sxs-lookup"><span data-stu-id="2843e-168">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="2843e-p113">Die Abschnittsgruppe, die den Abschnitt enthält.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2843e-p113">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="2843e-171">Methoden</span><span class="sxs-lookup"><span data-stu-id="2843e-171">Methods</span></span>

| <span data-ttu-id="2843e-172">Methode</span><span class="sxs-lookup"><span data-stu-id="2843e-172">Method</span></span>           | <span data-ttu-id="2843e-173">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2843e-173">Return Type</span></span>    |<span data-ttu-id="2843e-174">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2843e-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2843e-175">Get Abschnitt</span><span class="sxs-lookup"><span data-stu-id="2843e-175">Get section</span></span>](../api/section_get.md) | [<span data-ttu-id="2843e-176">Onenote Abschnitt</span><span class="sxs-lookup"><span data-stu-id="2843e-176">OnenoteSection</span></span>](section.md) |<span data-ttu-id="2843e-177">Dient zum Lesen der Eigenschaften und Beziehungen des Abschnitts.</span><span class="sxs-lookup"><span data-stu-id="2843e-177">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="2843e-178">Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="2843e-178">Create page</span></span>](../api/section_post_pages.md) |[<span data-ttu-id="2843e-179">Seite</span><span class="sxs-lookup"><span data-stu-id="2843e-179">Page</span></span>](page.md)| <span data-ttu-id="2843e-180">Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung im angegebenen Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="2843e-180">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="2843e-181">Seiten auflisten</span><span class="sxs-lookup"><span data-stu-id="2843e-181">List pages</span></span>](../api/section_list_pages.md) |<span data-ttu-id="2843e-182">[Page](page.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2843e-182">[Page](page.md) collection</span></span>| <span data-ttu-id="2843e-183">Dient zum Abrufen einer Sammlung von Seiten im angegebenen Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="2843e-183">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="2843e-184">In Notizbuch kopieren</span><span class="sxs-lookup"><span data-stu-id="2843e-184">copyToNotebook</span></span>](../api/section_copytonotebook.md)|<span data-ttu-id="2843e-185">Keine</span><span class="sxs-lookup"><span data-stu-id="2843e-185">None</span></span>|<span data-ttu-id="2843e-186">Dient zum Kopieren des Abschnitts in ein bestimmtes Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="2843e-186">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="2843e-187">In Abschnittsgruppe kopieren</span><span class="sxs-lookup"><span data-stu-id="2843e-187">copyToSectionGroup</span></span>](../api/section_copytosectiongroup.md)|<span data-ttu-id="2843e-188">Keine</span><span class="sxs-lookup"><span data-stu-id="2843e-188">None</span></span>|<span data-ttu-id="2843e-189">Dient zum Kopieren des Abschnitts in eine bestimmte Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="2843e-189">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
