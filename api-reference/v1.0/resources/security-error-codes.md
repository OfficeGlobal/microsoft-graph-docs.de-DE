# <a name="security-api-error-responses"></a>Sicherheits-API-Fehlerantworten

Fehler in der Sicherheits-API von Microsoft Graph werden mithilfe der Standard-HTTP-Statuscodes zurückgegeben und über einen Warnungsheader übermittelt.

Die Sicherheits-API ist ein Verbunddienst, der von allen Datenanbieter mehrere Antworten empfängt. Wenn ein HTTP-Fehler durch die Sicherheits-API empfangen wird, sendet sie wieder einen Warnungsheader im folgenden Format: <!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Dieser Warnungsheader wird nur an Clients zurückgesendet, wenn einer der Datenanbieter einen anderen Fehlercode als 2xx oder 404 zurückgibt. Beispiel:

- HttpStatusCode.Forbidden (403) könnte zurückgegeben werden, wenn der Zugriff auf die Ressource nicht gewährt wird.
- Wenn ein Anbieter ein Zeitlimit überschreitet, wird im Warnungsheader HttpStatusCode.GatewayTimeout (504) zurückgegeben.
- Wenn ein interner Anbieterfehler auftritt, wird im Warnungsheader HttpStatusCode.InternalServerError (500) verwendet.

Wenn ein Datenanbieter 2xx oder 404 zurückgibt, wird es nicht im Warnungsheader angezeigt, da diese Codes für den Erfolg erwartet werden oder wenn entsprechend Daten nicht gefunden werden. Ein "404 nicht gefunden" wird in einem Verbundsystem so oft erwartet, wie die Daten nur einem oder mehreren, aber nicht allen Anbieter bekannt sind.

## <a name="example"></a>Beispiel

Ein Benutzer fordert `security/alerts/{alert_id}` an.

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

Da 404 und 200 erwartete Bedingungen sind, enthält der Warnungsheader Folgendes: 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/29000",    (usual timeout limit is set at 29 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Hinweis:** Jeder HTTP-Header ist eine Sammlung von Unterelementen, sodass die Benutzer den Warnungsheader aufzählen und alle Elemente überprüfen können.

## <a name="see-also"></a>Siehe auch

Wenn Probleme bei der Autorisierung auftreten, beziehen Sie sich auf unseren [Blogbeitrag](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).
