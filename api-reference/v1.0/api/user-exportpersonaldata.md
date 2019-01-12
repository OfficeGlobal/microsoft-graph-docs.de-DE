---
title: 'Benutzer: ExportPersonalData'
description: Fordert die Daten Richtlinie Vorgang, versucht ein Unternehmensadministrator, eine Organisationseinheit Benutzerdaten exportieren.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba26d2b2bc5af63f01a4333490d9850ffa3dd767
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954302"
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
|storageLocation|Zeichenfolge|Dies ist die URL einer gemeinsamen Zugriff Signatur (SAS) ein Konto Azure-Speicher an, in dem Daten exportiert werden sollen.|

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Es gibt keine Suchzeichenfolge im Antworttext zurück. Die Antwort enthält die folgenden Antwortheader.

| Name       | Beschreibung|
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
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a>Antwort

```
{
  Location: https://graph.microsoft.com/v1.0/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
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
