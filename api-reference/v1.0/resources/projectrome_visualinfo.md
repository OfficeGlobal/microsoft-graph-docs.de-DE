# <a name="visualinfo-resource-type"></a><span data-ttu-id="9b287-101">Ressourcentyp visualInfo</span><span class="sxs-lookup"><span data-stu-id="9b287-101">visualInfo resource type</span></span>

<span data-ttu-id="9b287-102">Einen komplexen Typ für die Darstellung der **VisualElements** -Eigenschaft im [Aktivität](../resources/projectrome_activity.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="9b287-102">A complex type for representing the **attribution** property in the [visualInfo part of the activity](../resources/projectrome_activity.md) object.</span></span>

<span data-ttu-id="9b287-103">Die Aktivität jedes Benutzers wird in der Zeitachse als eine adaptive Karte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9b287-103">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="9b287-104">App-Entwickler werden ermutigt, eine benutzerdefinierte Karte bereitzustellen, die das Wesentliche der Aktivität in Ihrer App erfasst.</span><span class="sxs-lookup"><span data-stu-id="9b287-104">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="9b287-105">Dies ist möglich, indem Sie eine benutzerdefinierte JSON-Karte in der Inhaltseigenschaft bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="9b287-105">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="9b287-106">Zusätzlich zu visuellen Metadaten mit einer adaptiven Karte kann die App Inhaltsmetadaten angeben - Daten, die verwendet werden, um Rückschlüsse auf die Aktivität des Benutzers zu ziehen, um neue Aktivitäten für eine zukünftige Wiederverwendung anzubieten.</span><span class="sxs-lookup"><span data-stu-id="9b287-106">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="9b287-107">Dies ist möglich, indem Sie mithilfe der Eigenschaft contentInfo der Aktivität ein JSON-Objekt bereitstellen, das schema.org-Eigenschaften zur Beschreibung des Inhalts nutzt.</span><span class="sxs-lookup"><span data-stu-id="9b287-107">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="9b287-108">Wenn keine benutzerdefinierte Karte bereitgestellt wird, wird mit den Eigenschaften Textanzeige und Beschreibung eine einfache Karte generiert.</span><span class="sxs-lookup"><span data-stu-id="9b287-108">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="9b287-109">Benutzerdefinierte Karten werden empfohlen, um die besten Inhalte aus Ihrer App zu präsentieren.</span><span class="sxs-lookup"><span data-stu-id="9b287-109">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="9b287-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9b287-110">Properties</span></span>

|<span data-ttu-id="9b287-111">Name</span><span class="sxs-lookup"><span data-stu-id="9b287-111">Name</span></span> | <span data-ttu-id="9b287-112">Typ</span><span class="sxs-lookup"><span data-stu-id="9b287-112">Type</span></span> | <span data-ttu-id="9b287-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b287-113">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="9b287-114">Anzeigetext</span><span class="sxs-lookup"><span data-stu-id="9b287-114">displayText</span></span> | <span data-ttu-id="9b287-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9b287-115">String</span></span> | <span data-ttu-id="9b287-116">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9b287-116">Required.</span></span> <span data-ttu-id="9b287-117">Kurze Beschreibung der eindeutigen Aktivität des Benutzers (z. B. Dokumentname in Fällen, in denen sich eine Aktivität auf die Dokumenterstellung bezieht)</span><span class="sxs-lookup"><span data-stu-id="9b287-117">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="9b287-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b287-118">description</span></span> | <span data-ttu-id="9b287-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9b287-119">String</span></span> | <span data-ttu-id="9b287-120">Optional.</span><span class="sxs-lookup"><span data-stu-id="9b287-120">Optional.</span></span> <span data-ttu-id="9b287-121">Längere Textbeschreibung der eindeutigen Aktivität des Benutzers (Beispiel: Dokumentname, erster Satz und / oder Metadaten)</span><span class="sxs-lookup"><span data-stu-id="9b287-121">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="9b287-122">Hintergrundfarbe</span><span class="sxs-lookup"><span data-stu-id="9b287-122">background-color</span></span> | <span data-ttu-id="9b287-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9b287-123">String</span></span> | <span data-ttu-id="9b287-124">Optional.</span><span class="sxs-lookup"><span data-stu-id="9b287-124">Optional.</span></span> <span data-ttu-id="9b287-125">Hintergrundfarbe, mit der die Aktivität in der UI - Markenfarbe für die Anwendungsquelle der Aktivität gerendert wird.</span><span class="sxs-lookup"><span data-stu-id="9b287-125">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="9b287-126">Muss eine gültige Hex-Farbe sein</span><span class="sxs-lookup"><span data-stu-id="9b287-126">Must be a valid hex color</span></span>|
|<span data-ttu-id="9b287-127">Inhalt</span><span class="sxs-lookup"><span data-stu-id="9b287-127">content</span></span> | <span data-ttu-id="9b287-128">Nicht typisiertes JSON-Objekt</span><span class="sxs-lookup"><span data-stu-id="9b287-128">Untyped JSON object</span></span> | <span data-ttu-id="9b287-129">Optional.</span><span class="sxs-lookup"><span data-stu-id="9b287-129">Optional.</span></span> <span data-ttu-id="9b287-130">Benutzerdefiniertes Datenelement - JSON-Objekt, das zum Bereitstellen benutzerdefinierter Inhalte zum Rendern der Aktivität in der Windows-Shell-Benutzeroberfläche verwendet wird</span><span class="sxs-lookup"><span data-stu-id="9b287-130">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="9b287-131">Zuschreibung</span><span class="sxs-lookup"><span data-stu-id="9b287-131">attribution</span></span> | <span data-ttu-id="9b287-132">[imageInfo](../resources/projectrome_imageinfo.md)</span><span class="sxs-lookup"><span data-stu-id="9b287-132">Added [imageInfo](../resources/projectrome_imageinfo.md)</span></span> | <span data-ttu-id="9b287-133">Optional.</span><span class="sxs-lookup"><span data-stu-id="9b287-133">Optional.</span></span> <span data-ttu-id="9b287-134">JSON-Objekt zur Darstellung eines Symbols, das die Anwendung darstellt, die zum Generieren der Aktivität verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="9b287-134">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b287-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9b287-135">JSON Representation</span></span>

<span data-ttu-id="9b287-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9b287-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
