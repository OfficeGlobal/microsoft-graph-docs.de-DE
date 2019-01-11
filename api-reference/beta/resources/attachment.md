---
title: Ressourcentyp attachment
description: Sie können ein Ereignis verwandten Inhalten hinzugefügt
localization_priority: Normal
ms.openlocfilehash: 5648194b0f636c8757d1b20c492abc099dce377d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842791"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="e91bb-103">Ressourcentyp attachment</span><span class="sxs-lookup"><span data-stu-id="e91bb-103">attachment resource type</span></span>

> <span data-ttu-id="e91bb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e91bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e91bb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e91bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e91bb-106">Sie können ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder in Form einer Anlage [Buchen](../resources/post.md) verwandten Inhalten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="e91bb-106">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="e91bb-107">**attachment** ist die Basisressource für die folgenden abgeleiteten Typen von Anlagen:</span><span class="sxs-lookup"><span data-stu-id="e91bb-107">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="e91bb-108">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="e91bb-108">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="e91bb-109">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="e91bb-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="e91bb-110">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="e91bb-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="e91bb-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="e91bb-111">Methods</span></span>

<span data-ttu-id="e91bb-112">Die folgenden Methoden gelten für alle abgeleiteten Typen von Anlagen (**fileAttachment**, **itemAttachment** oder **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="e91bb-112">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="e91bb-113">Methode</span><span class="sxs-lookup"><span data-stu-id="e91bb-113">Method</span></span>       | <span data-ttu-id="e91bb-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e91bb-114">Return Type</span></span>  |<span data-ttu-id="e91bb-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e91bb-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e91bb-116">Anlage abrufen</span><span class="sxs-lookup"><span data-stu-id="e91bb-116">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e91bb-117">attachment</span><span class="sxs-lookup"><span data-stu-id="e91bb-117">attachment</span></span>](attachment.md) |<span data-ttu-id="e91bb-118">Lesen Sie die Eigenschaften und Beziehungen der Anlage, die ein Ereignis, Nachricht, Outlook-Aufgabe oder Post zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="e91bb-118">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="e91bb-119">Anlage einem Ereignis hinzufügen</span><span class="sxs-lookup"><span data-stu-id="e91bb-119">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="e91bb-120">attachment</span><span class="sxs-lookup"><span data-stu-id="e91bb-120">attachment</span></span>](attachment.md) |<span data-ttu-id="e91bb-121">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Ereignis.</span><span class="sxs-lookup"><span data-stu-id="e91bb-121">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="e91bb-122">Anlagen einer Nachricht hinzufügen</span><span class="sxs-lookup"><span data-stu-id="e91bb-122">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="e91bb-123">attachment</span><span class="sxs-lookup"><span data-stu-id="e91bb-123">attachment</span></span>](attachment.md) |<span data-ttu-id="e91bb-124">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einer Nachricht.</span><span class="sxs-lookup"><span data-stu-id="e91bb-124">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="e91bb-125">Hinzufügen einer Outlook-Aufgabe des Attachment-Objekts</span><span class="sxs-lookup"><span data-stu-id="e91bb-125">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="e91bb-126">Anlage</span><span class="sxs-lookup"><span data-stu-id="e91bb-126">attachment</span></span>](attachment.md) |<span data-ttu-id="e91bb-127">Hinzufügen einer Datei, Element oder Link Anlage zu einer Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="e91bb-127">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="e91bb-128">Anlage einem Beitrag hinzufügen</span><span class="sxs-lookup"><span data-stu-id="e91bb-128">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="e91bb-129">attachment</span><span class="sxs-lookup"><span data-stu-id="e91bb-129">attachment</span></span>](attachment.md) |<span data-ttu-id="e91bb-130">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Beitrag.</span><span class="sxs-lookup"><span data-stu-id="e91bb-130">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="e91bb-131">Anlagen eines Ereignisses auflisten</span><span class="sxs-lookup"><span data-stu-id="e91bb-131">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="e91bb-132">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="e91bb-132">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e91bb-133">Liste der Anlagen für ein Ereignis abrufen</span><span class="sxs-lookup"><span data-stu-id="e91bb-133">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="e91bb-134">Anlagen einer Nachricht auflisten</span><span class="sxs-lookup"><span data-stu-id="e91bb-134">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="e91bb-135">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="e91bb-135">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e91bb-136">Liste der Anlagen für eine Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="e91bb-136">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="e91bb-137">Liste von Anlagen eines Outlook-Aufgaben</span><span class="sxs-lookup"><span data-stu-id="e91bb-137">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="e91bb-138">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="e91bb-138">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e91bb-139">Abrufen einer Liste von Anlagen für eine Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="e91bb-139">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="e91bb-140">Anlagen eines Beitrags auflisten</span><span class="sxs-lookup"><span data-stu-id="e91bb-140">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="e91bb-141">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="e91bb-141">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="e91bb-142">Liste der Anlagen für einen Beitrag abrufen</span><span class="sxs-lookup"><span data-stu-id="e91bb-142">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="e91bb-143">Löschen</span><span class="sxs-lookup"><span data-stu-id="e91bb-143">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="e91bb-144">Keine</span><span class="sxs-lookup"><span data-stu-id="e91bb-144">None</span></span> |<span data-ttu-id="e91bb-145">Löschen einer Anlage auf ein Ereignis, Nachricht, Outlook-Aufgabe oder Post.</span><span class="sxs-lookup"><span data-stu-id="e91bb-145">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="e91bb-146">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e91bb-146">Properties</span></span>

<span data-ttu-id="e91bb-p102">Nachfolgend finden Sie die grundlegenden Eigenschaften von attachment-Ressourcen. Zusätzliche Eigenschaften finden Sie bei dem jeweiligen Anlagentyp ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) oder [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="e91bb-p102">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="e91bb-149">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e91bb-149">Property</span></span>     | <span data-ttu-id="e91bb-150">Typ</span><span class="sxs-lookup"><span data-stu-id="e91bb-150">Type</span></span>   |<span data-ttu-id="e91bb-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e91bb-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e91bb-152">contentType</span><span class="sxs-lookup"><span data-stu-id="e91bb-152">contentType</span></span>|<span data-ttu-id="e91bb-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e91bb-153">String</span></span>|<span data-ttu-id="e91bb-154">Der MIME-Typ.</span><span class="sxs-lookup"><span data-stu-id="e91bb-154">The MIME type.</span></span>|
|<span data-ttu-id="e91bb-155">id</span><span class="sxs-lookup"><span data-stu-id="e91bb-155">id</span></span>|<span data-ttu-id="e91bb-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e91bb-156">String</span></span>| <span data-ttu-id="e91bb-157">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e91bb-157">Read-only.</span></span>|
|<span data-ttu-id="e91bb-158">isInline</span><span class="sxs-lookup"><span data-stu-id="e91bb-158">isInline</span></span>|<span data-ttu-id="e91bb-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="e91bb-159">Boolean</span></span>|<span data-ttu-id="e91bb-160">`true`, wenn die Anlage eine Inlineanlage ist, andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="e91bb-160">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="e91bb-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e91bb-161">lastModifiedDateTime</span></span>|<span data-ttu-id="e91bb-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e91bb-162">DateTimeOffset</span></span>|<span data-ttu-id="e91bb-p103">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e91bb-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e91bb-165">name</span><span class="sxs-lookup"><span data-stu-id="e91bb-165">name</span></span>|<span data-ttu-id="e91bb-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e91bb-166">String</span></span>|<span data-ttu-id="e91bb-167">Der Anzeigename der Anlage.</span><span class="sxs-lookup"><span data-stu-id="e91bb-167">The display name of the attachment.</span></span> <span data-ttu-id="e91bb-168">Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="e91bb-168">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="e91bb-169">size</span><span class="sxs-lookup"><span data-stu-id="e91bb-169">size</span></span>|<span data-ttu-id="e91bb-170">Int32</span><span class="sxs-lookup"><span data-stu-id="e91bb-170">Int32</span></span>|<span data-ttu-id="e91bb-171">Die Länge der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="e91bb-171">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e91bb-172">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e91bb-172">Relationships</span></span>
<span data-ttu-id="e91bb-173">Keine</span><span class="sxs-lookup"><span data-stu-id="e91bb-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e91bb-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e91bb-174">JSON representation</span></span>

<span data-ttu-id="e91bb-175">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e91bb-175">Here is a JSON representation of the resource</span></span>

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
