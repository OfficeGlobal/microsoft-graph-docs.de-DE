---
title: itemAttachment-Ressourcentyp
description: Ein Kontakt, ein Ereignis oder eine Nachricht, die mit einem anderen Ereignis zugeordnet ist,
localization_priority: Normal
ms.openlocfilehash: b0e3b62e5f6100884e6fbea40d16221bf8503897
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571408"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="d2907-103">itemAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d2907-103">itemAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2907-104">Ein Kontakt, ein Ereignis oder eine Nachricht, die an einem anderen [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md)angefügt ist.</span><span class="sxs-lookup"><span data-stu-id="d2907-104">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="d2907-105">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="d2907-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d2907-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="d2907-106">Methods</span></span>

| <span data-ttu-id="d2907-107">Methode</span><span class="sxs-lookup"><span data-stu-id="d2907-107">Method</span></span>       | <span data-ttu-id="d2907-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d2907-108">Return Type</span></span>  |<span data-ttu-id="d2907-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2907-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2907-110">Get</span><span class="sxs-lookup"><span data-stu-id="d2907-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="d2907-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="d2907-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="d2907-112">Dient zum Lesen der Eigenschaften und der Beziehungen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d2907-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="d2907-113">Löschen</span><span class="sxs-lookup"><span data-stu-id="d2907-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="d2907-114">Keine</span><span class="sxs-lookup"><span data-stu-id="d2907-114">None</span></span> |<span data-ttu-id="d2907-115">Dient zum Löschen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d2907-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d2907-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d2907-116">Properties</span></span>
| <span data-ttu-id="d2907-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2907-117">Property</span></span>     | <span data-ttu-id="d2907-118">Typ</span><span class="sxs-lookup"><span data-stu-id="d2907-118">Type</span></span>   |<span data-ttu-id="d2907-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2907-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2907-120">contentType</span><span class="sxs-lookup"><span data-stu-id="d2907-120">contentType</span></span>|<span data-ttu-id="d2907-121">String</span><span class="sxs-lookup"><span data-stu-id="d2907-121">String</span></span>|<span data-ttu-id="d2907-122">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="d2907-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="d2907-123">id</span><span class="sxs-lookup"><span data-stu-id="d2907-123">id</span></span>|<span data-ttu-id="d2907-124">String</span><span class="sxs-lookup"><span data-stu-id="d2907-124">String</span></span>| <span data-ttu-id="d2907-125">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="d2907-125">The attachment ID.</span></span>|
|<span data-ttu-id="d2907-126">isInline</span><span class="sxs-lookup"><span data-stu-id="d2907-126">isInline</span></span>|<span data-ttu-id="d2907-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2907-127">Boolean</span></span>|<span data-ttu-id="d2907-128">Legen Sie diesen auf „true“ fest, wenn es sich um eine Inlineanlage handelt, z. B. ein eingebettetes Bild innerhalb des Textkörpers des Elements.</span><span class="sxs-lookup"><span data-stu-id="d2907-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="d2907-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2907-129">lastModifiedDateTime</span></span>|<span data-ttu-id="d2907-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2907-130">DateTimeOffset</span></span>|<span data-ttu-id="d2907-131">Letzte Uhrzeit und letztes Datum der Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="d2907-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="d2907-132">name</span><span class="sxs-lookup"><span data-stu-id="d2907-132">name</span></span>|<span data-ttu-id="d2907-133">String</span><span class="sxs-lookup"><span data-stu-id="d2907-133">String</span></span>|<span data-ttu-id="d2907-134">Der Anzeigename der Anlage.</span><span class="sxs-lookup"><span data-stu-id="d2907-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="d2907-135">size</span><span class="sxs-lookup"><span data-stu-id="d2907-135">size</span></span>|<span data-ttu-id="d2907-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d2907-136">Int32</span></span>|<span data-ttu-id="d2907-137">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="d2907-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2907-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d2907-138">Relationships</span></span>
| <span data-ttu-id="d2907-139">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d2907-139">Relationship</span></span> | <span data-ttu-id="d2907-140">Typ</span><span class="sxs-lookup"><span data-stu-id="d2907-140">Type</span></span>   |<span data-ttu-id="d2907-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2907-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2907-142">item</span><span class="sxs-lookup"><span data-stu-id="d2907-142">item</span></span>|[<span data-ttu-id="d2907-143">outlookItem</span><span class="sxs-lookup"><span data-stu-id="d2907-143">outlookItem</span></span>](outlookitem.md)|<span data-ttu-id="d2907-144">Das angefügte Kontakt Nachricht oder Ereignis.</span><span class="sxs-lookup"><span data-stu-id="d2907-144">The attached contact, message or event.</span></span> <span data-ttu-id="d2907-145">Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="d2907-145">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2907-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d2907-146">JSON representation</span></span>

<span data-ttu-id="d2907-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d2907-147">Here is a JSON representation of the resource</span></span>

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
