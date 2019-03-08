---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Konvertieren in andere Formate
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c3761525d0acbd5613a71519d9ebd56ab8475f03
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481825"
---
# <a name="download-a-file-in-another-format"></a>Datei in einem anderen Format herunterladen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mithilfe dieser API können Sie den Inhalt eines Elements in einem bestimmten Format abrufen.
Nicht jede Datei kann in sämtliche Formate konvertiert werden.

Informationen zum Herunterladen des Elements im ursprünglichen Format finden Sie unter [herunterladen der Inhalte eines Elements](driveitem-get-content.md).

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


Die folgenden Werte sind für den Parameter **Format** gültig:

| Wert | Beschreibung                        | Unterstützte Quellerweiterungen
|:------|:-----------------------------------|---------------------------------
| GLB   | Wandelt das Element in das GLB-Format um.  | cool, FBX, obj, Ply, STL, 3MF
| HTML  | Wandelt das Element in das HTML-Format um. | EML, MD, msg
| JPG   | Wandelt das Element in das JPG-Format um.  | 3G2, 3GP, 3GP2, 3GPP, 3MF, Ai, ARW, ASF, AVI, Bas, bash, bat, BMP, c, CBL, cmd, cool, cpp, CR2, CRW, CS, CSS, CSV, cur, DCM, dcm30, DIC, dicm, DICOM, DNG, doc, docx, DWG, eml, EPS, EPSF, epsi, , HEIC, heif, htm, HTML, ICO, Icon, Java, JFIF, JPEG, JPG, JS, JSON, Key, Log, M2TS, M4A, M4V, Abschlag, MD, MEF, MOV, Movie, MP3, MP4, MP4V, MRW, msg, MTS, NEF, NRW, Numbers, obj, Odp,------------------------- , POTM, POTX, PPS, PPSX, ppsxm, PPT, PPTM, PPTX, PS, PS1, PSB, PSD, PY, RAW, RB, RTF, RW1, RW2, sh, Sketch, SQL, SR2, STL, TIF, TIFF, TS, txt, WEBM, WMV,, XBM, XCF
| PDF   | Wandelt das Element in das PDF-Format um.  | doc, docx, ePub, eml, htm, HTML, MD, msg, Odp, ODS, ODT, PPS, PPSX, PPT, PPTX, RTF, TIF, TIFF, xls, XLSM

## <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name            | Wert   | Beschreibung                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | string  | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben. |

## <a name="example"></a>Beispiel

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
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

<!--
{
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-get-content-format.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
