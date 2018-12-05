---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Erhalten von Berechtigungen
ms.openlocfilehash: 1964d291b6243ac286d5ac08a6bc48f3e576bbd3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065850"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a>Abrufen einer Freigabeberechtigung für eine Datei oder einen Ordner

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Geben Sie die geltende Freigabeberechtigung für eine bestimmte Berechtigungsressource zurück.

Geltende Berechtigungen eines Elements können aus zwei Quellen stammen: Berechtigungen, die direkt für das Element selbst festgelegt werden, oder Berechtigungen, die von den Vorgängern des Elements geerbt werden.

Aufrufer können prüfen, ob die Berechtigung geerbt wurde, indem sie die `inheritedFrom`-Eigenschaft prüfen. Diese Eigenschaft ist eine [ItemReference](../resources/itemreference.md)-Ressource, die auf das Vorgängerelement verweist, von dem die Berechtigung vererbt wurde.

SharePoint-Berechtigungsstufen, die für ein Element festgelegt wurden, werden mit der Präfix „SP“ zurückgegeben. Zum Beispiel SP.Nur anzeigen, SP.Beschränkter Zugriff, SP.Web Analytics-Daten anzeigen. Weitere Informationen finden Sie unter [Vollständige Liste der SharePoint-Rollen](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).

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
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die [$select-Abfrageparameter](/graph/query-parameters) zum Modellieren der Antwort.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [Berechtigungs](../resources/permission.md)-Ressource im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

Nachfolgend finden Sie ein Beispiel der Anforderung für den Zugriff auf eine Berechtigung zu einem Ordner.

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
```
### <a name="response"></a>Antwort

Bei Erfolg gibt diese Methode eine [Permission](../resources/permission.md)-Ressource für die angegebene ID zurück. 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a>Hinweise

Die [Permission](../resources/permission.md)-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die die Ressource dargestellt.

Berechtigungen für ein [**link**](../resources/sharinglink.md)-Facet stellen Freigabe-Links dar, die für das Element erstellt wurden. Freigabelinks enthalten ein eindeutiges Token, mit dem alle Benutzer, die über den Link verfügen, Zugriff auf das Element haben.

Berechtigungen mit einem [**invitation**](../resources/sharinginvitation.md)-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen für Zugriff auf die Datei hinzugefügt werden.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission"
}-->