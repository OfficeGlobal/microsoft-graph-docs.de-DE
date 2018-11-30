---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Zugriff auf freigegebene Elemente
ms.openlocfilehash: d3f6ef956501cded8af9ed641b2bb37666174cef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061674"
---
# <a name="accessing-shared-driveitems"></a>Zugriff auf freigegebene DriveItems

Verwenden Sie für den Zugriff auf ein freigegebenes [DriveItem](../resources/driveitem.md)-Element oder eine Sammlung freigegebener Elemente eine **shareId** oder Freigabe-URL.

Um eine Freigabe-URL mit dieser API verwenden zu können, muss die App [die URL in ein Freigabetoken konvertieren](#encoding-sharing-urls).

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.ReadWrite, Files.ReadWrite.All    |
|Anwendung | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a>Pfadparameter

| Parametername        | Wert    | Beschreibung                                                                         |
|:----------------------|:---------|:------------------------------------------------------------------------------------|
| **sharingTokenOrUrl** | `string` | Erforderlich. Ein Freigabetoken, wie es von der API oder einer ordnungsgemäß codierten Freigabe-URL zurückgegeben wird. |

### <a name="encoding-sharing-urls"></a>Codieren von Freigabe-URLs

Verwenden Sie zum Codieren einer Freigabe-URL die folgende Logik:

1. Als Erstes codieren Sie die URL mithilfe von Base64.
2. Konvertieren Sie das Base64-codierte Ergebnis in das [base64url-Format ohne Füllzeichen](https://en.wikipedia.org/wiki/Base64), indem Sie `=`-Zeichen vom Ende des Werts entfernen und `/` durch `_` sowie `+` durch `-` ersetzen.
3. Fügen Sie `u!` an den Anfang der Zeichenfolge an.

Beispiel für die Codierung einer URL in C#:

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine [sharedDriveItem](../resources/shareddriveitem.md)-Ressource im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

Im Folgenden finden Sie ein Beispiel für die Anforderung zum Abrufen eines freigegebenen Elements:

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET https://graph.microsoft.com/beta/shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.sharedDriveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  },
  "remoteItem": { 
    "driveId": "",
    "id": ""
  }
}
```

## <a name="access-the-shared-item-directly"></a>Direkter Zugriff auf das freigegebene Element

Obwohl das [**SharedDriveItem**](../resources/shareddriveitem.md)-Element nützliche Informationen enthält, möchten die meisten Apps direkt auf das freigegebene [DriveItem](../resources/driveitem.md)-Element zugreifen. Die **SharedDriveItem**-Ressource umfasst **root**- und **items**-Beziehungen, die innerhalb des Bereichs des freigegebenen Elements auf die Inhalte zugreifen können.

## <a name="example-single-file"></a>Beispiel (einzelne Datei)

### <a name="request"></a>Anforderung

Durch das Anfordern der **driveItem**-Beziehung wird das **DriveItem**-Element zurückgegeben, das freigegeben wurde.

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a>Antwort

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a>Beispiel (freigegebener Ordner)

### <a name="request"></a>Anforderung

Durch das Anfordern der **driveItem**-Beziehung und das Erweitern der **children**-Sammlung wird das freigegebene **DriveItem**-Element mit Dateien im freigegebenen Ordner zurückgegeben.

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET https://graph.microsoft.com/beta/shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a>Antwort

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {},
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="remarks"></a>Bemerkungen

* Bei OneDrive for Business und SharePoint erfordert die Freigabe-API immer eine Authentifizierung und kann nicht verwendet werden, um auf anonym freigegebene Inhalte ohne Benutzerkontext zuzugreifen.

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link"
} -->
