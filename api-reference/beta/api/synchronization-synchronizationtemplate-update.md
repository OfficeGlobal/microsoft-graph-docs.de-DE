---
title: SynchronisationVorlage aktualisieren
description: Aktualisieren Sie (Override) die Synchronisierung-Vorlage mit einer bestimmten Anwendung verbunden sind.
ms.openlocfilehash: 9862b0a31294448e1b43e8438b76a16d471cb2d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065258"
---
# <a name="update-synchronizationtemplate"></a>SynchronisationVorlage aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Aktualisieren Sie (Override) die Synchronisierung-Vorlage mit einer bestimmten Anwendung verbunden sind.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     |Directory.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |Nicht unterstützt|
|Anwendung                            |Nicht unterstützt| 

### <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a>Anforderungsheader

| Name           | Typ    | Beschreibung|
|:---------------|:--------|:-----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Textkörper Anforderung das [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekt, um die vorhandene Vorlage ersetzt. Stellen Sie sicher, dass alle Eigenschaften vorhanden sind. Fehlende Eigenschaften werden gelöscht.

### <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

### <a name="examples"></a>Beispiele

##### <a name="request"></a>Anforderung
Es folgt ein Beispiel für eine Anforderung. 

>**Hinweis:** Das hier gezeigte Request-Objekt wird zur besseren Lesbarkeit gekürzt. Alle Eigenschaften in eine tatsächliche aufrufen einschließen.
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a>Antwort
Es folgt ein Beispiel für eine Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->