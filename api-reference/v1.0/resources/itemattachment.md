# <a name="itemattachment-resource-type"></a><span data-ttu-id="882f4-101">itemAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="882f4-101">itemAttachment resource type</span></span>

<span data-ttu-id="882f4-102">Kontakt, Ereignis oder Nachricht, die an ein anderes Ereignis, eine andere Nachricht oder einen anderen Beitrag angefügt sind.</span><span class="sxs-lookup"><span data-stu-id="882f4-102">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="882f4-103">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="882f4-103">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="882f4-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="882f4-104">Methods</span></span>

| <span data-ttu-id="882f4-105">Methode</span><span class="sxs-lookup"><span data-stu-id="882f4-105">Method</span></span>       | <span data-ttu-id="882f4-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="882f4-106">Return Type</span></span>  |<span data-ttu-id="882f4-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="882f4-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="882f4-108">Get</span><span class="sxs-lookup"><span data-stu-id="882f4-108">Get</span></span>](../api/attachment_get.md) | <span data-ttu-id="882f4-109">[itemAttachment](itemattachment.md)</span><span class="sxs-lookup"><span data-stu-id="882f4-109">[itemAttachment](itemattachment.md),</span></span> |<span data-ttu-id="882f4-110">Dient zum Lesen der Eigenschaften und der Beziehungen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="882f4-110">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="882f4-111">Löschen</span><span class="sxs-lookup"><span data-stu-id="882f4-111">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="882f4-112">Keine</span><span class="sxs-lookup"><span data-stu-id="882f4-112">None</span></span> |<span data-ttu-id="882f4-113">Dient zum Löschen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="882f4-113">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="882f4-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="882f4-114">Properties</span></span>
| <span data-ttu-id="882f4-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="882f4-115">Property</span></span>     | <span data-ttu-id="882f4-116">Typ</span><span class="sxs-lookup"><span data-stu-id="882f4-116">Type</span></span>   |<span data-ttu-id="882f4-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="882f4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="882f4-118">contentType</span><span class="sxs-lookup"><span data-stu-id="882f4-118">contentType</span></span>|<span data-ttu-id="882f4-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="882f4-119">String</span></span>|<span data-ttu-id="882f4-120">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="882f4-120">The content type of the attachment.</span></span>|
|<span data-ttu-id="882f4-121">id</span><span class="sxs-lookup"><span data-stu-id="882f4-121">id</span></span>|<span data-ttu-id="882f4-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="882f4-122">String</span></span>| <span data-ttu-id="882f4-123">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="882f4-123">The attachment ID.</span></span>|
|<span data-ttu-id="882f4-124">isInline</span><span class="sxs-lookup"><span data-stu-id="882f4-124">isInline</span></span>|<span data-ttu-id="882f4-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="882f4-125">Boolean</span></span>|<span data-ttu-id="882f4-126">Legen Sie diesen auf „true“ fest, wenn es sich um eine Inlineanlage handelt, z. B. ein eingebettetes Bild innerhalb des Textkörpers des Elements.</span><span class="sxs-lookup"><span data-stu-id="882f4-126">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="882f4-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="882f4-127">lastModifiedDateTime</span></span>|<span data-ttu-id="882f4-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="882f4-128">DateTimeOffset</span></span>|<span data-ttu-id="882f4-129">Letzte Uhrzeit und letztes Datum der Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="882f4-129">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="882f4-130">name</span><span class="sxs-lookup"><span data-stu-id="882f4-130">name</span></span>|<span data-ttu-id="882f4-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="882f4-131">String</span></span>|<span data-ttu-id="882f4-132">Der Anzeigename der Anlage.</span><span class="sxs-lookup"><span data-stu-id="882f4-132">The display name of the attachment.</span></span>|
|<span data-ttu-id="882f4-133">size</span><span class="sxs-lookup"><span data-stu-id="882f4-133">size</span></span>|<span data-ttu-id="882f4-134">Int32</span><span class="sxs-lookup"><span data-stu-id="882f4-134">Int32</span></span>|<span data-ttu-id="882f4-135">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="882f4-135">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="882f4-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="882f4-136">Relationships</span></span>
| <span data-ttu-id="882f4-137">Beziehung</span><span class="sxs-lookup"><span data-stu-id="882f4-137">Relationship</span></span> | <span data-ttu-id="882f4-138">Typ</span><span class="sxs-lookup"><span data-stu-id="882f4-138">Type</span></span>   |<span data-ttu-id="882f4-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="882f4-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="882f4-140">item</span><span class="sxs-lookup"><span data-stu-id="882f4-140">item</span></span>|[<span data-ttu-id="882f4-141">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="882f4-141">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="882f4-p101">Die angefügte Nachricht oder das angefügte Ereignis. Navigation-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="882f4-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="882f4-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="882f4-144">JSON representation</span></span>

<span data-ttu-id="882f4-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="882f4-145">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
