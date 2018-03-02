# <a name="referenceattachment-resource-type"></a><span data-ttu-id="83a0b-101">referenceAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="83a0b-101">referenceAttachment resource type</span></span>

<span data-ttu-id="83a0b-102">Ein Link zu einer Datei (z. B. eine Textdatei oder ein Word-Dokument) auf einem OneDrive for Business-Cloudlaufwerk oder anderen unterstützten Speicherorten, der an ein Ereignis, eine Nachricht oder einen Beitrag angefügt ist.</span><span class="sxs-lookup"><span data-stu-id="83a0b-102">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="83a0b-103">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="83a0b-103">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="83a0b-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="83a0b-104">Methods</span></span>

| <span data-ttu-id="83a0b-105">Methode</span><span class="sxs-lookup"><span data-stu-id="83a0b-105">Method</span></span>       | <span data-ttu-id="83a0b-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="83a0b-106">Return Type</span></span>  |<span data-ttu-id="83a0b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83a0b-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="83a0b-108">Abrufen</span><span class="sxs-lookup"><span data-stu-id="83a0b-108">Get</span></span>](../api/attachment_get.md) | [<span data-ttu-id="83a0b-109">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="83a0b-109">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="83a0b-110">Dient zum Lesen der Eigenschaften und der Beziehungen des referenceAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="83a0b-110">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="83a0b-111">Delete</span><span class="sxs-lookup"><span data-stu-id="83a0b-111">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="83a0b-112">Keine</span><span class="sxs-lookup"><span data-stu-id="83a0b-112">None</span></span> |<span data-ttu-id="83a0b-113">Dient zum Löschen des referenceAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="83a0b-113">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="83a0b-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="83a0b-114">Properties</span></span>
| <span data-ttu-id="83a0b-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83a0b-115">Property</span></span>     | <span data-ttu-id="83a0b-116">Typ</span><span class="sxs-lookup"><span data-stu-id="83a0b-116">Type</span></span>   |<span data-ttu-id="83a0b-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83a0b-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83a0b-118">contentType</span><span class="sxs-lookup"><span data-stu-id="83a0b-118">contentType</span></span>|<span data-ttu-id="83a0b-119">String</span><span class="sxs-lookup"><span data-stu-id="83a0b-119">String</span></span>|<span data-ttu-id="83a0b-120">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="83a0b-120">The content type of the attachment.</span></span>|
|<span data-ttu-id="83a0b-121">id</span><span class="sxs-lookup"><span data-stu-id="83a0b-121">id</span></span>|<span data-ttu-id="83a0b-122">String</span><span class="sxs-lookup"><span data-stu-id="83a0b-122">String</span></span>|<span data-ttu-id="83a0b-p101">Die Anlagen-ID.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="83a0b-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="83a0b-125">isInline</span><span class="sxs-lookup"><span data-stu-id="83a0b-125">isInline</span></span>|<span data-ttu-id="83a0b-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="83a0b-126">Boolean</span></span>|<span data-ttu-id="83a0b-127">Wird auf „true“ festgelegt, wenn die Anlage inline im Text des einbettenden Objekts angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="83a0b-127">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="83a0b-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83a0b-128">lastModifiedDateTime</span></span>|<span data-ttu-id="83a0b-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83a0b-129">DateTimeOffset</span></span>|<span data-ttu-id="83a0b-p102">Datum und Uhrzeit der letzten Änderung der Anlage. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="83a0b-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="83a0b-133">name</span><span class="sxs-lookup"><span data-stu-id="83a0b-133">name</span></span>|<span data-ttu-id="83a0b-134">String</span><span class="sxs-lookup"><span data-stu-id="83a0b-134">String</span></span>|<span data-ttu-id="83a0b-p103">Der Text, der unter dem Symbol angezeigt wird, das die eingebettete Anlage darstellt. Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="83a0b-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="83a0b-137">size</span><span class="sxs-lookup"><span data-stu-id="83a0b-137">size</span></span>|<span data-ttu-id="83a0b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="83a0b-138">Int32</span></span>|<span data-ttu-id="83a0b-139">Die Größe der Metadaten, die in der Nachricht für die Anlage gespeichert sind, in Byte.</span><span class="sxs-lookup"><span data-stu-id="83a0b-139">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="83a0b-140">Dieser Wert gibt nicht die Größe der tatsächlichen Datei an.</span><span class="sxs-lookup"><span data-stu-id="83a0b-140">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83a0b-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="83a0b-141">Relationships</span></span>
<span data-ttu-id="83a0b-142">Keine</span><span class="sxs-lookup"><span data-stu-id="83a0b-142">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="83a0b-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="83a0b-143">JSON representation</span></span>

<span data-ttu-id="83a0b-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="83a0b-144">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
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
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
