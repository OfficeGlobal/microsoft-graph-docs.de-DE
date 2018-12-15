---
title: 'Benutzer: ExportPersonalData'
description: Fordert die Daten Richtlinie Vorgang, versucht ein Unternehmensadministrator, eine Organisationseinheit Benutzerdaten exportieren.
ms.openlocfilehash: 7d41d6d855fee992a4ff3a542e6c11f692adcfe3
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2018
ms.locfileid: "27284133"
---
# <a name="user-exportpersonaldata"></a>Benutzer: ExportPersonalData

Fordern Sie ein Daten Richtlinie Vorgang aus ein Unternehmensadministrator oder einer Anwendung zum Exportieren von Daten für eine Organisationseinheit des Benutzers.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  User.Export.All User.Read.All  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht zutreffend  |
|Anwendung | User.Export.All User.Read.All |

>**Hinweis:** Der Exportvorgang kann nur von einem Unternehmensadministrator ausgeführt werden, wenn delegierte Berechtigungen verwendet werden.

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|storageLocation|String|Dies ist die URL einer gemeinsamen Zugriff Signatur (SAS) ein Konto Azure-Speicher an, in dem Daten exportiert werden sollen.|

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```

##### <a name="response"></a>Antwort
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
