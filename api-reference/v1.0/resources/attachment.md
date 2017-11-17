# <a name="attachment-resource-type"></a><span data-ttu-id="c561a-101">Ressourcentyp attachment</span><span class="sxs-lookup"><span data-stu-id="c561a-101">attachment resource type</span></span>

<span data-ttu-id="c561a-102">Sie können verwandte Inhalte in Form einer Anlage zu einem [Ereignis](../resources/event.md), einer [Nachricht](../resources/message.md) oder einem [Beitrag](../resources/post.md) hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="c561a-102">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="c561a-103">**attachment** ist die Basisressource für die folgenden abgeleiteten Typen von Anlagen:</span><span class="sxs-lookup"><span data-stu-id="c561a-103">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="c561a-104">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="c561a-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="c561a-105">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="c561a-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="c561a-106">Link zu einer Datei ([referenceAttachment](../resources/referenceAttachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="c561a-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="c561a-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="c561a-107">Methods</span></span>

<span data-ttu-id="c561a-108">Die folgenden Methoden gelten für alle abgeleiteten Typen von Anlagen (**fileAttachment**, **itemAttachment** oder **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="c561a-108">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="c561a-109">Methode</span><span class="sxs-lookup"><span data-stu-id="c561a-109">Method</span></span>       | <span data-ttu-id="c561a-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c561a-110">Return Type</span></span>  |<span data-ttu-id="c561a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c561a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c561a-112">Anlage abrufen</span><span class="sxs-lookup"><span data-stu-id="c561a-112">Get attachment</span></span>](../api/attachment_get.md) | [<span data-ttu-id="c561a-113">attachment</span><span class="sxs-lookup"><span data-stu-id="c561a-113">attachment</span></span>](attachment.md) |<span data-ttu-id="c561a-114">Lesen Sie die Eigenschaften und Beziehungen einer Anlage, die einem Ereignis, einer Nachricht oder einem Beitrag angehängt ist.</span><span class="sxs-lookup"><span data-stu-id="c561a-114">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="c561a-115">Anlage einem Ereignis hinzufügen</span><span class="sxs-lookup"><span data-stu-id="c561a-115">Add attachment to an event</span></span>](../api/event_post_attachments.md) | [<span data-ttu-id="c561a-116">attachment</span><span class="sxs-lookup"><span data-stu-id="c561a-116">attachment</span></span>](attachment.md) |<span data-ttu-id="c561a-117">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Ereignis.</span><span class="sxs-lookup"><span data-stu-id="c561a-117">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="c561a-118">Anlagen einer Nachricht hinzufügen</span><span class="sxs-lookup"><span data-stu-id="c561a-118">Add attachment to a message</span></span>](../api/message_post_attachments.md) | [<span data-ttu-id="c561a-119">attachment</span><span class="sxs-lookup"><span data-stu-id="c561a-119">attachment</span></span>](attachment.md) |<span data-ttu-id="c561a-120">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einer Nachricht.</span><span class="sxs-lookup"><span data-stu-id="c561a-120">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="c561a-121">Anlage einem Beitrag hinzufügen</span><span class="sxs-lookup"><span data-stu-id="c561a-121">Add attachment to a post</span></span>](../api/post_post_attachments.md) | [<span data-ttu-id="c561a-122">attachment</span><span class="sxs-lookup"><span data-stu-id="c561a-122">attachment</span></span>](attachment.md) |<span data-ttu-id="c561a-123">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Beitrag.</span><span class="sxs-lookup"><span data-stu-id="c561a-123">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="c561a-124">Anlagen eines Ereignisses auflisten</span><span class="sxs-lookup"><span data-stu-id="c561a-124">List attachments of an event</span></span>](../api/event_list_attachments.md) | <span data-ttu-id="c561a-125">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="c561a-125">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="c561a-126">Liste der Anlagen für ein Ereignis abrufen</span><span class="sxs-lookup"><span data-stu-id="c561a-126">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="c561a-127">Anlagen einer Nachricht auflisten</span><span class="sxs-lookup"><span data-stu-id="c561a-127">List attachments of a message</span></span>](../api/message_list_attachments.md) | <span data-ttu-id="c561a-128">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="c561a-128">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="c561a-129">Liste der Anlagen für eine Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="c561a-129">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="c561a-130">Anlagen eines Beitrags auflisten</span><span class="sxs-lookup"><span data-stu-id="c561a-130">List attachments of a post</span></span>](../api/post_list_attachments.md) | <span data-ttu-id="c561a-131">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="c561a-131">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="c561a-132">Liste der Anlagen für einen Beitrag abrufen</span><span class="sxs-lookup"><span data-stu-id="c561a-132">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="c561a-133">Löschen</span><span class="sxs-lookup"><span data-stu-id="c561a-133">Delete</span></span>](../api/attachment_delete.md) | <span data-ttu-id="c561a-134">Keine</span><span class="sxs-lookup"><span data-stu-id="c561a-134">None</span></span> |<span data-ttu-id="c561a-135">Eine Anlage für ein Ereignis, eine Nachricht oder einen Beitrag löschen</span><span class="sxs-lookup"><span data-stu-id="c561a-135">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="c561a-136">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c561a-136">Properties</span></span>

