# <a name="imageinfo-resource-type"></a><span data-ttu-id="0ce8d-101">imageInfo Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0ce8d-101">imageInfo resource type</span></span>

<span data-ttu-id="0ce8d-102">Ein komplexer Typ für die Eigenschaft **Zuweisung** im Teil [visualInfo](../resources/projectrome_visualinfo.md) des Objekts [Aktivität](../resources/projectrome_activity.md).</span><span class="sxs-lookup"><span data-stu-id="0ce8d-102">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome_visualinfo.md) part of the [activity](../resources/projectrome_activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="0ce8d-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0ce8d-103">Properties</span></span>

|<span data-ttu-id="0ce8d-104">Name</span><span class="sxs-lookup"><span data-stu-id="0ce8d-104">Name</span></span> | <span data-ttu-id="0ce8d-105">Typ</span><span class="sxs-lookup"><span data-stu-id="0ce8d-105">Type</span></span> | <span data-ttu-id="0ce8d-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ce8d-106">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="0ce8d-107">iconUrl</span><span class="sxs-lookup"><span data-stu-id="0ce8d-107">iconurl</span></span> | <span data-ttu-id="0ce8d-108">String</span><span class="sxs-lookup"><span data-stu-id="0ce8d-108">String</span></span> | <span data-ttu-id="0ce8d-109">Optional; URI, der auf ein Symbol verweist, das die Anwendung verwendet, um die Aktivität zu generieren</span><span class="sxs-lookup"><span data-stu-id="0ce8d-109">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="0ce8d-110">alternateText</span><span class="sxs-lookup"><span data-stu-id="0ce8d-110">alternateText</span></span> | <span data-ttu-id="0ce8d-111">String</span><span class="sxs-lookup"><span data-stu-id="0ce8d-111">String</span></span> | <span data-ttu-id="0ce8d-112">Optional; alternativer Text-Inhalt für das Bild</span><span class="sxs-lookup"><span data-stu-id="0ce8d-112">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="0ce8d-113">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="0ce8d-113">addImageQuery</span></span> | <span data-ttu-id="0ce8d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ce8d-114">Boolean</span></span> | <span data-ttu-id="0ce8d-115">Optional; Parameter, um anzuzeigen, dass der Server als Reaktion auf Parametrisierung das Bild dynamisch rendern kann.</span><span class="sxs-lookup"><span data-stu-id="0ce8d-115">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="0ce8d-116">Zum Beispiel – ein Bild mit hohem Kontrast</span><span class="sxs-lookup"><span data-stu-id="0ce8d-116">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ce8d-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0ce8d-117">JSON Representation</span></span>

<span data-ttu-id="0ce8d-118">Es folgt eine JSON-Darstellung der Ressource</span><span class="sxs-lookup"><span data-stu-id="0ce8d-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->