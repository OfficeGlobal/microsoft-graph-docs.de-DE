---
title: fileAttachment-Ressourcentyp
description: Eine Datei (beispielsweise eine Textdatei oder Word-Dokument), ein Ereignis zugeordnet ist,
localization_priority: Normal
ms.openlocfilehash: 5f7be9bca3114fc7e74be711dc606a278e0025ff
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572801"
---
# <a name="fileattachment-resource-type"></a>fileAttachment-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|contentBytes|String|Der base64-codierte Inhalt der Datei.|
|contentId|String|Die ID der Anlage im Exchange-Speicher.|
|contentLocation|String|Verwenden Sie diese Eigenschaft nicht auf, da es nicht unterstützt wird.|
|contentType|String|Der Inhaltstyp der Anlage.|
|id|String|Die Anlagen-ID.|
|isInline|Boolean|True, wenn es sich um eine Inlineanlage handelt.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Anlage.|
|name|String|Der Name, der den Text darstellt, der unter dem Symbol für die eingebettete Anlage angezeigt wird. Dies muss nicht der tatsächliche Dateiname sein.|
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
  "contentBytes": "String",
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
<!--
{
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/fileattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
