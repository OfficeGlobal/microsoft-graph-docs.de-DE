---
title: Domäne löschen erzwingen
description: Löscht eine Domäne mithilfe eines asynchronen Vorgangs langer.
author: lleonard-msft
ms.openlocfilehash: 85839d8bf7d36925661d0202c053574288763dc6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309114"
---
# <a name="force-domain-deletion"></a>Domäne löschen erzwingen

Löscht eine Domäne mithilfe eines asynchronen Vorgangs langer.

Im Rahmen dieses Vorgangs werden die folgenden Aktionen ausgeführt:

* Updates der `userPrincipalName`, `mail`, und `proxyAddresses` Eigenschaften des `users` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.

* Updates der `mail` -Eigenschaft des `groups` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.

* Updates der `identifierUris` -Eigenschaft des `applications` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.

* Wenn die Anzahl der Objekte umbenannt werden größer als 1000 ist, wird ein Fehler zurückgegeben.

* Wenn eine von der `applications` umbenannt werden, ist eine app mit mehreren Mandanten, wird ein Fehler zurückgegeben.

Nach Abschluss der Löschvorgang Domäne gibt API-Vorgänge für die gelöschten Domäne einen HTTP 404-Statuscode zurück. Zum Löschen einer Domäne zu bestätigen, können Sie einen Vorgang [Abrufen Domäne](domain-get.md) ausführen.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.

## <a name="request-headers"></a>Anforderungsheader

| Name | Beschreibung |
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich.|
| Content-Type  | application/json |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter | Typ | Beschreibung |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| Option zum Deaktivieren von Benutzerkonten die umbenannt werden. Wenn ein Benutzerkonto deaktiviert ist, wird der Benutzer nicht zulässig ist so melden Sie sich. Wenn auf **true** festgelegt, die `users` als Teil von diesem Vorgang wird deaktiviert werden aktualisiert.  Standardwert ist **true**. |

## <a name="response-body"></a>Antworttext

Wenn der Vorgang erfolgreich war, gibt diese Methode `HTTP/1.1 204 OK` Statuscode.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->