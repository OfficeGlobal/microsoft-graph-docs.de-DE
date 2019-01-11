---
title: fileAttachment-Ressourcentyp
description: 'Eine Datei (beispielsweise eine Textdatei oder Word-Dokument), ein Ereignis, Nachricht oder Post zugeordnet ist. Die **contentBytes** '
localization_priority: Priority
ms.openlocfilehash: 81de7a12ca371158d7f6369861a8a197fd544821
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870056"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="7336d-104">fileAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7336d-104">fileAttachment resource type</span></span>

<span data-ttu-id="7336d-p102">Eine Datei (z. B. eine Textdatei oder ein Word-Dokument), die an ein Ereignis, eine Nachricht oder einen Beitrag angefügt ist. Die **contentBytes**-Eigenschaft enthält den base64-codierten Inhalt der Datei.</span><span class="sxs-lookup"><span data-stu-id="7336d-p102">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="7336d-107">Fügen Sie beim Erstellen einer Dateianlage Folgendes zum Anforderungstext hinzu:</span><span class="sxs-lookup"><span data-stu-id="7336d-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="7336d-108">Die erforderlichen Eigenschaften **name** und **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="7336d-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="7336d-109">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="7336d-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7336d-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="7336d-110">Methods</span></span>

| <span data-ttu-id="7336d-111">Methode</span><span class="sxs-lookup"><span data-stu-id="7336d-111">Method</span></span>       | <span data-ttu-id="7336d-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7336d-112">Return Type</span></span>  |<span data-ttu-id="7336d-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7336d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7336d-114">Abrufen</span><span class="sxs-lookup"><span data-stu-id="7336d-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="7336d-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="7336d-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="7336d-116">Dient zum Lesen der Eigenschaften und der Beziehungen des fileAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7336d-116">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="7336d-117">Delete</span><span class="sxs-lookup"><span data-stu-id="7336d-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="7336d-118">Keine</span><span class="sxs-lookup"><span data-stu-id="7336d-118">None</span></span> |<span data-ttu-id="7336d-119">Löscht das fileAttachment-Objekt.</span><span class="sxs-lookup"><span data-stu-id="7336d-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7336d-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7336d-120">Properties</span></span>
| <span data-ttu-id="7336d-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7336d-121">Property</span></span>     | <span data-ttu-id="7336d-122">Typ</span><span class="sxs-lookup"><span data-stu-id="7336d-122">Type</span></span>   |<span data-ttu-id="7336d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7336d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7336d-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="7336d-124">contentBytes</span></span>|<span data-ttu-id="7336d-125">Binär</span><span class="sxs-lookup"><span data-stu-id="7336d-125">Binary</span></span>|<span data-ttu-id="7336d-126">Der base64-codierte Inhalt der Datei.</span><span class="sxs-lookup"><span data-stu-id="7336d-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="7336d-127">contentId</span><span class="sxs-lookup"><span data-stu-id="7336d-127">contentId</span></span>|<span data-ttu-id="7336d-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7336d-128">String</span></span>|<span data-ttu-id="7336d-129">Die ID der Anlage im Exchange-Speicher.</span><span class="sxs-lookup"><span data-stu-id="7336d-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="7336d-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="7336d-130">contentLocation</span></span>|<span data-ttu-id="7336d-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7336d-131">String</span></span>|<span data-ttu-id="7336d-132">Der URI (Uniform Resource Identifier), der dem Speicherort des Anlageninhalts entspricht.</span><span class="sxs-lookup"><span data-stu-id="7336d-132">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="7336d-133">contentType</span><span class="sxs-lookup"><span data-stu-id="7336d-133">contentType</span></span>|<span data-ttu-id="7336d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7336d-134">String</span></span>|<span data-ttu-id="7336d-135">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="7336d-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="7336d-136">id</span><span class="sxs-lookup"><span data-stu-id="7336d-136">id</span></span>|<span data-ttu-id="7336d-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7336d-137">String</span></span>|<span data-ttu-id="7336d-138">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="7336d-138">The attachment ID.</span></span>|
|<span data-ttu-id="7336d-139">isInline</span><span class="sxs-lookup"><span data-stu-id="7336d-139">isInline</span></span>|<span data-ttu-id="7336d-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="7336d-140">Boolean</span></span>|<span data-ttu-id="7336d-141">True, wenn es sich um eine Inlineanlage handelt.</span><span class="sxs-lookup"><span data-stu-id="7336d-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="7336d-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7336d-142">lastModifiedDateTime</span></span>|<span data-ttu-id="7336d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7336d-143">DateTimeOffset</span></span>|<span data-ttu-id="7336d-144">Datum und Uhrzeit der letzten Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="7336d-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="7336d-145">name</span><span class="sxs-lookup"><span data-stu-id="7336d-145">name</span></span>|<span data-ttu-id="7336d-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7336d-146">String</span></span>|<span data-ttu-id="7336d-147">Der Name, der den Text darstellt, der unter dem Symbol für die eingebettete Anlage angezeigt wird. Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="7336d-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="7336d-148">size</span><span class="sxs-lookup"><span data-stu-id="7336d-148">size</span></span>|<span data-ttu-id="7336d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7336d-149">Int32</span></span>|<span data-ttu-id="7336d-150">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="7336d-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7336d-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7336d-151">Relationships</span></span>
<span data-ttu-id="7336d-152">Keine</span><span class="sxs-lookup"><span data-stu-id="7336d-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7336d-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7336d-153">JSON representation</span></span>

<span data-ttu-id="7336d-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7336d-154">Here is a JSON representation of the resource</span></span>

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
