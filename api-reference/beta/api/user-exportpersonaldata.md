---
title: 'Benutzer: ExportPersonalData'
description: Fordert die Daten Richtlinie Vorgang, versucht ein Unternehmensadministrator, eine Organisationseinheit Benutzerdaten exportieren.
localization_priority: Normal
ms.openlocfilehash: d660994868e331fb8c1813bb9ff90aebe4790e9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845339"
---
# <a name="user-exportpersonaldata"></a>Benutzer: ExportPersonalData

Fordert die Daten Richtlinie Vorgang, mit einem Unternehmensadministrator vorgenommenen Änderungen für eine Organisationseinheit Benutzerdaten exportieren.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  User.Export.All und User.Read.All  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht zutreffend  |
|Anwendung | User.Export.All und User.Read.All |

>**Hinweis:** Export kann nur von einem Unternehmensadministrator ausgeführt werden, wenn die delegierte Berechtigung verwendet wird.

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung |
|:---------------|:----------|
| Authorization  | Bearer {token}|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung |
|:---------------|:--------|:----------|
|storageLocation|String|Dies ist die URL einer gemeinsamen Zugriff Signatur (SAS) ein Konto Azure-Speicher an, in dem Daten exportiert werden sollen.|

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Es gibt keine Suchzeichenfolge im Antworttext zurück. Die Antwort enthält die folgenden Kopfzeilen.

| Name       | Beschreibung |
|:---------------|:----------|
| Location  | URL, die den Status der Anforderung überprüfen. |
| Wiederholen Sie den Vorgang nach  | Der Zeitraum in Sekunden. Anforderung Maker warten soll lange nach der Übermittlung einer Anforderung an den Status überprüfen. |


## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a>Antwort

```
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

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
