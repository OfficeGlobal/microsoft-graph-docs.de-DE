---
title: 'Domäne: ForceDelete'
description: Löscht eine Domäne mithilfe eines asynchronen Vorgangs.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5a1a2b2510f0c79f2be4e70deb9efabc65f8dfc4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527689"
---
# <a name="domain-forcedelete"></a>Domäne: ForceDelete

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Löscht eine Domäne mithilfe eines asynchronen Vorgangs.

Im Rahmen dieses Vorgangs werden die folgenden Aktionen ausgeführt:

* Benennt den UPN, EmailAddress und ProxyAddress von Benutzern durch Verweise auf die gelöschte Domäne.

* Benennt das EmailAddress-Gruppen mit Verweisen auf die gelöschte Domäne.

* Benennt die IdentifierUris von Anwendungen mit Verweisen auf die gelöschte Domäne.

* Wenn die Anzahl der Objekte umbenannt werden größer als 1000 ist, wird ein Fehler zurückgegeben.

* Wenn eine der Anwendungen umbenannt werden eine mehrinstanzenfähige app ist, wird ein Fehler zurückgegeben.

Nach Abschluss der Löschvorgang Domäne gibt API-Vorgänge für die gelöschten Domäne ein 404 HTTP-Antwort-Code zurück. Zum Löschen einer Domäne zu bestätigen, können Sie die [erste Domäne](domain-get.md)ausführen. Wenn die Domäne erfolgreich gelöscht wurde, wird ein 404 HTTP-Antwort-Code in der Antwort zurückgegeben werden soll.

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

| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich.|
| Content-Type  | application/json |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|disableUserAccounts|Boolescher Wert| Option zum Deaktivieren von Benutzerkonten umbenannt. Wenn ein Benutzerkonto deaktiviert ist, wird der Benutzer nicht zulässig ist so melden Sie sich.<br>*"True"* (Standard) - Benutzer, die im Rahmen dieses Vorgangs umbenannte Konten deaktiviert wurden.<br>*False* - Benutzerkonten, die im Rahmen dieses Vorgangs umbenannt werden nicht deaktiviert. |

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. 

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

##### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
