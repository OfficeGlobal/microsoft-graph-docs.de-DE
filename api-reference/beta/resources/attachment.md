---
title: Ressourcentyp attachment
description: Sie können ein Ereignis verwandten Inhalten hinzugefügt
localization_priority: Normal
ms.openlocfilehash: 8f7a6f9392d376995a53d9a4c06083780b0437b9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573424"
---
# <a name="attachment-resource-type"></a><span data-ttu-id="eae5f-103">Ressourcentyp attachment</span><span class="sxs-lookup"><span data-stu-id="eae5f-103">attachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eae5f-104">Sie können ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder in Form einer Anlage [Buchen](../resources/post.md) verwandten Inhalten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="eae5f-104">You can add related content to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) in the form of an attachment.</span></span>

<span data-ttu-id="eae5f-105">**attachment** ist die Basisressource für die folgenden abgeleiteten Typen von Anlagen:</span><span class="sxs-lookup"><span data-stu-id="eae5f-105">**attachment** is the base resource for the following derived types of attachments:</span></span>

* <span data-ttu-id="eae5f-106">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="eae5f-106">A file ([fileAttachment](../resources/fileattachment.md) resource)</span></span>
* <span data-ttu-id="eae5f-107">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="eae5f-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="eae5f-108">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="eae5f-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="eae5f-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="eae5f-109">Methods</span></span>

<span data-ttu-id="eae5f-110">Die folgenden Methoden gelten für alle abgeleiteten Typen von Anlagen (**fileAttachment**, **itemAttachment** oder **referenceAttachment**).</span><span class="sxs-lookup"><span data-stu-id="eae5f-110">The following methods apply to any of the derived types of attachments (**fileAttachment**, **itemAttachment**, or **referenceAttachment**).</span></span>

| <span data-ttu-id="eae5f-111">Methode</span><span class="sxs-lookup"><span data-stu-id="eae5f-111">Method</span></span>       | <span data-ttu-id="eae5f-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="eae5f-112">Return Type</span></span>  |<span data-ttu-id="eae5f-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eae5f-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eae5f-114">Anlage abrufen</span><span class="sxs-lookup"><span data-stu-id="eae5f-114">Get attachment</span></span>](../api/attachment-get.md) | [<span data-ttu-id="eae5f-115">attachment</span><span class="sxs-lookup"><span data-stu-id="eae5f-115">attachment</span></span>](attachment.md) |<span data-ttu-id="eae5f-116">Lesen Sie die Eigenschaften und Beziehungen der Anlage, die ein Ereignis, Nachricht, Outlook-Aufgabe oder Post zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="eae5f-116">Read the properties and relationships of an attachment, attached to an event, message, Outlook task, or post.</span></span>|
|[<span data-ttu-id="eae5f-117">Anlage einem Ereignis hinzufügen</span><span class="sxs-lookup"><span data-stu-id="eae5f-117">Add attachment to an event</span></span>](../api/event-post-attachments.md) | [<span data-ttu-id="eae5f-118">attachment</span><span class="sxs-lookup"><span data-stu-id="eae5f-118">attachment</span></span>](attachment.md) |<span data-ttu-id="eae5f-119">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Ereignis.</span><span class="sxs-lookup"><span data-stu-id="eae5f-119">Add a file, item, or link attachment to an event.</span></span>|
|[<span data-ttu-id="eae5f-120">Anlagen einer Nachricht hinzufügen</span><span class="sxs-lookup"><span data-stu-id="eae5f-120">Add attachment to a message</span></span>](../api/message-post-attachments.md) | [<span data-ttu-id="eae5f-121">attachment</span><span class="sxs-lookup"><span data-stu-id="eae5f-121">attachment</span></span>](attachment.md) |<span data-ttu-id="eae5f-122">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einer Nachricht.</span><span class="sxs-lookup"><span data-stu-id="eae5f-122">Add a file, item, or link attachment to a message.</span></span>|
|[<span data-ttu-id="eae5f-123">Hinzufügen einer Outlook-Aufgabe des Attachment-Objekts</span><span class="sxs-lookup"><span data-stu-id="eae5f-123">Add attachment to an Outlook task</span></span>](../api/outlooktask-post-attachments.md) | [<span data-ttu-id="eae5f-124">Anlage</span><span class="sxs-lookup"><span data-stu-id="eae5f-124">attachment</span></span>](attachment.md) |<span data-ttu-id="eae5f-125">Hinzufügen einer Datei, Element oder Link Anlage zu einer Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="eae5f-125">Add a file, item, or link attachment to an Outlook task.</span></span>|
|[<span data-ttu-id="eae5f-126">Anlage einem Beitrag hinzufügen</span><span class="sxs-lookup"><span data-stu-id="eae5f-126">Add attachment to a post</span></span>](../api/post-post-attachments.md) | [<span data-ttu-id="eae5f-127">attachment</span><span class="sxs-lookup"><span data-stu-id="eae5f-127">attachment</span></span>](attachment.md) |<span data-ttu-id="eae5f-128">Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Beitrag.</span><span class="sxs-lookup"><span data-stu-id="eae5f-128">Add a file, item, or link attachment to a post.</span></span>|
|[<span data-ttu-id="eae5f-129">Anlagen eines Ereignisses auflisten</span><span class="sxs-lookup"><span data-stu-id="eae5f-129">List attachments of an event</span></span>](../api/event-list-attachments.md) | <span data-ttu-id="eae5f-130">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="eae5f-130">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="eae5f-131">Liste der Anlagen für ein Ereignis abrufen</span><span class="sxs-lookup"><span data-stu-id="eae5f-131">Get a list of attachments for an event.</span></span> |
|[<span data-ttu-id="eae5f-132">Anlagen einer Nachricht auflisten</span><span class="sxs-lookup"><span data-stu-id="eae5f-132">List attachments of a message</span></span>](../api/message-list-attachments.md) | <span data-ttu-id="eae5f-133">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="eae5f-133">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="eae5f-134">Liste der Anlagen für eine Nachricht abrufen</span><span class="sxs-lookup"><span data-stu-id="eae5f-134">Get a list of attachments for a message.</span></span> |
|[<span data-ttu-id="eae5f-135">Liste von Anlagen eines Outlook-Aufgaben</span><span class="sxs-lookup"><span data-stu-id="eae5f-135">List attachments of an Outlook task</span></span>](../api/outlooktask-list-attachments.md) | <span data-ttu-id="eae5f-136">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="eae5f-136">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="eae5f-137">Abrufen einer Liste von Anlagen für eine Outlook-Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="eae5f-137">Get a list of attachments for an Outlook task.</span></span> |
|[<span data-ttu-id="eae5f-138">Anlagen eines Beitrags auflisten</span><span class="sxs-lookup"><span data-stu-id="eae5f-138">List attachments of a post</span></span>](../api/post-list-attachments.md) | <span data-ttu-id="eae5f-139">[attachment](attachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="eae5f-139">[attachment](attachment.md) collection</span></span> | <span data-ttu-id="eae5f-140">Liste der Anlagen für einen Beitrag abrufen</span><span class="sxs-lookup"><span data-stu-id="eae5f-140">Get a list of attachments for a post.</span></span> |
|[<span data-ttu-id="eae5f-141">Löschen</span><span class="sxs-lookup"><span data-stu-id="eae5f-141">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="eae5f-142">Keine</span><span class="sxs-lookup"><span data-stu-id="eae5f-142">None</span></span> |<span data-ttu-id="eae5f-143">Löschen einer Anlage auf ein Ereignis, Nachricht, Outlook-Aufgabe oder Post.</span><span class="sxs-lookup"><span data-stu-id="eae5f-143">Delete an attachment on an event, message, Outlook task, or post.</span></span> |

## <a name="properties"></a><span data-ttu-id="eae5f-144">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eae5f-144">Properties</span></span>

<span data-ttu-id="eae5f-p101">Nachfolgend finden Sie die grundlegenden Eigenschaften von attachment-Ressourcen. Zusätzliche Eigenschaften finden Sie bei dem jeweiligen Anlagentyp ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) oder [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="eae5f-p101">The following are the base properties of any attachment resource. Refer to the specific type of attachment ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md)) for additional properties.</span></span>

