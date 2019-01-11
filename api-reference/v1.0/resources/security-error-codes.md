---
title: Microsoft Graph Sicherheit API Fehlerantworten
description: Fehler in der Microsoft Graph Sicherheit API werden mithilfe des standard 206 teilweise von HTTP-Statuscodes zurückgegeben und über eine Warnung Header übermittelt werden.
author: Preetikr
localization_priority: Normal
ms.openlocfilehash: 16a7153f460b57a74901b0d5c48bdd9004e06bc4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830765"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft Graph Sicherheit API Fehlerantworten

Fehler in der Microsoft Graph Sicherheit API werden mithilfe des standard 206 teilweise von HTTP-Statuscodes zurückgegeben und über eine Warnung Header übermittelt werden.

## <a name="errors"></a>Fehler

Sicherheit-API von Microsoft Graph ist ein Verbundpartner Dienst, der von allen Datenanbieter mehrere Antworten empfängt. Wenn ein HTTP-Fehler durch die Microsoft Graph Sicherheit API empfangen wird, sendet er wieder eine Warnung Kopfzeile im folgenden Format:<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Diese Warnung Kopfzeile ist nur an Clients gesendet, wenn-Datenanbieter einen Fehlercode als 2xx oder 404 zurückgibt. Beispiel:

- HttpStatusCode.Forbidden (403) könnte zurückgegeben werden, wenn der Zugriff auf die Ressource nicht gewährt wird.
- Wenn ein Anbieter ist ein Timeout aufgetreten, wird in der Kopfzeile Warnung HttpStatusCode.GatewayTimeout (504) zurückgegeben.
- Wenn ein für internen Anbieterfehler auftritt, wird HttpStatusCode.InternalServerError (500) in der Kopfzeile Warnung verwendet.

Wenn ein Datenanbieters 2xx oder 404 zurückgibt, wird er nicht in der Kopfzeile Warnung angezeigt, da diese Codes für den Erfolg erwartet werden oder wenn Daten jeweils nicht gefunden werden kann. Eine 404 nicht gefunden wird in einem Verbundpartner System erwartet, wie oft die Daten nur ein oder mehrere, aber nicht alle Anbieter bekannt ist.

## <a name="example"></a>Beispiel

Ein Benutzer fordert `security/alerts/{alert_id}`.

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

Da 404 und 200 erwartete Bedingungen sind, enthält die Warnung Kopfzeile Folgendes:

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Hinweis:** Jede HTTP-Header ist eine Auflistung von Unterelemente, sodass Benutzer die Warnung Kopfzeile auflisten und alle Elemente überprüfen können.

## <a name="constraints"></a>Einschränkungen

Die `$top` OData-Abfragezeichenfolgen-Parameter kann maximal 1000 Warnungen und eine Kombination von `$top`  +  `$skip` OData-Abfrage-Parameter können nicht überschreiten 6000 Warnungen. Beispielsweise `/security/alerts?$top=10&$skip=5990` zurückgegebenen eine `200 OK` Antwortcode, aber `/security/alerts?$top=10&$skip=5991` zurückgegebenen eine `400 Bad Request` Antwortcode.

Eine Umgehung für diese Grenze ist die Verwendung der `$filter` OData-Abfragezeichenfolgen-Parameter mit der `eventDateTime` der Warnung Entität aus der Microsoft Graph-Security-API mit `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` , und ersetzen den DateTime-Wert durch die letzte Benachrichtigung (6000th). Sie können auch festlegen, einen Bereich für die `eventDateTime`; beispielsweise *Alerts?$ Filter = Ereignisdatum/-Uhrzeit **Gt** 2018-11 -**11**T00:00:00.000Z & Ereignisdatum/-Uhrzeit **Lt** 2018-11 -**12**T00:00:00.000Z*

## <a name="see-also"></a>Siehe auch

Wenn Sie Probleme mit Autorisierung haben, finden Sie unter [Authorization and Security-API von Microsoft Graph](/graph/security-authorization).
