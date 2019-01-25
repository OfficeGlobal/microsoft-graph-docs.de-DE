---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Konvertieren in andere Formate
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8d65b7604c2ec17d4225c9cb887cbbfad2223009
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526305"
---
# <a name="download-a-file-in-another-format"></a>Herunterladen einer Datei in einem anderen Format

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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


Die folgenden Werte sind für den **Format** -Parameter gültig:

| Wert | Beschreibung                        | Unterstützte Quellerweiterungen
|:------|:-----------------------------------|---------------------------------
| GLB   | Das Element konvertiert in GLB-format  | Cool, Fbx, Obj, Blatt, Stl, 3mf
| html  | Das Element konvertiert in HTML-format | EML, Md, msg
| .jpg   | Das Element konvertiert in das JPG-format  | 3g 2, 3gp, 3gp2, 3gpp, 3mf, Ai, Arw, Asf, Avi, Bas, Bash, Bat, Bmp, c, Cbl, Cmd, Cool, Cpp, cr2, Crw, Cs, Css, Csv, übernehmen, dcm, dcm30, Dic, Dicm, Dicom, Dng, Doc, Docx, Dwg, Eml, Epi, Eps, Epsf, Epsi, Epub, Erf, Fbx, Fppx, Gif, Glb, h, hcp , Heic, Heif, Htm, html, Ico, Symbol, Java, Jfif, Jpeg, Jpg, Js, Json, Schlüssel, melden Sie sich, m2ts, m4a, m4v, Abzugsverteilung(en), Md, Mef, Mov, Film, MP3-, MP4 (engl.), mp4v, Mrw, msg, Mts, Nef, Nrw, Zahlen, Obj, Odp, Odt, Ogg, Orf, Seiten, Zusammenheften, Pdf, Pef, Php, Pict, pl, Blatt, Png, POT- , Potm, Potx, Pps, Ppsx, Ppsxm, ppt, Pptm, Pptx, Ps, ps1, Psb, Psd, hierhin, unformatiert, Rb, Rtf, rw1, rw2, sh skizzieren, Sql, sr2, Stl, Tif, Tiff, ts, Txt, Vb, Webm, Wma, Wmv, Xaml, Xbm, Xcf, xd, Xml, Xpm, Yaml, Yml
| PDF   | Konvertiert das Element ins PDF-Format.  | Doc, Docx, Epub, Eml, Htm, html, Md, msg, Odp, ods, Odt, PPS-, PPSX-, ppt, Pptx, Rtf, Tif, Tiff, Xls, Xlsm, Xlsx

## <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name            | Wert   | Beschreibung                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| _if-none-match_ | Zeichenfolge  | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben. |

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
