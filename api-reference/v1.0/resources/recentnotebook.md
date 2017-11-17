# <a name="recentnotebook-resource-type"></a><span data-ttu-id="7f050-101">recentNotebook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7f050-101">recentNotebook resource type</span></span>

<span data-ttu-id="7f050-102">Ein OneNote-Notizbuch, auf das kürzlich zugegriffen wurde.</span><span class="sxs-lookup"><span data-stu-id="7f050-102">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="7f050-103">Ein **recentNotebook** ist vergleichbar mit einem [Notizbuch](notebook.md), hat jedoch weniger Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="7f050-103">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="7f050-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7f050-104">Properties</span></span>
| <span data-ttu-id="7f050-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7f050-105">Property</span></span>     | <span data-ttu-id="7f050-106">Typ</span><span class="sxs-lookup"><span data-stu-id="7f050-106">Type</span></span>   |<span data-ttu-id="7f050-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f050-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f050-108">name</span><span class="sxs-lookup"><span data-stu-id="7f050-108">name</span></span>|<span data-ttu-id="7f050-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f050-109">String</span></span>|<span data-ttu-id="7f050-110">Der Name des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="7f050-110">The name of the notebook.</span></span>|
|<span data-ttu-id="7f050-111">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="7f050-111">lastAccessedTime</span></span>|<span data-ttu-id="7f050-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f050-112">DateTimeOffset</span></span>|<span data-ttu-id="7f050-113">Das Datum und die Uhrzeit der letzten Änderung des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="7f050-113">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="7f050-114">Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="7f050-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7f050-115">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7f050-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7f050-116">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7f050-116">Read-only.</span></span>|
|<span data-ttu-id="7f050-117">Links</span><span class="sxs-lookup"><span data-stu-id="7f050-117">links</span></span>|[<span data-ttu-id="7f050-118">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="7f050-118">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="7f050-119">Links zum Öffnen des Notizbuchs.</span><span class="sxs-lookup"><span data-stu-id="7f050-119">Links for opening the notebook.</span></span> <span data-ttu-id="7f050-120">Der Link `oneNoteClientURL` öffnet das Notizbuch im OneNote-Client, sofern er installiert ist.</span><span class="sxs-lookup"><span data-stu-id="7f050-120">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="7f050-121">Der Link `oneNoteWebURL` öffnet das Notizbuch in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="7f050-121">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="7f050-122">sourceService</span><span class="sxs-lookup"><span data-stu-id="7f050-122">sourceService</span></span>|<span data-ttu-id="7f050-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f050-123">String</span></span>|<span data-ttu-id="7f050-124">Der Back-End-Speicher, in dem das Notizbuch gespeichert ist (entweder `OneDriveForBusiness` oder `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="7f050-124">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f050-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7f050-125">JSON representation</span></span>

<span data-ttu-id="7f050-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7f050-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}

```

## <a name="methods"></a><span data-ttu-id="7f050-127">Methoden</span><span class="sxs-lookup"><span data-stu-id="7f050-127">Methods</span></span>

| <span data-ttu-id="7f050-128">Methode</span><span class="sxs-lookup"><span data-stu-id="7f050-128">Method</span></span>           | <span data-ttu-id="7f050-129">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7f050-129">Return Type</span></span>    |<span data-ttu-id="7f050-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f050-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f050-131">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="7f050-131">getRecentNotebooks</span></span>](../api/notebook_getrecentnotebooks.md) | <span data-ttu-id="7f050-132">Sammlung [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="7f050-132">[Notebook](notebook.md) collection</span></span> | <span data-ttu-id="7f050-133">Dient zum Abrufen einer Sammlung der zuletzt geöffneten Notizbücher des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="7f050-133">Get a collection of the most recently accessed notebooks for the user.</span></span> |
