---
title: referenceAttachment-Ressourcentyp
description: 'Einen Link zu einem Ordner oder Datei (beispielsweise eine Textdatei oder Word-Dokument) auf einen OneDrive for Business Cloud Laufwerk oder andere unterstützte Speicherorte, zugeordnet ist '
localization_priority: Normal
ms.openlocfilehash: 59ebb0af10a64195643cb7073d1206790ae6a875
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512710"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="cbde3-103">referenceAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cbde3-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbde3-104">Ein Link zur Datei (beispielsweise eine Textdatei oder Word-Dokument) in eine OneDrive for Business Cloud Laufwerk oder eine andere oder eines Ordners unterstützt Speicherorte, ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md) zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="cbde3-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="cbde3-105">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="cbde3-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cbde3-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="cbde3-106">Methods</span></span>

| <span data-ttu-id="cbde3-107">Methode</span><span class="sxs-lookup"><span data-stu-id="cbde3-107">Method</span></span>       | <span data-ttu-id="cbde3-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cbde3-108">Return Type</span></span>  |<span data-ttu-id="cbde3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbde3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbde3-110">Abrufen</span><span class="sxs-lookup"><span data-stu-id="cbde3-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="cbde3-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="cbde3-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="cbde3-112">Dient zum Lesen der Eigenschaften und der Beziehungen des referenceAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cbde3-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="cbde3-113">Delete</span><span class="sxs-lookup"><span data-stu-id="cbde3-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="cbde3-114">Keine</span><span class="sxs-lookup"><span data-stu-id="cbde3-114">None</span></span> |<span data-ttu-id="cbde3-115">Dient zum Löschen des referenceAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cbde3-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cbde3-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cbde3-116">Properties</span></span>
| <span data-ttu-id="cbde3-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cbde3-117">Property</span></span>     | <span data-ttu-id="cbde3-118">Typ</span><span class="sxs-lookup"><span data-stu-id="cbde3-118">Type</span></span>   |<span data-ttu-id="cbde3-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbde3-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbde3-120">contentType</span><span class="sxs-lookup"><span data-stu-id="cbde3-120">contentType</span></span>|<span data-ttu-id="cbde3-121">String</span><span class="sxs-lookup"><span data-stu-id="cbde3-121">String</span></span>|<span data-ttu-id="cbde3-122">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="cbde3-122">The content type of the attachment.</span></span> <span data-ttu-id="cbde3-123">Optional.</span><span class="sxs-lookup"><span data-stu-id="cbde3-123">Optional.</span></span>|
|<span data-ttu-id="cbde3-124">id</span><span class="sxs-lookup"><span data-stu-id="cbde3-124">id</span></span>|<span data-ttu-id="cbde3-125">String</span><span class="sxs-lookup"><span data-stu-id="cbde3-125">String</span></span>|<span data-ttu-id="cbde3-p102">Die Anlagen-ID.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cbde3-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="cbde3-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="cbde3-128">isFolder</span></span>|<span data-ttu-id="cbde3-129">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cbde3-129">Boolean</span></span>|<span data-ttu-id="cbde3-130">Gibt an, ob die Anlage eine Verknüpfung zu einem Ordner ist.</span><span class="sxs-lookup"><span data-stu-id="cbde3-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="cbde3-131">Setzen Sie müssen diese auf "true" Wenn **SourceUrl** eine Verknüpfung zu einem Ordner ist.</span><span class="sxs-lookup"><span data-stu-id="cbde3-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="cbde3-132">Optional.</span><span class="sxs-lookup"><span data-stu-id="cbde3-132">Optional.</span></span>|
|<span data-ttu-id="cbde3-133">isInline</span><span class="sxs-lookup"><span data-stu-id="cbde3-133">isInline</span></span>|<span data-ttu-id="cbde3-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cbde3-134">Boolean</span></span>|<span data-ttu-id="cbde3-135">Wird auf „true“ festgelegt, wenn die Anlage inline im Text des einbettenden Objekts angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="cbde3-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="cbde3-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="cbde3-136">Optional.</span></span>|
|<span data-ttu-id="cbde3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbde3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cbde3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbde3-138">DateTimeOffset</span></span>|<span data-ttu-id="cbde3-139">Datum und Uhrzeit der letzten Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="cbde3-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="cbde3-140">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="cbde3-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cbde3-141">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cbde3-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cbde3-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="cbde3-142">Optional.</span></span>|
|<span data-ttu-id="cbde3-143">name</span><span class="sxs-lookup"><span data-stu-id="cbde3-143">name</span></span>|<span data-ttu-id="cbde3-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cbde3-144">String</span></span>|<span data-ttu-id="cbde3-145">Der Text, der unterhalb des Symbols, das die eingebettete Anlage darstellt angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="cbde3-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="cbde3-146">Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="cbde3-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="cbde3-147">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cbde3-147">Required.</span></span>|
|<span data-ttu-id="cbde3-148">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="cbde3-148">permission</span></span>|<span data-ttu-id="cbde3-149">ReferenceAttachmentPermissions</span><span class="sxs-lookup"><span data-stu-id="cbde3-149">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="cbde3-150">Gibt die Berechtigungen für die Anlage durch den Typ des Anbieters in **ProviderType**erteilt.</span><span class="sxs-lookup"><span data-stu-id="cbde3-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="cbde3-151">Mögliche Werte sind: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView` und `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="cbde3-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="cbde3-152">Optional.</span><span class="sxs-lookup"><span data-stu-id="cbde3-152">Optional.</span></span>|
|<span data-ttu-id="cbde3-153">Vorschau-URL</span><span class="sxs-lookup"><span data-stu-id="cbde3-153">previewUrl</span></span>|<span data-ttu-id="cbde3-154">String</span><span class="sxs-lookup"><span data-stu-id="cbde3-154">String</span></span>|<span data-ttu-id="cbde3-155">Betrifft nur eine Referenz Anlage ein Bild - URL, um ein Vorschaubild abzurufen.</span><span class="sxs-lookup"><span data-stu-id="cbde3-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="cbde3-156">Verwenden Sie **ThumbnailUrl** und **PreviewUrl** nur, wenn **SourceUrl** eine Bilddatei identifiziert.</span><span class="sxs-lookup"><span data-stu-id="cbde3-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="cbde3-157">Optional.</span><span class="sxs-lookup"><span data-stu-id="cbde3-157">Optional.</span></span>|
|<span data-ttu-id="cbde3-158">providerType</span><span class="sxs-lookup"><span data-stu-id="cbde3-158">providerType</span></span>|<span data-ttu-id="cbde3-159">ReferenceAttachmentProviders</span><span class="sxs-lookup"><span data-stu-id="cbde3-159">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="cbde3-160">Der Typ der Anbieter, der eine Anlage von diesem ContentType unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cbde3-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="cbde3-161">Mögliche Werte: sind `other`, `oneDriveBusiness`, `oneDriveConsumer` und `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="cbde3-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="cbde3-162">Optional.</span><span class="sxs-lookup"><span data-stu-id="cbde3-162">Optional.</span></span>|
|<span data-ttu-id="cbde3-163">size</span><span class="sxs-lookup"><span data-stu-id="cbde3-163">size</span></span>|<span data-ttu-id="cbde3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="cbde3-164">Int32</span></span>|<span data-ttu-id="cbde3-165">Die Größe der Metadaten in Bytes, die für die Nachricht für die Anlage Verweis gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="cbde3-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="cbde3-166">Dieser Wert gibt nicht die Größe der tatsächlichen Datei an.</span><span class="sxs-lookup"><span data-stu-id="cbde3-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="cbde3-167">Optional.</span><span class="sxs-lookup"><span data-stu-id="cbde3-167">Optional.</span></span>|
|<span data-ttu-id="cbde3-168">SourceUrl</span><span class="sxs-lookup"><span data-stu-id="cbde3-168">sourceUrl</span></span>|<span data-ttu-id="cbde3-169">String</span><span class="sxs-lookup"><span data-stu-id="cbde3-169">String</span></span>|<span data-ttu-id="cbde3-170">URL, um den Inhalt der Anlage abzurufen.</span><span class="sxs-lookup"><span data-stu-id="cbde3-170">URL to get the attachment content.</span></span> <span data-ttu-id="cbde3-171">Ist dies eine URL zu einem Ordner, legen Sie dann für den Ordner in Outlook oder Outlook im Web ordnungsgemäß anzuzeigende **IsFolder** auf "true".</span><span class="sxs-lookup"><span data-stu-id="cbde3-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="cbde3-172">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cbde3-172">Required.</span></span>|
|<span data-ttu-id="cbde3-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="cbde3-173">thumbnailUrl</span></span>|<span data-ttu-id="cbde3-174">String</span><span class="sxs-lookup"><span data-stu-id="cbde3-174">String</span></span>|<span data-ttu-id="cbde3-175">Betrifft nur eine Referenz Anlage ein Bild - URL ein Miniaturbild abgerufen.</span><span class="sxs-lookup"><span data-stu-id="cbde3-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="cbde3-176">Verwenden Sie **ThumbnailUrl** und **PreviewUrl** nur, wenn **SourceUrl** eine Bilddatei identifiziert.</span><span class="sxs-lookup"><span data-stu-id="cbde3-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="cbde3-177">Optional.</span><span class="sxs-lookup"><span data-stu-id="cbde3-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbde3-178">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cbde3-178">Relationships</span></span>
<span data-ttu-id="cbde3-179">Keine</span><span class="sxs-lookup"><span data-stu-id="cbde3-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="cbde3-180">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cbde3-180">JSON representation</span></span>

<span data-ttu-id="cbde3-181">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cbde3-181">Here is a JSON representation of the resource</span></span>

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
  "isFolder": true,
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "permission": "string",
  "previewUrl": "string",
  "providerType": "string",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
