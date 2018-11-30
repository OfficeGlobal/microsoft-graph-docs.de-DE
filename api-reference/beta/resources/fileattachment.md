---
title: fileAttachment-Ressourcentyp
description: Eine Datei (beispielsweise eine Textdatei oder Word-Dokument), ein Ereignis zugeordnet ist,
ms.openlocfilehash: 2a43ebbc78d831e907bfd19d647e4b7e398abe90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062339"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="9a53c-103">fileAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9a53c-103">fileAttachment resource type</span></span>

> <span data-ttu-id="9a53c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9a53c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a53c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9a53c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a53c-106">Eine Datei (beispielsweise eine Textdatei oder Word-Dokument), ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md)zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="9a53c-106">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="9a53c-107">Die **ContentBytes** -Eigenschaft enthält die base64-codierten Inhalt der Datei.</span><span class="sxs-lookup"><span data-stu-id="9a53c-107">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="9a53c-108">Fügen Sie beim Erstellen einer Dateianlage Folgendes zum Anforderungstext hinzu:</span><span class="sxs-lookup"><span data-stu-id="9a53c-108">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="9a53c-109">Die erforderlichen Eigenschaften **name** und **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="9a53c-109">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="9a53c-110">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9a53c-110">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9a53c-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="9a53c-111">Methods</span></span>

| <span data-ttu-id="9a53c-112">Methode</span><span class="sxs-lookup"><span data-stu-id="9a53c-112">Method</span></span>       | <span data-ttu-id="9a53c-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9a53c-113">Return Type</span></span>  |<span data-ttu-id="9a53c-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a53c-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a53c-115">Abrufen</span><span class="sxs-lookup"><span data-stu-id="9a53c-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="9a53c-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="9a53c-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="9a53c-117">Dient zum Lesen der Eigenschaften und der Beziehungen des fileAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9a53c-117">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="9a53c-118">Delete</span><span class="sxs-lookup"><span data-stu-id="9a53c-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="9a53c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="9a53c-119">None</span></span> |<span data-ttu-id="9a53c-120">Löscht das fileAttachment-Objekt.</span><span class="sxs-lookup"><span data-stu-id="9a53c-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9a53c-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9a53c-121">Properties</span></span>
| <span data-ttu-id="9a53c-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9a53c-122">Property</span></span>     | <span data-ttu-id="9a53c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="9a53c-123">Type</span></span>   |<span data-ttu-id="9a53c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a53c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a53c-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="9a53c-125">contentBytes</span></span>|<span data-ttu-id="9a53c-126">Binär</span><span class="sxs-lookup"><span data-stu-id="9a53c-126">Binary</span></span>|<span data-ttu-id="9a53c-127">Der base64-codierte Inhalt der Datei.</span><span class="sxs-lookup"><span data-stu-id="9a53c-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="9a53c-128">contentId</span><span class="sxs-lookup"><span data-stu-id="9a53c-128">contentId</span></span>|<span data-ttu-id="9a53c-129">String</span><span class="sxs-lookup"><span data-stu-id="9a53c-129">String</span></span>|<span data-ttu-id="9a53c-130">Die ID der Anlage im Exchange-Speicher.</span><span class="sxs-lookup"><span data-stu-id="9a53c-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="9a53c-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="9a53c-131">contentLocation</span></span>|<span data-ttu-id="9a53c-132">String</span><span class="sxs-lookup"><span data-stu-id="9a53c-132">String</span></span>|<span data-ttu-id="9a53c-133">Der URI (Uniform Resource Identifier), der dem Speicherort des Anlageninhalts entspricht.</span><span class="sxs-lookup"><span data-stu-id="9a53c-133">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="9a53c-134">contentType</span><span class="sxs-lookup"><span data-stu-id="9a53c-134">contentType</span></span>|<span data-ttu-id="9a53c-135">String</span><span class="sxs-lookup"><span data-stu-id="9a53c-135">String</span></span>|<span data-ttu-id="9a53c-136">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="9a53c-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="9a53c-137">id</span><span class="sxs-lookup"><span data-stu-id="9a53c-137">id</span></span>|<span data-ttu-id="9a53c-138">String</span><span class="sxs-lookup"><span data-stu-id="9a53c-138">String</span></span>|<span data-ttu-id="9a53c-139">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="9a53c-139">The attachment ID.</span></span>|
|<span data-ttu-id="9a53c-140">isInline</span><span class="sxs-lookup"><span data-stu-id="9a53c-140">isInline</span></span>|<span data-ttu-id="9a53c-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a53c-141">Boolean</span></span>|<span data-ttu-id="9a53c-142">True, wenn es sich um eine Inlineanlage handelt.</span><span class="sxs-lookup"><span data-stu-id="9a53c-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="9a53c-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a53c-143">lastModifiedDateTime</span></span>|<span data-ttu-id="9a53c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a53c-144">DateTimeOffset</span></span>|<span data-ttu-id="9a53c-145">Datum und Uhrzeit der letzten Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="9a53c-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="9a53c-146">name</span><span class="sxs-lookup"><span data-stu-id="9a53c-146">name</span></span>|<span data-ttu-id="9a53c-147">String</span><span class="sxs-lookup"><span data-stu-id="9a53c-147">String</span></span>|<span data-ttu-id="9a53c-148">Der Name, der den Text darstellt, der unter dem Symbol für die eingebettete Anlage angezeigt wird. Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="9a53c-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="9a53c-149">size</span><span class="sxs-lookup"><span data-stu-id="9a53c-149">size</span></span>|<span data-ttu-id="9a53c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9a53c-150">Int32</span></span>|<span data-ttu-id="9a53c-151">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="9a53c-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a53c-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9a53c-152">Relationships</span></span>
<span data-ttu-id="9a53c-153">Keine</span><span class="sxs-lookup"><span data-stu-id="9a53c-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9a53c-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9a53c-154">JSON representation</span></span>

<span data-ttu-id="9a53c-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9a53c-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
