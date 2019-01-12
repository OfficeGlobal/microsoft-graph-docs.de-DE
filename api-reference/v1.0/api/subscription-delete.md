---
title: Abonnement löschen
description: Mit dieser API können Sie Abonnements löschen.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: eeed4a7f6981a89a1869257bed339eb6895f25b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932581"
---
# <a name="delete-subscription"></a>Abonnement löschen

Mit dieser API können Sie Abonnements löschen.

## <a name="permissions"></a>Berechtigungen

In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Ressourcentyp/Element        | Berechtigung          |
|-----------------------------|---------------------|
| Kontakte                    | Contacts.Read       |
| Unterhaltungen               | Group.Read.All      |
| Ereignisse                      | Calendars.Read      |
| Nachrichten                    | Mail.Read           |
| Gruppen                      | Group.Read.All      |
| Benutzer                       | User.Read.All       |
| Laufwerk (OneDrive eines Benutzers)    | Files.ReadWrite     |
| Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke) | Files.ReadWrite.All |
|Sicherheitshinweis| SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a>Anforderungsheader

| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
