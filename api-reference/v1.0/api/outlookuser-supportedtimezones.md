---
title: 'outlookUser: supportedTimeZones'
description: Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c9c90ea56b1c0924ec91436733c99c67333b99d5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981714"
---
# <a name="outlookuser-supportedtimezones"></a>outlookUser: supportedTimeZones

Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert.

Sie können explizit angeben, dass Zeitzonen im Windows-Zeitzonenformat oder im [IANA-Format (Internet Assigned Numbers Authority)](https://www.iana.org/time-zones) (auch als Olson-Zeitzone bezeichnet) zurückgegeben werden. Das Windows-Format ist die Standardeinstellung.

Beim Einrichten eines Outlook-Clients wählt der Benutzer die bevorzugte Zeitzone aus dieser unterstützten Liste aus. Sie können anschließend die bevorzugte Zeitzone abrufen, indem Sie [die Postfacheinstellungen des Benutzers abrufen](user-get-mailboxsettings.md).


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.Read, User.ReadBasic.All    |
|Delegiert (persönliches Microsoft-Konto) | User.Read    |
|Anwendung | User.Read.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a>Funktionsparameter
| Parameter       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| TimeZoneStandard  | timeZoneStandard  | Ein Zeitzonenformat. Unterstützte Werte sind: `Windows` und `Iana`. Optional. |

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von [timeZoneInformation](../resources/timezoneinformation.md)-Objekten im Antworttext zurück.

## <a name="example"></a>Beispiel

##### <a name="request-1"></a>Anforderung 1
Im folgenden Beispiel wird der `timeZoneStandard`-Parameter nicht angegeben, und es wird eine Liste unterstützter Zeitzonen abgerufen, die im Windows-Zeitzonenformat dargestellt werden. 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a>Antwort 1
Nachfolgend sehen Sie ein Beispiel der Antwort. 
<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_default",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Dateline Standard Time",
      "displayName":"(UTC-12:00) International Date Line West"
    },
    {
      "alias":"Samoa Standard Time",
      "displayName":"(UTC+13:00) Samoa"
    },
    {
       "alias":"UTC-11",
       "displayName":"(UTC-11:00) Coordinated Universal Time-11"
    },
    {
      "alias":"Aleutian Standard Time",
      "displayName":"(UTC-10:00) Aleutian Islands"
    }
  ]
}
```

##### <a name="request-2"></a>Anforderung 2
Im folgenden Beispiel wird `Iana` für den `TimeZoneStandard`-Parameter angegeben und die Liste der unterstützten Zeitzonen abgerufen, die im IANA-Format dargestellt werden. 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a>Antwort 2
Nachfolgend sehen Sie ein Beispiel der Antwort. 

<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_iana",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Etc/GMT+12",
      "displayName":"Etc/GMT+12"
    },
    {
      "alias":"US/Samoa",
      "displayName":"US/Samoa"
    },
    {
      "alias":"Etc/GMT+11",
      "displayName":"Etc/GMT+11"
    },
    {
      "alias":"US/Aleutian",
      "displayName":"US/Aleutian"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
