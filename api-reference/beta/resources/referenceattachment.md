---
title: referenceAttachment-Ressourcentyp
description: 'Einen Link zu einem Ordner oder Datei (beispielsweise eine Textdatei oder Word-Dokument) auf einen OneDrive for Business Cloud Laufwerk oder andere unterstützte Speicherorte, zugeordnet ist '
ms.openlocfilehash: e9885c3a0e5c7f723303d7d6461f4c07dbed6bf6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063918"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="9f6e9-103">referenceAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9f6e9-103">referenceAttachment resource type</span></span>

> <span data-ttu-id="9f6e9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f6e9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f6e9-106">Ein Link zur Datei (beispielsweise eine Textdatei oder Word-Dokument) in eine OneDrive for Business Cloud Laufwerk oder eine andere oder eines Ordners unterstützt Speicherorte, ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md) zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-106">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="9f6e9-107">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9f6e9-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9f6e9-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="9f6e9-108">Methods</span></span>

| <span data-ttu-id="9f6e9-109">Methode</span><span class="sxs-lookup"><span data-stu-id="9f6e9-109">Method</span></span>       | <span data-ttu-id="9f6e9-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9f6e9-110">Return Type</span></span>  |<span data-ttu-id="9f6e9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f6e9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f6e9-112">Abrufen</span><span class="sxs-lookup"><span data-stu-id="9f6e9-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="9f6e9-113">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="9f6e9-113">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="9f6e9-114">Dient zum Lesen der Eigenschaften und der Beziehungen des referenceAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-114">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="9f6e9-115">Delete</span><span class="sxs-lookup"><span data-stu-id="9f6e9-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="9f6e9-116">Keine</span><span class="sxs-lookup"><span data-stu-id="9f6e9-116">None</span></span> |<span data-ttu-id="9f6e9-117">Dient zum Löschen des referenceAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-117">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9f6e9-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9f6e9-118">Properties</span></span>
| <span data-ttu-id="9f6e9-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f6e9-119">Property</span></span>     | <span data-ttu-id="9f6e9-120">Typ</span><span class="sxs-lookup"><span data-stu-id="9f6e9-120">Type</span></span>   |<span data-ttu-id="9f6e9-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f6e9-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f6e9-122">contentType</span><span class="sxs-lookup"><span data-stu-id="9f6e9-122">contentType</span></span>|<span data-ttu-id="9f6e9-123">String</span><span class="sxs-lookup"><span data-stu-id="9f6e9-123">String</span></span>|<span data-ttu-id="9f6e9-124">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-124">The content type of the attachment.</span></span> <span data-ttu-id="9f6e9-125">Optional.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-125">Optional.</span></span>|
|<span data-ttu-id="9f6e9-126">id</span><span class="sxs-lookup"><span data-stu-id="9f6e9-126">id</span></span>|<span data-ttu-id="9f6e9-127">String</span><span class="sxs-lookup"><span data-stu-id="9f6e9-127">String</span></span>|<span data-ttu-id="9f6e9-p103">Die Anlagen-ID.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-p103">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="9f6e9-130">isFolder</span><span class="sxs-lookup"><span data-stu-id="9f6e9-130">isFolder</span></span>|<span data-ttu-id="9f6e9-131">Boolesch</span><span class="sxs-lookup"><span data-stu-id="9f6e9-131">Boolean</span></span>|<span data-ttu-id="9f6e9-132">Gibt an, ob die Anlage eine Verknüpfung zu einem Ordner ist.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-132">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="9f6e9-133">Setzen Sie müssen diese auf "true" Wenn **SourceUrl** eine Verknüpfung zu einem Ordner ist.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-133">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="9f6e9-134">Optional.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-134">Optional.</span></span>|
|<span data-ttu-id="9f6e9-135">isInline</span><span class="sxs-lookup"><span data-stu-id="9f6e9-135">isInline</span></span>|<span data-ttu-id="9f6e9-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9f6e9-136">Boolean</span></span>|<span data-ttu-id="9f6e9-137">Wird auf „true“ festgelegt, wenn die Anlage inline im Text des einbettenden Objekts angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-137">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="9f6e9-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-138">Optional.</span></span>|
|<span data-ttu-id="9f6e9-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f6e9-139">lastModifiedDateTime</span></span>|<span data-ttu-id="9f6e9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f6e9-140">DateTimeOffset</span></span>|<span data-ttu-id="9f6e9-141">Datum und Uhrzeit der letzten Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-141">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="9f6e9-142">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9f6e9-143">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9f6e9-144">Optional.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-144">Optional.</span></span>|
|<span data-ttu-id="9f6e9-145">name</span><span class="sxs-lookup"><span data-stu-id="9f6e9-145">name</span></span>|<span data-ttu-id="9f6e9-146">String</span><span class="sxs-lookup"><span data-stu-id="9f6e9-146">String</span></span>|<span data-ttu-id="9f6e9-147">Der Text, der unterhalb des Symbols, das die eingebettete Anlage darstellt angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-147">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="9f6e9-148">Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-148">This does not need to be the actual file name.</span></span> <span data-ttu-id="9f6e9-149">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-149">Required.</span></span>|
|<span data-ttu-id="9f6e9-150">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="9f6e9-150">permission</span></span>|<span data-ttu-id="9f6e9-151">ReferenceAttachmentPermissions</span><span class="sxs-lookup"><span data-stu-id="9f6e9-151">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="9f6e9-152">Gibt die Berechtigungen für die Anlage durch den Typ des Anbieters in **ProviderType**erteilt.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-152">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="9f6e9-153">Mögliche Werte sind: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView` und `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-153">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="9f6e9-154">Optional.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-154">Optional.</span></span>|
|<span data-ttu-id="9f6e9-155">previewUrl</span><span class="sxs-lookup"><span data-stu-id="9f6e9-155">previewUrl</span></span>|<span data-ttu-id="9f6e9-156">String</span><span class="sxs-lookup"><span data-stu-id="9f6e9-156">String</span></span>|<span data-ttu-id="9f6e9-157">Betrifft nur eine Referenz Anlage ein Bild - URL, um ein Vorschaubild abzurufen.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-157">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="9f6e9-158">Verwenden Sie **ThumbnailUrl** und **PreviewUrl** nur, wenn **SourceUrl** eine Bilddatei identifiziert.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-158">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="9f6e9-159">Optional.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-159">Optional.</span></span>|
|<span data-ttu-id="9f6e9-160">providerType</span><span class="sxs-lookup"><span data-stu-id="9f6e9-160">providerType</span></span>|<span data-ttu-id="9f6e9-161">ReferenceAttachmentProviders</span><span class="sxs-lookup"><span data-stu-id="9f6e9-161">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="9f6e9-162">Der Typ der Anbieter, der eine Anlage von diesem ContentType unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-162">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="9f6e9-163">Mögliche Werte: sind `other`, `oneDriveBusiness`, `oneDriveConsumer` und `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-163">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="9f6e9-164">Optional.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-164">Optional.</span></span>|
|<span data-ttu-id="9f6e9-165">size</span><span class="sxs-lookup"><span data-stu-id="9f6e9-165">size</span></span>|<span data-ttu-id="9f6e9-166">Int32</span><span class="sxs-lookup"><span data-stu-id="9f6e9-166">Int32</span></span>|<span data-ttu-id="9f6e9-167">Die Größe der Metadaten in Bytes, die für die Nachricht für die Anlage Verweis gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-167">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="9f6e9-168">Dieser Wert gibt nicht die Größe der tatsächlichen Datei an.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-168">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="9f6e9-169">Optional.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-169">Optional.</span></span>|
|<span data-ttu-id="9f6e9-170">SourceUrl</span><span class="sxs-lookup"><span data-stu-id="9f6e9-170">sourceUrl</span></span>|<span data-ttu-id="9f6e9-171">String</span><span class="sxs-lookup"><span data-stu-id="9f6e9-171">String</span></span>|<span data-ttu-id="9f6e9-172">URL, um den Inhalt der Anlage abzurufen.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-172">URL to get the attachment content.</span></span> <span data-ttu-id="9f6e9-173">Ist dies eine URL zu einem Ordner, legen Sie dann für den Ordner in Outlook oder Outlook im Web ordnungsgemäß anzuzeigende **IsFolder** auf "true".</span><span class="sxs-lookup"><span data-stu-id="9f6e9-173">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="9f6e9-174">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-174">Required.</span></span>|
|<span data-ttu-id="9f6e9-175">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="9f6e9-175">thumbnailUrl</span></span>|<span data-ttu-id="9f6e9-176">String</span><span class="sxs-lookup"><span data-stu-id="9f6e9-176">String</span></span>|<span data-ttu-id="9f6e9-177">Betrifft nur eine Referenz Anlage ein Bild - URL ein Miniaturbild abgerufen.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-177">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="9f6e9-178">Verwenden Sie **ThumbnailUrl** und **PreviewUrl** nur, wenn **SourceUrl** eine Bilddatei identifiziert.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-178">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="9f6e9-179">Optional.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-179">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f6e9-180">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9f6e9-180">Relationships</span></span>
<span data-ttu-id="9f6e9-181">Keine</span><span class="sxs-lookup"><span data-stu-id="9f6e9-181">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="9f6e9-182">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9f6e9-182">JSON representation</span></span>

<span data-ttu-id="9f6e9-183">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9f6e9-183">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