<span data-ttu-id="c561a-p101">Nachfolgend finden Sie die grundlegenden Eigenschaften von attachment-Ressourcen. Zusätzliche Eigenschaften finden Sie bei dem jeweiligen Anlagentyp ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) oder [referenceAttachment](../resources/referenceAttachment.md)).</span><span class="sxs-lookup"><span data-stu-id="c561a-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceAttachment.md)) for additional properties.</span></span>

| <span data-ttu-id="c561a-139">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c561a-139">Property</span></span>     | <span data-ttu-id="c561a-140">Typ</span><span class="sxs-lookup"><span data-stu-id="c561a-140">Type</span></span>   |<span data-ttu-id="c561a-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c561a-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c561a-142">contentType</span><span class="sxs-lookup"><span data-stu-id="c561a-142">contentType</span></span>|<span data-ttu-id="c561a-143">String</span><span class="sxs-lookup"><span data-stu-id="c561a-143">String</span></span>|<span data-ttu-id="c561a-144">Der MIME-Typ.</span><span class="sxs-lookup"><span data-stu-id="c561a-144">The MIME type.</span></span>|
|<span data-ttu-id="c561a-145">id</span><span class="sxs-lookup"><span data-stu-id="c561a-145">id</span></span>|<span data-ttu-id="c561a-146">String</span><span class="sxs-lookup"><span data-stu-id="c561a-146">String</span></span>| <span data-ttu-id="c561a-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c561a-147">Read-only.</span></span>|
|<span data-ttu-id="c561a-148">isInline</span><span class="sxs-lookup"><span data-stu-id="c561a-148">isInline</span></span>|<span data-ttu-id="c561a-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c561a-149">Boolean</span></span>|<span data-ttu-id="c561a-150">`true`, wenn die Anlage eine Inlineanlage ist, andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="c561a-150">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="c561a-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c561a-151">lastModifiedDateTime</span></span>|<span data-ttu-id="c561a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c561a-152">DateTimeOffset</span></span>|<span data-ttu-id="c561a-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c561a-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c561a-155">name</span><span class="sxs-lookup"><span data-stu-id="c561a-155">name</span></span>|<span data-ttu-id="c561a-156">String</span><span class="sxs-lookup"><span data-stu-id="c561a-156">String</span></span>|<span data-ttu-id="c561a-157">Der Dateiname der Anlage.</span><span class="sxs-lookup"><span data-stu-id="c561a-157">The attachment's file name.</span></span>|
|<span data-ttu-id="c561a-158">size</span><span class="sxs-lookup"><span data-stu-id="c561a-158">size</span></span>|<span data-ttu-id="c561a-159">Int32</span><span class="sxs-lookup"><span data-stu-id="c561a-159">Int32</span></span>|<span data-ttu-id="c561a-160">Die Länge der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="c561a-160">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c561a-161">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c561a-161">Relationships</span></span>
<span data-ttu-id="c561a-162">Keine</span><span class="sxs-lookup"><span data-stu-id="c561a-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c561a-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c561a-163">JSON representation</span></span>

<span data-ttu-id="c561a-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c561a-164">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
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
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
