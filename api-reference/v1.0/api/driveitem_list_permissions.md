---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Liste mit Zugriff auf eine Datei
ms.openlocfilehash: 8b8671fbad37601a42127119f8bef6e5eca23dea
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="list-sharing-permissions-on-a-driveitem"></a>Auflisten von Berechtigungen für ein DriveItem

Listen Sie geltende Freigabe-Berechtigungen für ein [DriveItem](../resources/driveitem.md) auf.

## <a name="access-to-sharing-permissions"></a>Zugriff auf Freigabe-Berechtigungen

Die Berechtigungssammlung umfasst potenziell vertrauliche Informationen und ist möglicherweise nicht für alle Aufrufer verfügbar.

* Für den Besitzer des Elements werden alle Freigabe-Berechtigungen zurückgegeben. Dies umfasst Mitbesitzer.
* Für Aufrufer, die keine Besitzer sind, werden nur die Freigabe-Berechtigungen zurückgegeben, die für den Aufrufer gelten.
* Freigabe-Berechtigungseigenschaften, die Geheimnisse enthalten (z. B. `shareId` und `webUrl`), werden nur für Aufrufer zurückgegeben, die Freigabe-Berechtigungen erstellen können.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Anwendung | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die `$select` [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.

## <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name          | Typ   | Beschreibung                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | string | Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen eTag in dem Element übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben. |

## <a name="response"></a>Antwort

Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und eine Sammlung von [Permission](../resources/permission.md)-Ressourcen im Antworttext zurück.

Geltende Freigabe-Berechtigungen eines DriveItem können aus zwei Quellen stammen:

* Freigabe-Berechtigungen, die direkt für das DriveItem selbst gelten
* Freigabe-Berechtigungen, die von Vorgänger-DriveItems geerbt werden

Aufrufer können prüfen, ob die Berechtigung geerbt wurde, indem sie die **inheritedFrom**-Eigenschaft prüfen. Diese Eigenschaft ist eine [**itemReference**](../resources/itemreference.md)-Ressource, die auf das Vorgängerelement verweist, von dem die Berechtigung vererbt wurde.

SharePoint-Berechtigungsstufen, die für ein Element festgelegt wurden, werden mit der Präfix „SP“ zurückgegeben. Zum Beispiel SP.Nur anzeigen, SP.Beschränkter Zugriff, SP.Web Analytics-Daten anzeigen. Weitere Informationen finden Sie unter [Vollständige Liste der SharePoint-Rollen](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).

## <a name="example"></a>Beispiel

In diesem Beispiel wird die Sammlung von Berechtigungen für ein Element auf dem Laufwerk des angemeldeten Benutzers abgerufen.

<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/permissions
```

### <a name="response"></a>Antwort

Diese Beispielantwort umfasst drei Berechtigungen, bei der ersten handelt es sich um einen Freigabelink mit Bearbeitungsberechtigungen, bei der zweiten handelt es sich um eine ausdrückliche Berechtigung für einen Benutzer mit dem Namen John, die von einem übergeordneten Ordner vererbt wurde und bei der dritten handelt es sich um einen Freigabelink mit Lese-/Schreibberechtigung, der von einer Anwendung erstellt wurde.

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "Contoso Time Manager"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>Hinweise

Die **permissions**-Beziehungen eines DriveItem-Elements können nicht im Rahmen eines Aufrufs von [get DriveItem](driveitem_get.md) oder einer Sammlung von DriveItems erweitert werden. Sie müssen direkt auf die permissions-Eigenschaft zugreifen.

## <a name="error-responses"></a>Fehlerantworten

Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions"
} -->
