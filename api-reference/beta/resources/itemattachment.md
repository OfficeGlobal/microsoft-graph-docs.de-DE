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
# <a name="itemattachment-resource-type"></a>itemAttachment-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Kontakt, ein Ereignis oder eine Nachricht, die an einem anderen [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md)angefügt ist.  

Abgeleitet von [attachment](attachment.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [itemAttachment](itemattachment.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des itemAttachment-Objekts.|
|[Delete](../api/attachment-delete.md) | Keine |Dient zum Löschen des itemAttachment-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|contentType|String|Der Inhaltstyp der Anlage.|
|id|String| Die Anlagen-ID.|
|isInline|Boolescher Wert|Legen Sie diesen auf „true“ fest, wenn es sich um eine Inlineanlage handelt, z. B. ein eingebettetes Bild innerhalb des Textkörpers des Elements.|
|lastModifiedDateTime|DateTimeOffset|Letzte Uhrzeit und letztes Datum der Änderung der Anlage.|
|name|String|Der Anzeigename der Anlage.|
|size|Int32|Die Größe der Anlage in Byte.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|item|[OutlookItem](outlookitem.md)|Das angefügte Kontakt Nachricht oder Ereignis. Navigationseigenschaft.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

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
