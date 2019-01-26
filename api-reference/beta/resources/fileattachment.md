---
title: fileAttachment-Ressourcentyp
description: Eine Datei (beispielsweise eine Textdatei oder Word-Dokument), ein Ereignis zugeordnet ist,
localization_priority: Normal
ms.openlocfilehash: 5f7be9bca3114fc7e74be711dc606a278e0025ff
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572801"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="b7b6e-103">fileAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b7b6e-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b6e-104">Eine Datei (beispielsweise eine Textdatei oder Word-Dokument), ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md)zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="b7b6e-105">Die **ContentBytes** -Eigenschaft enthält die base64-codierten Inhalt der Datei.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="b7b6e-106">Fügen Sie beim Erstellen einer Dateianlage Folgendes zum Anforderungstext hinzu:</span><span class="sxs-lookup"><span data-stu-id="b7b6e-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="b7b6e-107">Die erforderlichen Eigenschaften **name** und **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="b7b6e-108">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b7b6e-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b7b6e-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="b7b6e-109">Methods</span></span>

| <span data-ttu-id="b7b6e-110">Methode</span><span class="sxs-lookup"><span data-stu-id="b7b6e-110">Method</span></span>       | <span data-ttu-id="b7b6e-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b7b6e-111">Return Type</span></span>  |<span data-ttu-id="b7b6e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7b6e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b7b6e-113">Abrufen</span><span class="sxs-lookup"><span data-stu-id="b7b6e-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="b7b6e-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="b7b6e-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="b7b6e-115">Dient zum Lesen der Eigenschaften und der Beziehungen des fileAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="b7b6e-116">Delete</span><span class="sxs-lookup"><span data-stu-id="b7b6e-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="b7b6e-117">Keine</span><span class="sxs-lookup"><span data-stu-id="b7b6e-117">None</span></span> |<span data-ttu-id="b7b6e-118">Löscht das fileAttachment-Objekt.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b7b6e-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b7b6e-119">Properties</span></span>
| <span data-ttu-id="b7b6e-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b7b6e-120">Property</span></span>     | <span data-ttu-id="b7b6e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="b7b6e-121">Type</span></span>   |<span data-ttu-id="b7b6e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7b6e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7b6e-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="b7b6e-123">contentBytes</span></span>|<span data-ttu-id="b7b6e-124">String</span><span class="sxs-lookup"><span data-stu-id="b7b6e-124">String</span></span>|<span data-ttu-id="b7b6e-125">Der base64-codierte Inhalt der Datei.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="b7b6e-126">contentId</span><span class="sxs-lookup"><span data-stu-id="b7b6e-126">contentId</span></span>|<span data-ttu-id="b7b6e-127">String</span><span class="sxs-lookup"><span data-stu-id="b7b6e-127">String</span></span>|<span data-ttu-id="b7b6e-128">Die ID der Anlage im Exchange-Speicher.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="b7b6e-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="b7b6e-129">contentLocation</span></span>|<span data-ttu-id="b7b6e-130">String</span><span class="sxs-lookup"><span data-stu-id="b7b6e-130">String</span></span>|<span data-ttu-id="b7b6e-131">Verwenden Sie diese Eigenschaft nicht auf, da es nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-131">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="b7b6e-132">contentType</span><span class="sxs-lookup"><span data-stu-id="b7b6e-132">contentType</span></span>|<span data-ttu-id="b7b6e-133">String</span><span class="sxs-lookup"><span data-stu-id="b7b6e-133">String</span></span>|<span data-ttu-id="b7b6e-134">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="b7b6e-135">id</span><span class="sxs-lookup"><span data-stu-id="b7b6e-135">id</span></span>|<span data-ttu-id="b7b6e-136">String</span><span class="sxs-lookup"><span data-stu-id="b7b6e-136">String</span></span>|<span data-ttu-id="b7b6e-137">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-137">The attachment ID.</span></span>|
|<span data-ttu-id="b7b6e-138">isInline</span><span class="sxs-lookup"><span data-stu-id="b7b6e-138">isInline</span></span>|<span data-ttu-id="b7b6e-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7b6e-139">Boolean</span></span>|<span data-ttu-id="b7b6e-140">True, wenn es sich um eine Inlineanlage handelt.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="b7b6e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7b6e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b7b6e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7b6e-142">DateTimeOffset</span></span>|<span data-ttu-id="b7b6e-143">Datum und Uhrzeit der letzten Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="b7b6e-144">name</span><span class="sxs-lookup"><span data-stu-id="b7b6e-144">name</span></span>|<span data-ttu-id="b7b6e-145">String</span><span class="sxs-lookup"><span data-stu-id="b7b6e-145">String</span></span>|<span data-ttu-id="b7b6e-146">Der Name, der den Text darstellt, der unter dem Symbol für die eingebettete Anlage angezeigt wird. Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="b7b6e-147">size</span><span class="sxs-lookup"><span data-stu-id="b7b6e-147">size</span></span>|<span data-ttu-id="b7b6e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b7b6e-148">Int32</span></span>|<span data-ttu-id="b7b6e-149">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7b6e-150">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b7b6e-150">Relationships</span></span>
<span data-ttu-id="b7b6e-151">Keine</span><span class="sxs-lookup"><span data-stu-id="b7b6e-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b7b6e-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b7b6e-152">JSON representation</span></span>

<span data-ttu-id="b7b6e-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b7b6e-153">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "String",
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
