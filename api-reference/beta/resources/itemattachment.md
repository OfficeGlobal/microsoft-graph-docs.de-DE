---
title: itemAttachment-Ressourcentyp
description: Ein Kontakt, ein Ereignis oder eine Nachricht, die mit einem anderen Ereignis zugeordnet ist,
localization_priority: Normal
ms.openlocfilehash: cce33cb7597f04435daff723a0125305968eea99
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520109"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="6a852-103">itemAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6a852-103">itemAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a852-104">Ein Kontakt, ein Ereignis oder eine Nachricht, die an einem anderen [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md)angefügt ist.</span><span class="sxs-lookup"><span data-stu-id="6a852-104">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="6a852-105">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="6a852-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6a852-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="6a852-106">Methods</span></span>

| <span data-ttu-id="6a852-107">Methode</span><span class="sxs-lookup"><span data-stu-id="6a852-107">Method</span></span>       | <span data-ttu-id="6a852-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6a852-108">Return Type</span></span>  |<span data-ttu-id="6a852-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a852-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a852-110">Get</span><span class="sxs-lookup"><span data-stu-id="6a852-110">Get</span></span>](../api/attachment-get.md) | <span data-ttu-id="6a852-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="6a852-111">[itemAttachment](itemattachment.md)</span></span> |<span data-ttu-id="6a852-112">Dient zum Lesen der Eigenschaften und der Beziehungen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a852-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="6a852-113">Delete</span><span class="sxs-lookup"><span data-stu-id="6a852-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="6a852-114">Keine</span><span class="sxs-lookup"><span data-stu-id="6a852-114">None</span></span> |<span data-ttu-id="6a852-115">Dient zum Löschen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a852-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6a852-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6a852-116">Properties</span></span>
| <span data-ttu-id="6a852-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a852-117">Property</span></span>     | <span data-ttu-id="6a852-118">Typ</span><span class="sxs-lookup"><span data-stu-id="6a852-118">Type</span></span>   |<span data-ttu-id="6a852-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a852-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a852-120">contentType</span><span class="sxs-lookup"><span data-stu-id="6a852-120">contentType</span></span>|<span data-ttu-id="6a852-121">String</span><span class="sxs-lookup"><span data-stu-id="6a852-121">String</span></span>|<span data-ttu-id="6a852-122">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="6a852-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="6a852-123">id</span><span class="sxs-lookup"><span data-stu-id="6a852-123">id</span></span>|<span data-ttu-id="6a852-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a852-124">String</span></span>| <span data-ttu-id="6a852-125">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="6a852-125">The attachment ID.</span></span>|
|<span data-ttu-id="6a852-126">isInline</span><span class="sxs-lookup"><span data-stu-id="6a852-126">isInline</span></span>|<span data-ttu-id="6a852-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6a852-127">Boolean</span></span>|<span data-ttu-id="6a852-128">Legen Sie diesen auf „true“ fest, wenn es sich um eine Inlineanlage handelt, z. B. ein eingebettetes Bild innerhalb des Textkörpers des Elements.</span><span class="sxs-lookup"><span data-stu-id="6a852-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="6a852-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a852-129">lastModifiedDateTime</span></span>|<span data-ttu-id="6a852-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a852-130">DateTimeOffset</span></span>|<span data-ttu-id="6a852-131">Letzte Uhrzeit und letztes Datum der Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="6a852-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="6a852-132">name</span><span class="sxs-lookup"><span data-stu-id="6a852-132">name</span></span>|<span data-ttu-id="6a852-133">String</span><span class="sxs-lookup"><span data-stu-id="6a852-133">String</span></span>|<span data-ttu-id="6a852-134">Der Anzeigename der Anlage.</span><span class="sxs-lookup"><span data-stu-id="6a852-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="6a852-135">size</span><span class="sxs-lookup"><span data-stu-id="6a852-135">size</span></span>|<span data-ttu-id="6a852-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6a852-136">Int32</span></span>|<span data-ttu-id="6a852-137">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="6a852-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a852-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6a852-138">Relationships</span></span>
| <span data-ttu-id="6a852-139">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6a852-139">Relationship</span></span> | <span data-ttu-id="6a852-140">Typ</span><span class="sxs-lookup"><span data-stu-id="6a852-140">Type</span></span>   |<span data-ttu-id="6a852-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a852-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a852-142">item</span><span class="sxs-lookup"><span data-stu-id="6a852-142">item</span></span>|<span data-ttu-id="6a852-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="6a852-143">[OutlookItem](outlookitem.md)</span></span>|<span data-ttu-id="6a852-144">Das angefügte Kontakt Nachricht oder Ereignis.</span><span class="sxs-lookup"><span data-stu-id="6a852-144">The attached contact, message or event.</span></span> <span data-ttu-id="6a852-145">Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="6a852-145">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a852-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6a852-146">JSON representation</span></span>

<span data-ttu-id="6a852-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6a852-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "@odata.type": "microsoft.graph.itemAttachment"
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
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