| <span data-ttu-id="eae5f-147">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eae5f-147">Property</span></span>     | <span data-ttu-id="eae5f-148">Typ</span><span class="sxs-lookup"><span data-stu-id="eae5f-148">Type</span></span>   |<span data-ttu-id="eae5f-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eae5f-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eae5f-150">contentType</span><span class="sxs-lookup"><span data-stu-id="eae5f-150">contentType</span></span>|<span data-ttu-id="eae5f-151">String</span><span class="sxs-lookup"><span data-stu-id="eae5f-151">String</span></span>|<span data-ttu-id="eae5f-152">Der MIME-Typ.</span><span class="sxs-lookup"><span data-stu-id="eae5f-152">The MIME type.</span></span>|
|<span data-ttu-id="eae5f-153">id</span><span class="sxs-lookup"><span data-stu-id="eae5f-153">id</span></span>|<span data-ttu-id="eae5f-154">String</span><span class="sxs-lookup"><span data-stu-id="eae5f-154">String</span></span>| <span data-ttu-id="eae5f-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="eae5f-155">Read-only.</span></span>|
|<span data-ttu-id="eae5f-156">isInline</span><span class="sxs-lookup"><span data-stu-id="eae5f-156">isInline</span></span>|<span data-ttu-id="eae5f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="eae5f-157">Boolean</span></span>|<span data-ttu-id="eae5f-158">`true`, wenn die Anlage eine Inlineanlage ist, andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="eae5f-158">`true` if the attachment is an inline attachment; otherwise, `false`.</span></span>|
|<span data-ttu-id="eae5f-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eae5f-159">lastModifiedDateTime</span></span>|<span data-ttu-id="eae5f-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eae5f-160">DateTimeOffset</span></span>|<span data-ttu-id="eae5f-p102">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eae5f-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="eae5f-163">name</span><span class="sxs-lookup"><span data-stu-id="eae5f-163">name</span></span>|<span data-ttu-id="eae5f-164">String</span><span class="sxs-lookup"><span data-stu-id="eae5f-164">String</span></span>|<span data-ttu-id="eae5f-165">Der Anzeigename der Anlage.</span><span class="sxs-lookup"><span data-stu-id="eae5f-165">The display name of the attachment.</span></span> <span data-ttu-id="eae5f-166">Dies muss nicht der tatsächliche Dateiname sein.</span><span class="sxs-lookup"><span data-stu-id="eae5f-166">This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="eae5f-167">size</span><span class="sxs-lookup"><span data-stu-id="eae5f-167">size</span></span>|<span data-ttu-id="eae5f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="eae5f-168">Int32</span></span>|<span data-ttu-id="eae5f-169">Die Länge der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="eae5f-169">The length of the attachment in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eae5f-170">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="eae5f-170">Relationships</span></span>
<span data-ttu-id="eae5f-171">Keine</span><span class="sxs-lookup"><span data-stu-id="eae5f-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eae5f-172">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eae5f-172">JSON representation</span></span>

<span data-ttu-id="eae5f-173">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eae5f-173">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
