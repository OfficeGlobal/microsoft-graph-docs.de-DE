---
title: fileAttachment-Ressourcentyp
description: Eine Datei (beispielsweise eine Textdatei oder Word-Dokument), ein Ereignis zugeordnet ist,
localization_priority: Normal
ms.openlocfilehash: 7f7270bd5392e2d880daeb45491f4c65e9fca198
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869279"
---
# <a name="fileattachment-resource-type"></a>fileAttachment-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Datei (beispielsweise eine Textdatei oder Word-Dokument), ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md)zugeordnet ist. Die **ContentBytes** -Eigenschaft enthält die base64-codierten Inhalt der Datei.  

Fügen Sie beim Erstellen einer Dateianlage Folgendes zum Anforderungstext hinzu:

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* Die erforderlichen Eigenschaften **name** und **contentBytes**.

Abgeleitet von [attachment](attachment.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen](../api/attachment-get.md) | [fileAttachment](fileattachment.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des fileAttachment-Objekts.|
|[Delete](../api/attachment-delete.md) | Keine |Löscht das fileAttachment-Objekt. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|contentBytes|Binär|Der base64-codierte Inhalt der Datei.|
|contentId|Zeichenfolge|Die ID der Anlage im Exchange-Speicher.|
|contentLocation|Zeichenfolge|Der URI (Uniform Resource Identifier), der dem Speicherort des Anlageninhalts entspricht.|
|contentType|Zeichenfolge|Der Inhaltstyp der Anlage.|
|id|Zeichenfolge|Die Anlagen-ID.|
|isInline|Boolean|True, wenn es sich um eine Inlineanlage handelt.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Anlage.|
|name|Zeichenfolge|Der Name, der den Text darstellt, der unter dem Symbol für die eingebettete Anlage angezeigt wird. Dies muss nicht der tatsächliche Dateiname sein.|
|size|Int32|Die Größe der Anlage in Byte.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
  "contentId": "string",
  "contentLocation": "string",
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
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
