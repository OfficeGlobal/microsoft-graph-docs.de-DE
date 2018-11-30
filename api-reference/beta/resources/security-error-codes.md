---
title: Microsoft Graph Sicherheit API Fehlerantworten
description: Fehler in der Microsoft Graph Sicherheit API werden mithilfe der standard-HTTP-206 teilweise Content Statuscode zurückgegeben und über eine Warnung Kopfzeile übermittelt werden.
ms.openlocfilehash: a67023a8a21687e357e6b6eff1ffa47f026ccd68
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059944"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Microsoft Graph Sicherheit API Fehlerantworten

Fehler in der Microsoft Graph Sicherheit API werden mithilfe der standard-HTTP-206 teilweise Content Statuscode zurückgegeben und über eine Warnung Kopfzeile übermittelt werden.

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

Ein Benutzer fordert `/alerts/{alert-id}`.

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

## <a name="see-also"></a>Siehe auch

Wenn Sie Probleme mit Autorisierung haben, finden Sie in unserem [Blog veröffentlichen](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).
