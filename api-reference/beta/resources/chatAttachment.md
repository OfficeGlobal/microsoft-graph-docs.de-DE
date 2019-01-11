---
title: Ressourcentyp chatMessageAttachment
description: Stellt eine Anlage zu einer Chat Nachrichtenentität dar.
localization_priority: Normal
ms.openlocfilehash: 83574a7dbbb35f9c8b95474fac1154154f413470
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805558"
---
# <a name="chatmessageattachment-resource-type"></a>Ressourcentyp chatMessageAttachment

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Anlage zu einer Chat Nachrichtenentität dar.

Eine Entität vom Typ `chatMessageAttachment` wird als Teil des [ChatMessage](chatmessage.md) -Entität als Teil des [Kanalnachrichten abrufen](../api/channel-list-messages.md) -API zurückgegeben.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string| Schreibgeschützt. Eindeutige Id der Anlage|
|contentType| string | Der Medientyp der Content Anlage. Sie können die folgenden Werte aufweisen: <br><ul><li>Referenz: Anlage ist eine Verknüpfung zu einer anderen Datei. Füllen Sie die ContentURL mit den Link, um das Objekt<br></li><li>Datei: unformatierte Dateianlage. Füllen Sie das Feld Contenturl mit base64-Codierung der Datei im Data: Format<br></li><li>Bild /: Bildtyp mit dem Typ des Bilds angegeben: Image/Png, Image/Jpeg, Image/Gif. Füllen Sie das Feld ContentUrl mit base64-Codierung der Datei im Data: Format<br></li><li>Video /: Videotyp mit dem angegebenen Format. Beispiel: Video/mp4. Füllen Sie das Feld ContentUrl mit base64-Codierung der Datei im Data: Format<br></li><li>Audio-/: Audio-Typ, mit dem angegebenen Format. Beispiel: Audio-/Wmw. Füllen Sie das Feld ContentUrl mit base64-Codierung der Datei im Data: Format<br></li><li>Anwendung/Kartentyp: Rich Karte Anlagetyp mit den Kartentyp angeben das genaue Kartenformat verwenden. Legen Sie Inhalt mit der Karte Json-Format. Unterstützte Werte für Kartentyp:<br><ul><li>application/vnd.Microsoft.Card.Adaptive: eine umfassende Karte, die eine beliebige Kombination von Text, Sprache, Bilder,, Schaltflächen und Felder enthalten kann. Legen Sie die Content-Eigenschaft, um ein AdaptiveCard-Objekt.</li><li>application/vnd.Microsoft.Card.Animation: eine umfassende Karte, die Animation wiedergegeben wird. Legen Sie die Content-Eigenschaft auf eine AnimationCardobject.</li><li>application/vnd.Microsoft.Card.Audio: eine umfassende Karte, die Wiedergabe von Audiodateien. Legen Sie die Content-Eigenschaft auf ein AudioCard-Objekt.</li><li>application/vnd.Microsoft.Card.Video: eine umfassende Karte, die Videos wiedergegeben wird. Legen Sie die Content-Eigenschaft auf ein Objekt Videokarte.</li><li>application/vnd.Microsoft.Card.Hero: eine Karte Textlinks. Legen Sie die Content-Eigenschaft auf ein HeroCard-Objekt.</li><li>application/vnd.Microsoft.Card.Thumbnail: eine Karte Miniaturansicht. Legen Sie die Content-Eigenschaft auf ein ThumbnailCard-Objekt.</li><li>application/vnd.Microsoft.com.Card.Receipt: eine Bestätigung Karte. Legen Sie die Content-Eigenschaft auf ein ReceiptCard-Objekt.</li><li>application/vnd.Microsoft.com.Card.SignIn: ein Benutzer anmelden Karte. Legen Sie die Content-Eigenschaft auf ein SignInCard-Objekt.</ul></ul>|
|contentUrl|string|URL für den Inhalt der Anlage. Unterstützte Protokolle: http, Https, Datei und Daten|
|content|string|Der Inhalt der Anlage. Wenn die Anlage eine umfangreiche Karte ist, legen Sie die-Eigenschaft auf das rich-Karte-Objekt. Diese Eigenschaft und ContentUrl schließen sich gegenseitig aus|
|name|string|Name der Anlage|
|thumbnailUrl| string |URL zu einer ein Miniaturbild, die der DDE-Kanal verwenden können, wenn es unterstützt die Verwendung eines alternativen, kleineren-Formulars des Inhalts oder ContentUrl. Angenommen, wenn Sie ContentType auf/Word-Anwendung und ContentUrl an den Speicherort des Word-Dokuments festgelegt, Sie ein Miniaturbild enthalten können, die das Dokument darstellt. Der Kanal konnte das Miniaturbild statt des Dokuments angezeigt werden. Wenn der Benutzer das Bild klickt, würde der Kanal das Dokument geöffnet.|

## <a name="json-representation"></a>JSON-Darstellung
 Der folgende Code ist ein JSON-Darstellung der Ressource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageAttachment"
}-->

```json
{
  "id": "string (identifier)",
  "contentType": "string",
  "contentUrl": "string",
  "content": "string",
  "name": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
