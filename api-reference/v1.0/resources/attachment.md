---
title: Ressourcentyp attachment
description: Sie können ein Ereignis verwandten Inhalten hinzugefügt
localization_priority: Priority
ms.openlocfilehash: 284895871a0c6a80140ff248045b89d2de104c20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892330"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="accfc-103">Ressourcentyp attachment</span><span class="sxs-lookup"><span data-stu-id="accfc-103">attachment resource type</span></span>

<span data-ttu-id="accfc-104">Sie können verwandte Inhalte in Form einer Anlage zu einem [Ereignis](../resources/event.md), einer [Nachricht](../resources/message.md) oder einem [Beitrag](../resources/post.md) hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="accfc-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="accfc-105">**attachment** ist die Basisressource für die folgenden abgeleiteten Typen von Anlagen:</span><span class="sxs-lookup"><span data-stu-id="accfc-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="accfc-106">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="accfc-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="accfc-107">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="accfc-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="accfc-108">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="accfc-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>


## <a name="methods"></a><span data-ttu-id="accfc-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="accfc-109">Methods</span></span>

<span data-ttu-id="accfc-110">Die folgenden Methoden gelten für alle abgeleiteten Typen von Anlagen (**fileAttachment**, **itemAttachment** oder **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="accfc-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="accfc-111">Methode</span><span class="sxs-lookup"><span data-stu-id="accfc-111">Method</span></span>       | <span data-ttu-id="accfc-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="accfc-112">Return Type</span></span>  |<span data-ttu-id="accfc-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="accfc-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="accfc-114">Anlage abrufen</span><span class="sxs-lookup"><span data-stu-id="accfc-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="accfc-115">attachment</span><span class="sxs-lookup"><span data-stu-id="accfc-115">attachment</span></span>](attachment.md) |<span data-ttu-id="accfc-116">Lesen Sie die Eigenschaften und Beziehungen einer Anlage, die einem Ereignis, einer Nachricht oder einem Beitrag angehängt ist.</span><span class="sxs-lookup"><span data-stu-id="accfc-116">Read the properties and relationships of an attachment, attached to an event, message, or post.</span></span>|
|[<span data-ttu-id="accfc-117">Anlage einem Ereignis hinzufügen</span><span class="sxs-lookup"><span data-stu-id="accfc-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="accfc-118">attachment</span><span class="sxs-lookup"><span data-stu-id="accfc-118">attachment</span></span>](attachment.md) |<span data-ttu-id="accfc-119">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Ereignis.</span><span class="sxs-lookup"><span data-stu-id="accfc-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="accfc-120">Anlagen einer Nachricht hinzufügen</span><span class="sxs-lookup"><span data-stu-id="accfc-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="accfc-121">attachment</span><span class="sxs-lookup"><span data-stu-id="accfc-121">attachment</span></span>](attachment.md) |<span data-ttu-id="accfc-122">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einer Nachricht.</span><span class="sxs-lookup"><span data-stu-id="accfc-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="accfc-123">Anlage einem Beitrag hinzufügen</span><span class="sxs-lookup"><span data-stu-id="accfc-123">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="accfc-124">attachment</span><span class="sxs-lookup"><span data-stu-id="accfc-124">attachment</span></span>](attachment.md) |<span data-ttu-id="accfc-125">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Beitrag.</span><span class="sxs-lookup"><span data-stu-id="accfc-125">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="accfc-126">Anlagen eines Ereignisses auflisten</span><span class="sxs-lookup"><span data-stu-id="accfc-126">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="accfc-127">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="accfc-127">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="accfc-128">Liste der Anlagen für ein Ereignis abrufen</span><span class="sxs-lookup"><span data-stu-id="accfc-128">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="accfc-129">Anlagen einer Nachricht auflisten</span><span class="sxs-lookup"><span data-stu-id="accfc-129">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="accfc-130">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="accfc-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="accfc-131">Liste der Anlagen für eine Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="accfc-131">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="accfc-132">Anlagen eines Beitrags auflisten</span><span class="sxs-lookup"><span data-stu-id="accfc-132">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="accfc-133">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="accfc-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="accfc-134">Liste der Anlagen für einen Beitrag abrufen</span><span class="sxs-lookup"><span data-stu-id="accfc-134">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="accfc-135">Löschen</span><span class="sxs-lookup"><span data-stu-id="accfc-135">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="accfc-136">Keine</span><span class="sxs-lookup"><span data-stu-id="accfc-136">None</span></span> |<span data-ttu-id="accfc-137">Eine Anlage für ein Ereignis, eine Nachricht oder einen Beitrag löschen</span><span class="sxs-lookup"><span data-stu-id="accfc-137">Delete an attachment on an event, message, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="accfc-138">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="accfc-138">Properties</span></span>

<span data-ttu-id="accfc-p101">Nachfolgend finden Sie die grundlegenden Eigenschaften von attachment-Ressourcen. Zusätzliche Eigenschaften finden Sie bei dem jeweiligen Anlagentyp ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) oder [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="accfc-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="accfc-141">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="accfc-141">Property</span></span>     | <span data-ttu-id="accfc-142">Typ</span><span class="sxs-lookup"><span data-stu-id="accfc-142">Type</span></span>   |<span data-ttu-id="accfc-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="accfc-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="accfc-144">contentType</span><span class="sxs-lookup"><span data-stu-id="accfc-144">contentType</span></span>|<span data-ttu-id="accfc-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="accfc-145">String</span></span>|<span data-ttu-id="accfc-146">Der MIME-Typ.</span><span class="sxs-lookup"><span data-stu-id="accfc-146">The MIME type.</span></span>|
|<span data-ttu-id="accfc-147">id</span><span class="sxs-lookup"><span data-stu-id="accfc-147">id</span></span>|<span data-ttu-id="accfc-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="accfc-148">String</span></span>| <span data-ttu-id="accfc-149">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="accfc-149">Read-only.</span></span>|
|<span data-ttu-id="accfc-150">isInline</span><span class="sxs-lookup"><span data-stu-id="accfc-150">isInline</span></span>|<span data-ttu-id="accfc-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="accfc-151">Boolean</span></span>|<span data-ttu-id="accfc-152">`true`, wenn die Anlage eine Inlineanlage ist, andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="accfc-152">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="accfc-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="accfc-153">lastModifiedDateTime</span></span>|<span data-ttu-id="accfc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="accfc-154">DateTimeOffset</span></span>|<span data-ttu-id="accfc-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="accfc-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="accfc-157">name</span><span class="sxs-lookup"><span data-stu-id="accfc-157">name</span></span>|<span data-ttu-id="accfc-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="accfc-158">String</span></span>|<span data-ttu-id="accfc-159">Der Dateiname der Anlage.</span><span class="sxs-lookup"><span data-stu-id="accfc-159">The attachment's file name.</span></span>|
|<span data-ttu-id="accfc-160">size</span><span class="sxs-lookup"><span data-stu-id="accfc-160">size</span></span>|<span data-ttu-id="accfc-161">Int32</span><span class="sxs-lookup"><span data-stu-id="accfc-161">Int32</span></span>|<span data-ttu-id="accfc-162">Die Länge der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="accfc-162">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="accfc-163">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="accfc-163">Relationships</span></span>
<span data-ttu-id="accfc-164">Keine</span><span class="sxs-lookup"><span data-stu-id="accfc-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="accfc-165">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="accfc-165">JSON representation</span></span>

<span data-ttu-id="accfc-166">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="accfc-166">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "abstract": true,
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
