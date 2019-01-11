---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Konvertieren in andere Formate
localization_priority: Priority
ms.openlocfilehash: 86210d4364f771d2bf6f8d0ebbdd70634521cd67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812411"
---
# <a name="download-a-file-in-another-format"></a>Herunterladen einer Datei in einem anderen Format

Mithilfe dieser API können Sie den Inhalt eines Elements in einem bestimmten Format abrufen.
Nicht jede Datei kann in sämtliche Formate konvertiert werden.

Wenn das Element im Originalformat herunterladen möchten, finden Sie unter [Herunterladen der Inhalt des Elements](driveitem-get-content.md).

## <a name="prerequisites"></a>Voraussetzungen

Damit diese API aufgerufen werden kann, muss der Benutzer der Anwendung Lesezugriff auf die Datei gewährt haben, die von der App konvertiert werden soll.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a>Abfrageparameter

| Parameter      | Typ  | Beschreibung                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| _format_  | string | Hier geben Sie das Format an, in dem der Elementinhalt heruntergeladen werden soll. |


### <a name="format-options"></a>Formatoptionen

Die folgenden Werte sind für den **Format** -Parameter gültig:

| Format-Wert | Beschreibung                        | Unterstützte Quellerweiterungen
|:-------------|:-----------------------------------|----------------------------
| pdf          | Konvertiert das Element ins PDF-Format. | CSV, DOC, DOCX, ODP, ODS, ODT, POT, POTM, POTX, PPS, PPSX, PPSXM, PPT, PPTM, PPTX, RTF, XLS, XLSX

## <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name            | Wert   | Beschreibung                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | Zeichenfolge  | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben. |

## <a name="example"></a>Beispiel

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```

## <a name="response"></a>Antwort

Die Methode gibt eine Antwort `302 Found` zurück, die auf eine vorab authentifizierte URL zum Download der konvertierten Datei umleitet.

Um die konvertierte Datei herunterladen zu können, muss die App den `Location`-Header in der Antwort aufrufen.

Vorab authentifizierte URLs sind nur für eine kurze Zeit gültig (einige Minuten) und erfordern für den Zugriff keinen `Authorization`-Header.

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a>Fehlerantworten

Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im unter [Fehlerantworten][error-response].

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
