# <a name="itemreference-resource-type"></a><span data-ttu-id="886ec-101">ItemReference-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="886ec-101">ItemReference resource type</span></span>

<span data-ttu-id="886ec-102">Die **ItemReference**-Ressource enthält Informationen, die erforderlich sind, um ein [DriveItem](driveitem.md) über die API zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="886ec-102">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="886ec-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="886ec-103">JSON representation</span></span>

<span data-ttu-id="886ec-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="886ec-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a><span data-ttu-id="886ec-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="886ec-105">Properties</span></span>

| <span data-ttu-id="886ec-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="886ec-106">Property</span></span>      | <span data-ttu-id="886ec-107">Typ</span><span class="sxs-lookup"><span data-stu-id="886ec-107">Type</span></span>                              | <span data-ttu-id="886ec-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="886ec-108">Description</span></span>                                                                                                |
| :------------ | :-------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="886ec-109">driveId</span><span class="sxs-lookup"><span data-stu-id="886ec-109">driveId</span></span>       | <span data-ttu-id="886ec-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="886ec-110">String</span></span>                            | <span data-ttu-id="886ec-p101">Eindeutiger Bezeichner der drive-Instanz, die das Element enthält. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="886ec-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>                                 |
| <span data-ttu-id="886ec-113">id</span><span class="sxs-lookup"><span data-stu-id="886ec-113">id</span></span>            | <span data-ttu-id="886ec-114">String</span><span class="sxs-lookup"><span data-stu-id="886ec-114">String</span></span>                            | <span data-ttu-id="886ec-p102">Eindeutiger Bezeichner des Elements im Laufwerk. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="886ec-p102">Unique identifier of the item in the drive. Read-only.</span></span>                                                     |
| <span data-ttu-id="886ec-117">name</span><span class="sxs-lookup"><span data-stu-id="886ec-117">name</span></span>          | <span data-ttu-id="886ec-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="886ec-118">String</span></span>                            | <span data-ttu-id="886ec-p103">Der Name des Elements, auf das verwiesen wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="886ec-p103">The name of the item being referenced. Read-only.</span></span>                                                          |
| <span data-ttu-id="886ec-121">Pfad</span><span class="sxs-lookup"><span data-stu-id="886ec-121">path</span></span>          | <span data-ttu-id="886ec-122">String</span><span class="sxs-lookup"><span data-stu-id="886ec-122">String</span></span>                            | <span data-ttu-id="886ec-p104">Pfad, der verwendet werden kann, um zu dem Element zu navigieren. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="886ec-p104">Path that can be used to navigate to the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="886ec-125">shareId</span><span class="sxs-lookup"><span data-stu-id="886ec-125">shareId</span></span>       | <span data-ttu-id="886ec-126">String</span><span class="sxs-lookup"><span data-stu-id="886ec-126">String</span></span>                            | <span data-ttu-id="886ec-127">Ein eindeutiger Bezeichner für eine freigegebene Ressource, auf die über [Freigabe](../api/shares_get.md)-API zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="886ec-127">A unique identifier for a shared resource that can be accessed via the [Shares](../api/shares_get.md) API.</span></span> |
| <span data-ttu-id="886ec-128">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="886ec-128">sharepointIds</span></span> | [<span data-ttu-id="886ec-129">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="886ec-129">sharepointIds</span></span>](sharepointids.md) | <span data-ttu-id="886ec-p105">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="886ec-p105">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                   |

## <a name="remarks"></a><span data-ttu-id="886ec-132">HinwBemerkungeneise</span><span class="sxs-lookup"><span data-stu-id="886ec-132">Remarks</span></span>

<span data-ttu-id="886ec-133">Um ein **driveItem**-Element aus einer **itemReference**-Ressource zu adressieren, erstellen Sie eine URL im folgenden Format:</span><span class="sxs-lookup"><span data-stu-id="886ec-133">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="886ec-134">Der **path**-Wert ist ein API-Pfad relativ zu dem Ziellaufwerk, z. B.: `/drive/root:/Documents/myfile.docx`.</span><span class="sxs-lookup"><span data-stu-id="886ec-134">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="886ec-135">Um den lesbaren Pfad für ein Breadcrumb abzurufen, können Sie alles bis zum ersten `:` in der Pfadzeichenfolge problemlos ignorieren.</span><span class="sxs-lookup"><span data-stu-id="886ec-135">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
