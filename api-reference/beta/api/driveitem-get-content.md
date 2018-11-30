---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Eine Datei herunterladen
ms.openlocfilehash: 8b86954bd2a07d7b476762c4baef36f4f7fb7cbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063138"
---
# <a name="download-the-contents-of-a-driveitem"></a>Inhalte von DriveItem herunterladen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Laden Sie die Inhalte des primären Streams (Datei) eines DriveItem herunter. Es können nur driveItems mit der Eigenschaft **file** heruntergeladen werden.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name          | Wert  | Beschreibung                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | String | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben. |

## <a name="example"></a>Beispiel

Dies ist ein Beispiel für das Herunterladen einer vollständigen Datei.


<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content
```

### <a name="response"></a>Antwort

Gibt eine `302 Found`-Antwort zurück, mit der zu einer zuvor authentifizierten Download-URL umgeleitet wird. Dies ist dieselbe URL, die `@microsoft.graph.downloadUrl`-Eigenschaft für DriveItem verfügbar ist.

Zum Herunterladen der Inhalte der Datei muss die Anwendung dem `Location`-Header in der Antwort folgen. Viele HTTP-Clientbibliotheken folgen automatisch der 302-Umleitung und beginnen sofort mit dem Download der Datei.

Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header für den Download.

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a>Teilbereichdownloads

Zum Herunterladen eines Teilbereichs von Bytes aus einer Datei kann die App den `Range`-Header gemäß der Angabe in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) verwenden. Sie müssen den `Range`-Header an die tatsächliche `@microsoft.graph.downloadUrl`-URL anfügen, und nicht an die Anforderung für `/content`.

<!-- { "blockType": "request", "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

Es wird eine `HTTP 206 Partial Content`-Antwort mit dem Anforderungsbereich von Bytes aus der Datei zurückgegeben. Wenn der Bereich nicht generiert werden kann, wird der Range-Header möglicherweise ignoriert und gibt eine `HTTP 200`-Antwort mit dem gesamten Inhalt der Datei zurück.

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048

<first 1024 bytes of file>
```

### <a name="error-responses"></a>Fehlerantworten

Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download"
} -->
