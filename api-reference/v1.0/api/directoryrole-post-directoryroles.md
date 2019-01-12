---
title: directoryRole aktivieren
description: Dient zum Aktivieren einer Verzeichnisrolle. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren und die impliziten Benutzerverzeichnisrollen sind standardmäßig aktiviert. Um auf Mitglieder zuzugreifen und diese einer anderen Verzeichnisrolle zuzuweisen, müssen Sie diese zuerst mit der entsprechenden Verzeichnisrollenvorlage aktivieren (directoryRoleTemplate).
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d127580c0a4851c5a991ccc0646007ddf1298a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924916"
---
# <a name="activate-directoryrole"></a>directoryRole aktivieren

Dient zum Aktivieren einer Verzeichnisrolle. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren und die impliziten Benutzerverzeichnisrollen sind standardmäßig aktiviert. Um auf Mitglieder zuzugreifen und diese einer anderen Verzeichnisrolle zuzuweisen, müssen Sie diese zuerst mit der entsprechenden Verzeichnisrollenvorlage aktivieren ([directoryRoleTemplate](../resources/directoryroletemplate.md)).

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |
| Content-Type  | string  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Aktivieren einer Verzeichnisrolle erforderlich sind.

|Parameter | Typ | Beschreibung|
|:---------|:---------|:---------|
|roleTemplateId | string | Erforderlich. Die ID des der [DirectoryRoleTemplate](../resources/directoryroletemplate.md) , die die Rolle basiert. Dies ist die einzige Eigenschaft, die in der Anforderung angegeben werden können.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.
##### <a name="response"></a>Antwort
Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
