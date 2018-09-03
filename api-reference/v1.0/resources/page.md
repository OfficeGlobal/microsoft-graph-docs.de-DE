# <a name="page-resource-type"></a><span data-ttu-id="020a1-101">page-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="020a1-101">page resource type</span></span>

<span data-ttu-id="020a1-102">Eine Seite in einem OneNote-Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="020a1-102">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="020a1-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="020a1-103">JSON representation</span></span>

<span data-ttu-id="020a1-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="020a1-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a><span data-ttu-id="020a1-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="020a1-105">Properties</span></span>
| <span data-ttu-id="020a1-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="020a1-106">Property</span></span>     | <span data-ttu-id="020a1-107">Typ</span><span class="sxs-lookup"><span data-stu-id="020a1-107">Type</span></span>   |<span data-ttu-id="020a1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="020a1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="020a1-109">Inhalt</span><span class="sxs-lookup"><span data-stu-id="020a1-109">content</span></span>|<span data-ttu-id="020a1-110">Stream</span><span class="sxs-lookup"><span data-stu-id="020a1-110">Stream</span></span>|<span data-ttu-id="020a1-111">Der HTML-Inhalt der Seite.</span><span class="sxs-lookup"><span data-stu-id="020a1-111">The page's HTML content.</span></span>|
|<span data-ttu-id="020a1-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="020a1-112">contentUrl</span></span>|<span data-ttu-id="020a1-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="020a1-113">String</span></span>|<span data-ttu-id="020a1-p101">Die URL für die HTML-Inhalt der Seite.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="020a1-116">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="020a1-116">createdByAppId</span></span>|<span data-ttu-id="020a1-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="020a1-117">String</span></span>|<span data-ttu-id="020a1-p102">Der eindeutige Bezeichner der Anwendung, mit der die Seite erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="020a1-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="020a1-120">createdDateTime</span></span>|<span data-ttu-id="020a1-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="020a1-121">DateTimeOffset</span></span>|<span data-ttu-id="020a1-p103">Das Datum und die Uhrzeit der Erstellung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="020a1-126">ID</span><span class="sxs-lookup"><span data-stu-id="020a1-126">id</span></span>|<span data-ttu-id="020a1-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="020a1-127">String</span></span>|<span data-ttu-id="020a1-p104">Der eindeutige Bezeichner der Seite.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="020a1-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="020a1-130">lastModifiedDateTime</span></span>|<span data-ttu-id="020a1-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="020a1-131">DateTimeOffset</span></span>|<span data-ttu-id="020a1-p105">Das Datum und die Uhrzeit der letzten Änderung der Seite. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="020a1-136">Ebene</span><span class="sxs-lookup"><span data-stu-id="020a1-136">level</span></span>|<span data-ttu-id="020a1-137">Int32</span><span class="sxs-lookup"><span data-stu-id="020a1-137">Int32</span></span>|<span data-ttu-id="020a1-p106">Die Einzugsebene der Seite. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="020a1-140">links</span><span class="sxs-lookup"><span data-stu-id="020a1-140">links</span></span>|[<span data-ttu-id="020a1-141">PageLinks</span><span class="sxs-lookup"><span data-stu-id="020a1-141">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="020a1-p107">Links zum Öffnen der Seite. Der Link `oneNoteClientURL` öffnet die Seite im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebUrl` öffnet die Seite in OneNote Online. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="020a1-146">order</span><span class="sxs-lookup"><span data-stu-id="020a1-146">order</span></span>|<span data-ttu-id="020a1-147">Int32</span><span class="sxs-lookup"><span data-stu-id="020a1-147">Int32</span></span>|<span data-ttu-id="020a1-p108">Die Anordnung der Seite im übergeordneten Abschnitt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="020a1-150">self</span><span class="sxs-lookup"><span data-stu-id="020a1-150">self</span></span>|<span data-ttu-id="020a1-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="020a1-151">String</span></span>|<span data-ttu-id="020a1-p109">Der Endpunkt, an dem Sie Details zur Seite abrufen können. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="020a1-154">title</span><span class="sxs-lookup"><span data-stu-id="020a1-154">title</span></span>|<span data-ttu-id="020a1-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="020a1-155">String</span></span>|<span data-ttu-id="020a1-156">Der Titel der Seite.</span><span class="sxs-lookup"><span data-stu-id="020a1-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="020a1-157">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="020a1-157">Relationships</span></span>
| <span data-ttu-id="020a1-158">Beziehung</span><span class="sxs-lookup"><span data-stu-id="020a1-158">Relationship</span></span> | <span data-ttu-id="020a1-159">Typ</span><span class="sxs-lookup"><span data-stu-id="020a1-159">Type</span></span>   |<span data-ttu-id="020a1-160">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="020a1-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="020a1-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="020a1-161">parentNotebook</span></span>|[<span data-ttu-id="020a1-162">Notizbuch</span><span class="sxs-lookup"><span data-stu-id="020a1-162">Notebook</span></span>](notebook.md)|<span data-ttu-id="020a1-p110">Das Notizbuch, das die Seite enthält.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="020a1-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="020a1-165">parentSection</span></span>|[<span data-ttu-id="020a1-166">Onenote Abschnitt</span><span class="sxs-lookup"><span data-stu-id="020a1-166">OnenoteSection</span></span>](section.md)|<span data-ttu-id="020a1-p111">Der Abschnitt, der die Seite enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="020a1-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="020a1-169">Methoden</span><span class="sxs-lookup"><span data-stu-id="020a1-169">Methods</span></span>

| <span data-ttu-id="020a1-170">Methode</span><span class="sxs-lookup"><span data-stu-id="020a1-170">Method</span></span>           | <span data-ttu-id="020a1-171">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="020a1-171">Return Type</span></span>    |<span data-ttu-id="020a1-172">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="020a1-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="020a1-173">Seite abrufen</span><span class="sxs-lookup"><span data-stu-id="020a1-173">Get page</span></span>](../api/page_get.md) | [<span data-ttu-id="020a1-174">Seite</span><span class="sxs-lookup"><span data-stu-id="020a1-174">Page</span></span>](page.md) |<span data-ttu-id="020a1-175">Dient zum Lesen der Eigenschaften und Beziehungen der Seite.</span><span class="sxs-lookup"><span data-stu-id="020a1-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="020a1-176">Seiteninhalt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="020a1-176">Update page content</span></span>](../api/page_update.md) | <span data-ttu-id="020a1-177">Keine</span><span class="sxs-lookup"><span data-stu-id="020a1-177">None</span></span> |<span data-ttu-id="020a1-178">Dient zum Aktualisieren des HTML-Inhalts der Seite.</span><span class="sxs-lookup"><span data-stu-id="020a1-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="020a1-179">Seite löschen</span><span class="sxs-lookup"><span data-stu-id="020a1-179">Delete page</span></span>](../api/page_delete.md) | <span data-ttu-id="020a1-180">Keine</span><span class="sxs-lookup"><span data-stu-id="020a1-180">None</span></span> |<span data-ttu-id="020a1-181">Dient zum Löschen der Seite.</span><span class="sxs-lookup"><span data-stu-id="020a1-181">Delete the page.</span></span> |
|[<span data-ttu-id="020a1-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="020a1-182">copyToSection</span></span>](../api/page_copytosection.md)| <span data-ttu-id="020a1-183">Keine</span><span class="sxs-lookup"><span data-stu-id="020a1-183">None</span></span> |<span data-ttu-id="020a1-184">Kopiert die Seite in einen bestimmten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="020a1-184">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->