---
title: Ressourcentyp attachment
description: Sie können ein Ereignis verwandten Inhalten hinzugefügt
ms.openlocfilehash: f0bb9ec37d2fe3d034dce9532ad316d371c4937e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065477"
---
# <a name="attachment-resource-type"></a>Ressourcentyp attachment

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie können ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder in Form einer Anlage [Buchen](../resources/post.md) verwandten Inhalten hinzufügen.

**attachment** ist die Basisressource für die folgenden abgeleiteten Typen von Anlagen:

* Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)
* Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)
* Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)

## <a name="methods"></a>Methoden

Die folgenden Methoden gelten für alle abgeleiteten Typen von Anlagen (**fileAttachment**, **itemAttachment** oder **referenceAttachment**).

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Anlage abrufen](../api/attachment-get.md) | [attachment](attachment.md) |Lesen Sie die Eigenschaften und Beziehungen der Anlage, die ein Ereignis, Nachricht, Outlook-Aufgabe oder Post zugeordnet ist.|
|[Anlage einem Ereignis hinzufügen](../api/event-post-attachments.md) | [attachment](attachment.md) |Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Ereignis.|
|[Anlagen einer Nachricht hinzufügen](../api/message-post-attachments.md) | [attachment](attachment.md) |Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einer Nachricht.|
|[Hinzufügen einer Outlook-Aufgabe des Attachment-Objekts](../api/outlooktask-post-attachments.md) | [Anlage](attachment.md) |Hinzufügen einer Datei, Element oder Link Anlage zu einer Outlook-Aufgabe.|
|[Anlage einem Beitrag hinzufügen](../api/post-post-attachments.md) | [attachment](attachment.md) |Dient dem Hinzufügen einer Datei, eines Elements oder einer verknüpften Anlage zu einem Beitrag.|
|[Anlagen eines Ereignisses auflisten](../api/event-list-attachments.md) | [attachment](attachment.md) collection | Liste der Anlagen für ein Ereignis abrufen |
|[Anlagen einer Nachricht auflisten](../api/message-list-attachments.md) | [attachment](attachment.md) collection | Liste der Anlagen für eine Nachricht abrufen |
|[Liste von Anlagen eines Outlook-Aufgaben](../api/outlooktask-list-attachments.md) | [attachment](attachment.md) collection | Abrufen einer Liste von Anlagen für eine Outlook-Aufgabe. |
|[Anlagen eines Beitrags auflisten](../api/post-list-attachments.md) | [attachment](attachment.md) collection | Liste der Anlagen für einen Beitrag abrufen |
|[Löschen](../api/attachment-delete.md) | Keine |Löschen einer Anlage auf ein Ereignis, Nachricht, Outlook-Aufgabe oder Post. |

## <a name="properties"></a>Eigenschaften

Nachfolgend finden Sie die grundlegenden Eigenschaften von attachment-Ressourcen. Zusätzliche Eigenschaften finden Sie bei dem jeweiligen Anlagentyp ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) oder [referenceAttachment](../resources/referenceattachment.md)).

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|contentType|String|Der MIME-Typ.|
|id|String| Schreibgeschützt.|
|isInline|Boolean|`true`, wenn die Anlage eine Inlineanlage ist, andernfalls `false`.|
|lastModifiedDateTime|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|name|String|Der Anzeigename der Anlage. Dies muss nicht der tatsächliche Dateiname sein.|
|size|Int32|Die Länge der Anlage in Byte.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

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
