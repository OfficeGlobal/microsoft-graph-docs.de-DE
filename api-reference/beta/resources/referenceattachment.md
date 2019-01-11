---
title: referenceAttachment-Ressourcentyp
description: 'Einen Link zu einem Ordner oder Datei (beispielsweise eine Textdatei oder Word-Dokument) auf einen OneDrive for Business Cloud Laufwerk oder andere unterstützte Speicherorte, zugeordnet ist '
localization_priority: Normal
ms.openlocfilehash: 6a334b303bea7aff768733434b9ba882de237a12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880052"
---
# <a name="referenceattachment-resource-type"></a>referenceAttachment-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Link zur Datei (beispielsweise eine Textdatei oder Word-Dokument) in eine OneDrive for Business Cloud Laufwerk oder eine andere oder eines Ordners unterstützt Speicherorte, ein [Ereignis](../resources/event.md), [Nachricht](../resources/message.md), [Outlook-Aufgabe](../resources/outlooktask.md)oder [Buchen](../resources/post.md) zugeordnet ist.

Abgeleitet von [attachment](attachment.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des referenceAttachment-Objekts.|
|[Delete](../api/attachment-delete.md) | Keine |Dient zum Löschen des referenceAttachment-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|contentType|Zeichenfolge|Der Inhaltstyp der Anlage. Optional.|
|id|Zeichenfolge|Die Anlagen-ID.  Schreibgeschützt.|
|isFolder|Boolescher Wert|Gibt an, ob die Anlage eine Verknüpfung zu einem Ordner ist. Setzen Sie müssen diese auf "true" Wenn **SourceUrl** eine Verknüpfung zu einem Ordner ist. Optional.|
|isInline|Boolescher Wert|Wird auf „true“ festgelegt, wenn die Anlage inline im Text des einbettenden Objekts angezeigt wird. Optional.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Anlage. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Optional.|
|name|Zeichenfolge|Der Text, der unterhalb des Symbols, das die eingebettete Anlage darstellt angezeigt wird. Dies muss nicht der tatsächliche Dateiname sein. Erforderlich.|
|Berechtigung|ReferenceAttachmentPermissions|Gibt die Berechtigungen für die Anlage durch den Typ des Anbieters in **ProviderType**erteilt. Mögliche Werte sind: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView` und `organizationEdit`. Optional.|
|previewUrl|Zeichenfolge|Betrifft nur eine Referenz Anlage ein Bild - URL, um ein Vorschaubild abzurufen. Verwenden Sie **ThumbnailUrl** und **PreviewUrl** nur, wenn **SourceUrl** eine Bilddatei identifiziert. Optional.|
|providerType|ReferenceAttachmentProviders|Der Typ der Anbieter, der eine Anlage von diesem ContentType unterstützt. Mögliche Werte: sind `other`, `oneDriveBusiness`, `oneDriveConsumer` und `dropbox`. Optional.|
|size|Int32|Die Größe der Metadaten in Bytes, die für die Nachricht für die Anlage Verweis gespeichert ist. Dieser Wert gibt nicht die Größe der tatsächlichen Datei an. Optional.|
|SourceUrl|Zeichenfolge|URL, um den Inhalt der Anlage abzurufen. Ist dies eine URL zu einem Ordner, legen Sie dann für den Ordner in Outlook oder Outlook im Web ordnungsgemäß anzuzeigende **IsFolder** auf "true". Erforderlich.|
|thumbnailUrl|Zeichenfolge|Betrifft nur eine Referenz Anlage ein Bild - URL ein Miniaturbild abgerufen. Verwenden Sie **ThumbnailUrl** und **PreviewUrl** nur, wenn **SourceUrl** eine Bilddatei identifiziert. Optional.|

## <a name="relationships"></a>Beziehungen
Keine



## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isFolder": true,
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "permission": "string",
  "previewUrl": "string",
  "providerType": "string",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
