---
title: itemAttachment-Ressourcentyp
description: Ein Kontakt, ein Ereignis oder eine Nachricht, die mit einem anderen Ereignis zugeordnet ist,
ms.openlocfilehash: fd8638a7d263c2ebbe09c77f717af989e1dd5a0e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063568"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="3ed29-103">itemAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3ed29-103">itemAttachment resource type</span></span>

> <span data-ttu-id="3ed29-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3ed29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ed29-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ed29-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ed29-106">Ein Kontakt, ein Ereignis oder eine Nachricht, die an einem anderen [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md)angefügt ist.</span><span class="sxs-lookup"><span data-stu-id="3ed29-106">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="3ed29-107">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="3ed29-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3ed29-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="3ed29-108">Methods</span></span>

| <span data-ttu-id="3ed29-109">Methode</span><span class="sxs-lookup"><span data-stu-id="3ed29-109">Method</span></span>       | <span data-ttu-id="3ed29-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3ed29-110">Return Type</span></span>  |<span data-ttu-id="3ed29-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ed29-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3ed29-112">Get</span><span class="sxs-lookup"><span data-stu-id="3ed29-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="3ed29-113">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="3ed29-113">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="3ed29-114">Dient zum Lesen der Eigenschaften und der Beziehungen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3ed29-114">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="3ed29-115">Delete</span><span class="sxs-lookup"><span data-stu-id="3ed29-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="3ed29-116">Keine</span><span class="sxs-lookup"><span data-stu-id="3ed29-116">None</span></span> |<span data-ttu-id="3ed29-117">Dient zum Löschen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3ed29-117">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3ed29-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3ed29-118">Properties</span></span>
| <span data-ttu-id="3ed29-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ed29-119">Property</span></span>     | <span data-ttu-id="3ed29-120">Typ</span><span class="sxs-lookup"><span data-stu-id="3ed29-120">Type</span></span>   |<span data-ttu-id="3ed29-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ed29-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ed29-122">contentType</span><span class="sxs-lookup"><span data-stu-id="3ed29-122">contentType</span></span>|<span data-ttu-id="3ed29-123">String</span><span class="sxs-lookup"><span data-stu-id="3ed29-123">String</span></span>|<span data-ttu-id="3ed29-124">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="3ed29-124">The content type of the attachment.</span></span>|
|<span data-ttu-id="3ed29-125">id</span><span class="sxs-lookup"><span data-stu-id="3ed29-125">id</span></span>|<span data-ttu-id="3ed29-126">String</span><span class="sxs-lookup"><span data-stu-id="3ed29-126">String</span></span>| <span data-ttu-id="3ed29-127">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="3ed29-127">The attachment ID.</span></span>|
|<span data-ttu-id="3ed29-128">isInline</span><span class="sxs-lookup"><span data-stu-id="3ed29-128">isInline</span></span>|<span data-ttu-id="3ed29-129">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3ed29-129">Boolean</span></span>|<span data-ttu-id="3ed29-130">Legen Sie diesen auf „true“ fest, wenn es sich um eine Inlineanlage handelt, z. B. ein eingebettetes Bild innerhalb des Textkörpers des Elements.</span><span class="sxs-lookup"><span data-stu-id="3ed29-130">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="3ed29-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ed29-131">lastModifiedDateTime</span></span>|<span data-ttu-id="3ed29-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ed29-132">DateTimeOffset</span></span>|<span data-ttu-id="3ed29-133">Letzte Uhrzeit und letztes Datum der Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="3ed29-133">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="3ed29-134">name</span><span class="sxs-lookup"><span data-stu-id="3ed29-134">name</span></span>|<span data-ttu-id="3ed29-135">String</span><span class="sxs-lookup"><span data-stu-id="3ed29-135">String</span></span>|<span data-ttu-id="3ed29-136">Der Anzeigename der Anlage.</span><span class="sxs-lookup"><span data-stu-id="3ed29-136">The display name of the attachment.</span></span>|
|<span data-ttu-id="3ed29-137">size</span><span class="sxs-lookup"><span data-stu-id="3ed29-137">size</span></span>|<span data-ttu-id="3ed29-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3ed29-138">Int32</span></span>|<span data-ttu-id="3ed29-139">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="3ed29-139">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ed29-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3ed29-140">Relationships</span></span>
| <span data-ttu-id="3ed29-141">Beziehung</span><span class="sxs-lookup"><span data-stu-id="3ed29-141">Relationship</span></span> | <span data-ttu-id="3ed29-142">Typ</span><span class="sxs-lookup"><span data-stu-id="3ed29-142">Type</span></span>   |<span data-ttu-id="3ed29-143">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ed29-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ed29-144">item</span><span class="sxs-lookup"><span data-stu-id="3ed29-144">item</span></span>|[<span data-ttu-id="3ed29-145">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="3ed29-145">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="3ed29-146">Das angefügte Kontakt Nachricht oder Ereignis.</span><span class="sxs-lookup"><span data-stu-id="3ed29-146">The attached contact, message or event.</span></span> <span data-ttu-id="3ed29-147">Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="3ed29-147">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ed29-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3ed29-148">JSON representation</span></span>

<span data-ttu-id="3ed29-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3ed29-149">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
