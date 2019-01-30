---
title: fileAttachment-Ressourcentyp
description: Eine Datei (beispielsweise eine Textdatei oder Word-Dokument), ein Ereignis zugeordnet ist,
localization_priority: Normal
ms.openlocfilehash: 7d9f92565e38aaf418691480b7f8f3187c57647c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644091"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="956f2-103">fileAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="956f2-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="956f2-104">Eine Datei (beispielsweise eine Textdatei oder Word-Dokument), ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md)zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="956f2-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="956f2-105">Die **ContentBytes** -Eigenschaft enthält die base64-codierten Inhalt der Datei.</span><span class="sxs-lookup"><span data-stu-id="956f2-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="956f2-106">Fügen Sie beim Erstellen einer Dateianlage Folgendes zum Anforderungstext hinzu:</span><span class="sxs-lookup"><span data-stu-id="956f2-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="956f2-107">Die erforderlichen Eigenschaften **name** und **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="956f2-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="956f2-108">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="956f2-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="956f2-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="956f2-109">Methods</span></span>

| <span data-ttu-id="956f2-110">Methode</span><span class="sxs-lookup"><span data-stu-id="956f2-110">Method</span></span>       | <span data-ttu-id="956f2-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="956f2-111">Return Type</span></span>  |<span data-ttu-id="956f2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="956f2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="956f2-113">Abrufen</span><span class="sxs-lookup"><span data-stu-id="956f2-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="956f2-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="956f2-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="956f2-115">Dient zum Lesen der Eigenschaften und der Beziehungen des fileAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="956f2-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="956f2-116">Delete</span><span class="sxs-lookup"><span data-stu-id="956f2-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="956f2-117">Keine</span><span class="sxs-lookup"><span data-stu-id="956f2-117">None</span></span> |<span data-ttu-id="956f2-118">Löscht das fileAttachment-Objekt.</span><span class="sxs-lookup"><span data-stu-id="956f2-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="956f2-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="956f2-119">Properties</span></span>
| <span data-ttu-id="956f2-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="956f2-120">Property</span></span>     | <span data-ttu-id="956f2-121">Typ</span><span class="sxs-lookup"><span data-stu-id="956f2-121">Type</span></span>   |<span data-ttu-id="956f2-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="956f2-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="956f2-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="956f2-123">contentBytes</span></span>|<span data-ttu-id="956f2-124">Binär</span><span class="sxs-lookup"><span data-stu-id="956f2-124">Binary</span></span>|<span data-ttu-id="956f2-125">Der base64-codierte Inhalt der Datei.</span><span class="sxs-lookup"><span data-stu-id="956f2-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="956f2-126">contentId</span><span class="sxs-lookup"><span data-stu-id="956f2-126">contentId</span></span>|<span data-ttu-id="956f2-127">String</span><span class="sxs-lookup"><span data-stu-id="956f2-127">String</span></span>|<span data-ttu-id="956f2-128">Die ID der Anlage im Exchange-Speicher.</span><span class="sxs-lookup"><span data-stu-id="956f2-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="956f2-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="956f2-129">contentLocation</span></span>|<span data-ttu-id="956f2-130">String</span><span class="sxs-lookup"><span data-stu-id="956f2-130">String</span></span>|<span data-ttu-id="956f2-131">Verwenden Sie diese Eigenschaft nicht, weil sie nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="956f2-131">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="956f2-132">contentType</span><span class="sxs-lookup"><span data-stu-id="956f2-132">contentType</span></span>|<span data-ttu-id="956f2-133">String</span><span class="sxs-lookup"><span data-stu-id="956f2-133">String</span></span>|<span data-ttu-id="956f2-134">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="956f2-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="956f2-135">id</span><span class="sxs-lookup"><span data-stu-id="956f2-135">id</span></span>|<span data-ttu-id="956f2-136">String</span><span class="sxs-lookup"><span data-stu-id="956f2-136">String</span></span>|<span data-ttu-id="956f2-137">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="956f2-137">The attachment ID.</span></span>|
|<span data-ttu-id="956f2-138">isInline</span><span class="sxs-lookup"><span data-stu-id="956f2-138">isInline</span></span>|<span data-ttu-id="956f2-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="956f2-139">Boolean</span></span>|<span data-ttu-id="956f2-140">True, wenn es sich um eine Inlineanlage handelt.</span><span class="sxs-lookup"><span data-stu-id="956f2-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="956f2-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="956f2-141">lastModifiedDateTime</span></span>|<span data-ttu-id="956f2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="956f2-142">DateTimeOffset</span></span>|<span data-ttu-id="956f2-143">Datum und Uhrzeit der letzten Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="956f2-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="956f2-144">name</span><span class="sxs-lookup"><span data-stu-id="956f2-144">name</span></span>|<span data-ttu-id="956f2-145">String</span><span class="sxs-lookup"><span data-stu-id="956f2-145">String</span></span>|<span data-ttu-id="956f2-146">Der Name, der den Text darstellt, der unter dem Symbol für die eingebettete Anlage angezeigt wird. Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="956f2-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="956f2-147">size</span><span class="sxs-lookup"><span data-stu-id="956f2-147">size</span></span>|<span data-ttu-id="956f2-148">Int32</span><span class="sxs-lookup"><span data-stu-id="956f2-148">Int32</span></span>|<span data-ttu-id="956f2-149">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="956f2-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="956f2-150">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="956f2-150">Relationships</span></span>
<span data-ttu-id="956f2-151">Keine</span><span class="sxs-lookup"><span data-stu-id="956f2-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="956f2-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="956f2-152">JSON representation</span></span>

<span data-ttu-id="956f2-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="956f2-153">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/fileattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
