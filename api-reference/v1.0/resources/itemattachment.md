---
title: itemAttachment-Ressourcentyp
description: 'Kontakt, Ereignis oder Nachricht, die an ein anderes Ereignis, eine andere Nachricht oder einen anderen Beitrag angefügt sind.  '
ms.openlocfilehash: 79097b10327d895a41090e068a2fd8e9681df125
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017875"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="02533-103">itemAttachment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="02533-103">itemAttachment resource type</span></span>

<span data-ttu-id="02533-104">Kontakt, Ereignis oder Nachricht, die an ein anderes Ereignis, eine andere Nachricht oder einen anderen Beitrag angefügt sind.</span><span class="sxs-lookup"><span data-stu-id="02533-104">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="02533-105">Abgeleitet von [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="02533-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="02533-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="02533-106">Methods</span></span>

| <span data-ttu-id="02533-107">Methode</span><span class="sxs-lookup"><span data-stu-id="02533-107">Method</span></span>       | <span data-ttu-id="02533-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="02533-108">Return Type</span></span>  |<span data-ttu-id="02533-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02533-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02533-110">Get</span><span class="sxs-lookup"><span data-stu-id="02533-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="02533-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="02533-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="02533-112">Dient zum Lesen der Eigenschaften und der Beziehungen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="02533-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="02533-113">Delete</span><span class="sxs-lookup"><span data-stu-id="02533-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="02533-114">Keine</span><span class="sxs-lookup"><span data-stu-id="02533-114">None</span></span> |<span data-ttu-id="02533-115">Dient zum Löschen des itemAttachment-Objekts.</span><span class="sxs-lookup"><span data-stu-id="02533-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="02533-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="02533-116">Properties</span></span>
| <span data-ttu-id="02533-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02533-117">Property</span></span>     | <span data-ttu-id="02533-118">Typ</span><span class="sxs-lookup"><span data-stu-id="02533-118">Type</span></span>   |<span data-ttu-id="02533-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02533-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02533-120">contentType</span><span class="sxs-lookup"><span data-stu-id="02533-120">contentType</span></span>|<span data-ttu-id="02533-121">String</span><span class="sxs-lookup"><span data-stu-id="02533-121">String</span></span>|<span data-ttu-id="02533-122">Der Inhaltstyp der Anlage.</span><span class="sxs-lookup"><span data-stu-id="02533-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="02533-123">id</span><span class="sxs-lookup"><span data-stu-id="02533-123">id</span></span>|<span data-ttu-id="02533-124">String</span><span class="sxs-lookup"><span data-stu-id="02533-124">String</span></span>| <span data-ttu-id="02533-125">Die Anlagen-ID.</span><span class="sxs-lookup"><span data-stu-id="02533-125">The attachment ID.</span></span>|
|<span data-ttu-id="02533-126">isInline</span><span class="sxs-lookup"><span data-stu-id="02533-126">isInline</span></span>|<span data-ttu-id="02533-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="02533-127">Boolean</span></span>|<span data-ttu-id="02533-128">Legen Sie diesen auf „true“ fest, wenn es sich um eine Inlineanlage handelt, z. B. ein eingebettetes Bild innerhalb des Textkörpers des Elements.</span><span class="sxs-lookup"><span data-stu-id="02533-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="02533-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02533-129">lastModifiedDateTime</span></span>|<span data-ttu-id="02533-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02533-130">DateTimeOffset</span></span>|<span data-ttu-id="02533-131">Letzte Uhrzeit und letztes Datum der Änderung der Anlage.</span><span class="sxs-lookup"><span data-stu-id="02533-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="02533-132">name</span><span class="sxs-lookup"><span data-stu-id="02533-132">name</span></span>|<span data-ttu-id="02533-133">String</span><span class="sxs-lookup"><span data-stu-id="02533-133">String</span></span>|<span data-ttu-id="02533-134">Der Anzeigename der Anlage.</span><span class="sxs-lookup"><span data-stu-id="02533-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="02533-135">size</span><span class="sxs-lookup"><span data-stu-id="02533-135">size</span></span>|<span data-ttu-id="02533-136">Int32</span><span class="sxs-lookup"><span data-stu-id="02533-136">Int32</span></span>|<span data-ttu-id="02533-137">Die Größe der Anlage in Byte.</span><span class="sxs-lookup"><span data-stu-id="02533-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02533-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="02533-138">Relationships</span></span>
| <span data-ttu-id="02533-139">Beziehung</span><span class="sxs-lookup"><span data-stu-id="02533-139">Relationship</span></span> | <span data-ttu-id="02533-140">Typ</span><span class="sxs-lookup"><span data-stu-id="02533-140">Type</span></span>   |<span data-ttu-id="02533-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02533-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02533-142">item</span><span class="sxs-lookup"><span data-stu-id="02533-142">item</span></span>|[<span data-ttu-id="02533-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="02533-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="02533-p101">Die angefügte Nachricht oder das angefügte Ereignis. Navigation-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02533-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02533-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="02533-146">JSON representation</span></span>

<span data-ttu-id="02533-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="02533-147">Here is a JSON representation of the resource</span></span>

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
