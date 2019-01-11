---
title: referenceAttachment-Ressourcentyp
description: Ein Link zu einer Datei (z. B. eine Textdatei oder ein Word-Dokument) auf einem OneDrive for Business-Cloudlaufwerk oder anderen unterstützten Speicherorten, der an ein Ereignis, eine Nachricht oder einen Beitrag angefügt ist.
localization_priority: Normal
ms.openlocfilehash: 0696ac4b0f93ed4982ec576a15afe071486f9c88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853123"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="8bf81-103">referenceAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8bf81-103">referenceAttachment resource type</span></span>

<span data-ttu-id="8bf81-104">Ein Link zu einer Datei (z. B. eine Textdatei oder ein Word-Dokument) auf einem OneDrive for Business-Cloudlaufwerk oder anderen unterstützten Speicherorten, der an ein Ereignis, eine Nachricht oder einen Beitrag angefügt ist.</span><span class="sxs-lookup"><span data-stu-id="8bf81-104">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="8bf81-105">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="8bf81-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8bf81-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="8bf81-106">Methods</span></span>

| <span data-ttu-id="8bf81-107">Methode</span><span class="sxs-lookup"><span data-stu-id="8bf81-107">Method</span></span>       | <span data-ttu-id="8bf81-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8bf81-108">Return Type</span></span>  |<span data-ttu-id="8bf81-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8bf81-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8bf81-110">Abrufen</span><span class="sxs-lookup"><span data-stu-id="8bf81-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="8bf81-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="8bf81-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="8bf81-112">Dient zum Lesen der Eigenschaften und der Beziehungen des referenceAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8bf81-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="8bf81-113">Delete</span><span class="sxs-lookup"><span data-stu-id="8bf81-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="8bf81-114">Keine</span><span class="sxs-lookup"><span data-stu-id="8bf81-114">None</span></span> |<span data-ttu-id="8bf81-115">Dient zum Löschen des referenceAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8bf81-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8bf81-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8bf81-116">Properties</span></span>
| <span data-ttu-id="8bf81-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8bf81-117">Property</span></span>     | <span data-ttu-id="8bf81-118">Typ</span><span class="sxs-lookup"><span data-stu-id="8bf81-118">Type</span></span>   |<span data-ttu-id="8bf81-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8bf81-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bf81-120">contentType</span><span class="sxs-lookup"><span data-stu-id="8bf81-120">contentType</span></span>|<span data-ttu-id="8bf81-121">String</span><span class="sxs-lookup"><span data-stu-id="8bf81-121">String</span></span>|<span data-ttu-id="8bf81-122">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="8bf81-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="8bf81-123">id</span><span class="sxs-lookup"><span data-stu-id="8bf81-123">id</span></span>|<span data-ttu-id="8bf81-124">String</span><span class="sxs-lookup"><span data-stu-id="8bf81-124">String</span></span>|<span data-ttu-id="8bf81-p101">Die Anlagen-ID.  Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8bf81-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="8bf81-127">isInline</span><span class="sxs-lookup"><span data-stu-id="8bf81-127">isInline</span></span>|<span data-ttu-id="8bf81-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bf81-128">Boolean</span></span>|<span data-ttu-id="8bf81-129">Wird auf „true“ festgelegt, wenn die Anlage inline im Text des einbettenden Objekts angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="8bf81-129">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="8bf81-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bf81-130">lastModifiedDateTime</span></span>|<span data-ttu-id="8bf81-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bf81-131">DateTimeOffset</span></span>|<span data-ttu-id="8bf81-p102">Datum und Uhrzeit der letzten Änderung der Anlage. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8bf81-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8bf81-135">name</span><span class="sxs-lookup"><span data-stu-id="8bf81-135">name</span></span>|<span data-ttu-id="8bf81-136">String</span><span class="sxs-lookup"><span data-stu-id="8bf81-136">String</span></span>|<span data-ttu-id="8bf81-p103">Der Text, der unter dem Symbol angezeigt wird, das die eingebettete Anlage darstellt. Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="8bf81-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="8bf81-139">size</span><span class="sxs-lookup"><span data-stu-id="8bf81-139">size</span></span>|<span data-ttu-id="8bf81-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8bf81-140">Int32</span></span>|<span data-ttu-id="8bf81-141">Die Größe der Metadaten, die in der Nachricht für die Anlage gespeichert sind, in Byte.</span><span class="sxs-lookup"><span data-stu-id="8bf81-141">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="8bf81-142">Dieser Wert gibt nicht die Größe der tatsächlichen Datei an.</span><span class="sxs-lookup"><span data-stu-id="8bf81-142">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bf81-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8bf81-143">Relationships</span></span>
<span data-ttu-id="8bf81-144">Keine</span><span class="sxs-lookup"><span data-stu-id="8bf81-144">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="8bf81-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8bf81-145">JSON representation</span></span>

<span data-ttu-id="8bf81-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8bf81-146">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
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
