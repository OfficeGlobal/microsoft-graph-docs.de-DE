---
title: profilephoto aktualisieren
description: Aktualisieren Sie das Foto für jeden Benutzer in den Mandanten, einschließlich der angemeldeten Benutzer oder der angegebenen Gruppe oder des Kontakts. Seit dort
ms.openlocfilehash: 801ccd58e57cb02c1805f927dc22c9fd593cbae5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062866"
---
# <a name="update-profilephoto"></a>profilephoto aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Aktualisieren Sie das Foto für einen beliebigen Benutzer im Mandanten, einschließlich des angemeldeten Benutzers, der angegebenen Gruppe oder des angegebenen Kontakts. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe des Fotos, das Sie hinzufügen können, auf unter 4 MB beschränkt.

Verwenden Sie für diesen Vorgang nur PUT in der Betaversion.

> **Hinweis** Dieser Vorgang des Aktualisierens eines Fotos in der Betaversion unterstützt nur Geschäfts- oder Schulpostfächer eines Benutzers, keine persönlichen Postfächer.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | Profilfoto des angemeldeten **Benutzers**:<br/>User.ReadWrite User.ReadWrite.All<br /><br />Für **group**-Ressource:<br />Group.ReadWrite.All<br /><br />Für **contact**-Ressource:<br />Contacts.ReadWrite |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Für **user**-Ressource:<br/>User.ReadWrite.All<br /><br />Für **group**-Ressource:<br />Group.ReadWrite.All<br /><br />Für **contact**-Ressource:<br />Contacts.ReadWrite |

> **Hinweis** Um das Foto eines Benutzers in der Organisation zu aktualisieren, muss Ihre App über die User.ReadWrite.All-Anwendungsberechtigung verfügen und diese API unter ihrer eigenen Identität und nicht im Auftrag eines Benutzers aufrufen. Weitere Informationen hierzu finden Sie unter [Zugriff ohne einen angemeldeten Benutzer erlangen](/graph/auth-v2-service).

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | image/jpeg. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Fügen Sie in den Anforderungstext die Binärdaten des Fotos ein.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
