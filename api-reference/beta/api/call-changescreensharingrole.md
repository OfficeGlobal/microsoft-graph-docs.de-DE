---
title: 'Rufen Sie: ChangeScreenSharingRole'
description: Starten Sie und beenden Sie die Freigabe Bildschirm in den Anruf. Diese API wird verwendet, um Bildschirm Freigeben von Inhalten mit den Teilnehmern für einen Anruf oder eine Besprechung zu ermöglichen.
author: VinodRavichandran
ms.openlocfilehash: 4b4c7e0afa452bef414dd466086463aa16c9d9cf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328364"
---
# <a name="call-changescreensharingrole"></a>Rufen Sie: ChangeScreenSharingRole

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Starten Sie und beenden Sie die Freigabe Bildschirm in den Anruf. Diese API wird verwendet, um Bildschirm Freigeben von Inhalten mit den Teilnehmern für einen Anruf oder eine Besprechung zu ermöglichen.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
|:---------------------------------------|:--------------------------------------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Nicht unterstützt                               |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt                               |
| Anwendung                            | Calls.AccessMedia.All                       |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a>Anforderungsheader
| Name          | Beschreibung               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter      | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|role|String|Mögliche Werte sind: 'Viewer', 'Mitbenutzenden'|

## <a name="response"></a>Antwort
Gibt `202 Accepted` Antwortcode.

## <a name="example"></a>Beispiel
Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.

##### <a name="request"></a>Anforderung
Das folgende Beispiel zeigt die Antwort.

<!-- {
  "blockType": "request",
  "name": "call_changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
