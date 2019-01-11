---
title: itemAttachment-Ressourcentyp
description: 'Kontakt, Ereignis oder Nachricht, die an ein anderes Ereignis, eine andere Nachricht oder einen anderen Beitrag angefügt sind.  '
localization_priority: Priority
ms.openlocfilehash: df996175e545b78f4ca9a1b6271b9cb012ffffce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853522"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="1b681-103">itemAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1b681-103">itemAttachment resource type</span></span>

<span data-ttu-id="1b681-104">Kontakt, Ereignis oder Nachricht, die an ein anderes Ereignis, eine andere Nachricht oder einen anderen Beitrag angefügt sind.</span><span class="sxs-lookup"><span data-stu-id="1b681-104">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="1b681-105">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="1b681-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1b681-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="1b681-106">Methods</span></span>

| <span data-ttu-id="1b681-107">Methode</span><span class="sxs-lookup"><span data-stu-id="1b681-107">Method</span></span>       | <span data-ttu-id="1b681-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1b681-108">Return Type</span></span>  |<span data-ttu-id="1b681-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b681-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b681-110">Get</span><span class="sxs-lookup"><span data-stu-id="1b681-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="1b681-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="1b681-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="1b681-112">Dient zum Lesen der Eigenschaften und der Beziehungen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b681-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="1b681-113">Delete</span><span class="sxs-lookup"><span data-stu-id="1b681-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="1b681-114">Keine</span><span class="sxs-lookup"><span data-stu-id="1b681-114">None</span></span> |<span data-ttu-id="1b681-115">Dient zum Löschen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b681-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b681-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1b681-116">Properties</span></span>
| <span data-ttu-id="1b681-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b681-117">Property</span></span>     | <span data-ttu-id="1b681-118">Typ</span><span class="sxs-lookup"><span data-stu-id="1b681-118">Type</span></span>   |<span data-ttu-id="1b681-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b681-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b681-120">contentType</span><span class="sxs-lookup"><span data-stu-id="1b681-120">contentType</span></span>|<span data-ttu-id="1b681-121">String</span><span class="sxs-lookup"><span data-stu-id="1b681-121">String</span></span>|<span data-ttu-id="1b681-122">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="1b681-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="1b681-123">id</span><span class="sxs-lookup"><span data-stu-id="1b681-123">id</span></span>|<span data-ttu-id="1b681-124">String</span><span class="sxs-lookup"><span data-stu-id="1b681-124">String</span></span>| <span data-ttu-id="1b681-125">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="1b681-125">The attachment ID.</span></span>|
|<span data-ttu-id="1b681-126">isInline</span><span class="sxs-lookup"><span data-stu-id="1b681-126">isInline</span></span>|<span data-ttu-id="1b681-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b681-127">Boolean</span></span>|<span data-ttu-id="1b681-128">Legen Sie diesen auf „true“ fest, wenn es sich um eine Inlineanlage handelt, z. B. ein eingebettetes Bild innerhalb des Textkörpers des Elements.</span><span class="sxs-lookup"><span data-stu-id="1b681-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="1b681-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b681-129">lastModifiedDateTime</span></span>|<span data-ttu-id="1b681-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b681-130">DateTimeOffset</span></span>|<span data-ttu-id="1b681-131">Letzte Uhrzeit und letztes Datum der Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="1b681-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="1b681-132">name</span><span class="sxs-lookup"><span data-stu-id="1b681-132">name</span></span>|<span data-ttu-id="1b681-133">String</span><span class="sxs-lookup"><span data-stu-id="1b681-133">String</span></span>|<span data-ttu-id="1b681-134">Der Anzeigename der Anlage.</span><span class="sxs-lookup"><span data-stu-id="1b681-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="1b681-135">size</span><span class="sxs-lookup"><span data-stu-id="1b681-135">size</span></span>|<span data-ttu-id="1b681-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1b681-136">Int32</span></span>|<span data-ttu-id="1b681-137">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="1b681-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b681-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1b681-138">Relationships</span></span>
| <span data-ttu-id="1b681-139">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1b681-139">Relationship</span></span> | <span data-ttu-id="1b681-140">Typ</span><span class="sxs-lookup"><span data-stu-id="1b681-140">Type</span></span>   |<span data-ttu-id="1b681-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b681-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b681-142">item</span><span class="sxs-lookup"><span data-stu-id="1b681-142">item</span></span>|[<span data-ttu-id="1b681-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="1b681-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="1b681-p101">Die angefügte Nachricht oder das angefügte Ereignis. Navigation-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b681-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b681-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1b681-146">JSON representation</span></span>

<span data-ttu-id="1b681-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1b681-147">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
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
