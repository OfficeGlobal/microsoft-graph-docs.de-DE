# <a name="fileattachment-resource-type"></a><span data-ttu-id="8f0e4-101">fileAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8f0e4-101">fileAttachment resource type</span></span>

<span data-ttu-id="8f0e4-p101">Eine Datei (z. B. eine Textdatei oder ein Word-Dokument), die an ein Ereignis, eine Nachricht oder einen Beitrag angefügt ist. Die **contentBytes**-Eigenschaft enthält den base64-codierten Inhalt der Datei.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-p101">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="8f0e4-104">Fügen Sie beim Erstellen einer Dateianlage Folgendes zum Anforderungstext hinzu:</span><span class="sxs-lookup"><span data-stu-id="8f0e4-104">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="8f0e4-105">Die erforderlichen Eigenschaften **name** und **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-105">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="8f0e4-106">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="8f0e4-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8f0e4-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="8f0e4-107">Methods</span></span>

| <span data-ttu-id="8f0e4-108">Methode</span><span class="sxs-lookup"><span data-stu-id="8f0e4-108">Method</span></span>       | <span data-ttu-id="8f0e4-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8f0e4-109">Return Type</span></span>  |<span data-ttu-id="8f0e4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f0e4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f0e4-111">Abrufen</span><span class="sxs-lookup"><span data-stu-id="8f0e4-111">Get</span></span>](../api/attachment_get.md) | [<span data-ttu-id="8f0e4-112">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="8f0e4-112">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="8f0e4-113">Dient zum Lesen der Eigenschaften und der Beziehungen des fileAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-113">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="8f0e4-114">Delete</span><span class="sxs-lookup"><span data-stu-id="8f0e4-114">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="8f0e4-115">Keine</span><span class="sxs-lookup"><span data-stu-id="8f0e4-115">None</span></span> |<span data-ttu-id="8f0e4-116">Löscht das fileAttachment-Objekt.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-116">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8f0e4-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f0e4-117">Properties</span></span>
| <span data-ttu-id="8f0e4-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f0e4-118">Property</span></span>     | <span data-ttu-id="8f0e4-119">Typ</span><span class="sxs-lookup"><span data-stu-id="8f0e4-119">Type</span></span>   |<span data-ttu-id="8f0e4-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f0e4-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f0e4-121">contentBytes</span><span class="sxs-lookup"><span data-stu-id="8f0e4-121">contentBytes</span></span>|<span data-ttu-id="8f0e4-122">Binär</span><span class="sxs-lookup"><span data-stu-id="8f0e4-122">Binary</span></span>|<span data-ttu-id="8f0e4-123">Der base64-codierte Inhalt der Datei.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-123">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="8f0e4-124">contentId</span><span class="sxs-lookup"><span data-stu-id="8f0e4-124">contentId</span></span>|<span data-ttu-id="8f0e4-125">String</span><span class="sxs-lookup"><span data-stu-id="8f0e4-125">String</span></span>|<span data-ttu-id="8f0e4-126">Die ID der Anlage im Exchange-Speicher.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-126">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="8f0e4-127">contentLocation</span><span class="sxs-lookup"><span data-stu-id="8f0e4-127">contentLocation</span></span>|<span data-ttu-id="8f0e4-128">String</span><span class="sxs-lookup"><span data-stu-id="8f0e4-128">String</span></span>|<span data-ttu-id="8f0e4-129">Der URI (Uniform Resource Identifier), der dem Speicherort des Anlageninhalts entspricht.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-129">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="8f0e4-130">contentType</span><span class="sxs-lookup"><span data-stu-id="8f0e4-130">contentType</span></span>|<span data-ttu-id="8f0e4-131">String</span><span class="sxs-lookup"><span data-stu-id="8f0e4-131">String</span></span>|<span data-ttu-id="8f0e4-132">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-132">The content type of the attachment.</span></span>|
|<span data-ttu-id="8f0e4-133">id</span><span class="sxs-lookup"><span data-stu-id="8f0e4-133">id</span></span>|<span data-ttu-id="8f0e4-134">String</span><span class="sxs-lookup"><span data-stu-id="8f0e4-134">String</span></span>|<span data-ttu-id="8f0e4-135">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-135">The attachment ID.</span></span>|
|<span data-ttu-id="8f0e4-136">isInline</span><span class="sxs-lookup"><span data-stu-id="8f0e4-136">isInline</span></span>|<span data-ttu-id="8f0e4-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f0e4-137">Boolean</span></span>|<span data-ttu-id="8f0e4-138">True, wenn es sich um eine Inlineanlage handelt.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-138">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="8f0e4-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f0e4-139">lastModifiedDateTime</span></span>|<span data-ttu-id="8f0e4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f0e4-140">DateTimeOffset</span></span>|<span data-ttu-id="8f0e4-141">Datum und Uhrzeit der letzten Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-141">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="8f0e4-142">name</span><span class="sxs-lookup"><span data-stu-id="8f0e4-142">name</span></span>|<span data-ttu-id="8f0e4-143">String</span><span class="sxs-lookup"><span data-stu-id="8f0e4-143">String</span></span>|<span data-ttu-id="8f0e4-144">Der Name, der den Text darstellt, der unter dem Symbol für die eingebettete Anlage angezeigt wird. Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-144">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="8f0e4-145">size</span><span class="sxs-lookup"><span data-stu-id="8f0e4-145">size</span></span>|<span data-ttu-id="8f0e4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8f0e4-146">Int32</span></span>|<span data-ttu-id="8f0e4-147">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-147">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f0e4-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8f0e4-148">Relationships</span></span>
<span data-ttu-id="8f0e4-149">Keine</span><span class="sxs-lookup"><span data-stu-id="8f0e4-149">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f0e4-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f0e4-150">JSON representation</span></span>

<span data-ttu-id="8f0e4-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f0e4-151">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
  "contentId": "string",
  "contentLocation": "string",
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
