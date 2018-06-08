# <a name="best-practices-for-working-with-microsoft-graph"></a>Optimale Methoden für das Arbeiten mit Microsoft Graph

In diesem Artikel werden bewährte Methoden beschrieben, die Sie anwenden können, damit Ihre Anwendungen Microsoft Graph optimal nutzen, ganz gleich, ob es dabei um mehr Informationen zu Microsoft Graph, das Verbessern der App-Leistung oder darum geht, die Anwendung für Endbenutzer zuverlässiger zu gestalten.

## <a name="use-graph-explorer-to-get-to-know-the-api"></a>Verwenden von Graph-Explorer, um die API kennenzulernen

Der einfachste Weg, um die über Microsoft Graph verfügbaren Daten zu erkunden, besteht darin, [Graph-Explorer](https://aka.ms/ge) zu verwenden. Mit Graph-Explorer können Sie REST-Abfragen (mit voller CRUD-Unterstützung) erstellen, die HTTP-Anforderungsheader anpassen und die Datenantworten anzeigen. Um Ihnen den Einstieg zu erleichtern, stellt Graph-Explorer auch eine Reihe von Beispielabfragen bereit.

Experimentieren Sie mit neuen APIs, bevor Sie sie in Ihre Anwendung integrieren.

## <a name="authentication"></a>Authentifizierung

Um auf die Daten in Microsoft Graph zuzugreifen, muss Ihre Anwendung ein OAuth 2.0-Zugriffstoken abrufen und dieses Microsoft Graph in einem der folgenden Elemente präsentieren:

- Dem HTTP-Anforderungsheader für die *Autorisierung*, als *Bearer*token
- Dem Graph-Clientkonstruktor, wenn Sie eine Microsoft Graph-Clientbibliothek verwenden

Verwenden Sie die API der Microsoft-Authentifizierungsbibliothek, [MSAL](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-v2-libraries), um das Zugriffstoken für Microsoft Graph zu erhalten.

## <a name="consent-and-authorization"></a>Zustimmung und Autorisierung

Wenden Sie die folgenden bewährten Methoden für Zustimmung und Autorisierung in Ihrer App an:

- **Verwenden Sie die niedrigsten Berechtigungen**. Fordern Sie nur Berechtigungen an, die unbedingt notwendig sind, und nur dann, wenn Sie sie benötigen. Für die APIs in Ihren Anwendungsaufrufen überprüfen Sie den Berechtigungsabschnitt im Thema mit den Methoden (sehen Sie sich beispielsweise [Erstellen eines Benutzers](../api-reference/v1.0/api/user_post_users.md) an, und wählen Sie die Berechtigungen mit den geringsten Rechten aus). Eine vollständige Liste von Berechtigungen finden Sie unter [Berechtigungsreferenz](permissions_reference.md).

- **Verwenden Sie den entsprechenden Berechtigungstyp basierend auf Szenarien**. Wenn Sie eine interaktive Anwendung erstellen, bei der es einen angemeldeten Benutzer gibt, sollte die Anwendung *delegierte* Berechtigungen verwenden, sodass der Anwendung die Berechtigung delegiert wird, bei Aufrufen von Microsoft Graph als angemeldeter Benutzer zu fungieren. Wenn Ihre Anwendung jedoch ohne angemeldeten Benutzer ausgeführt wird, z. B. als Hintergrunddienst oder Daemon, sollte die Anwendung Anwendungsberechtigungen verwenden.

    >**Hinweis:** Die Verwendung von Anwendungsberechtigungen für interaktive Szenarien kann für Ihre Anwendung ein Compliance- und Sicherheitsrisiko darstellen. Die Berechtigungen eines Benutzers könnten versehentlich erhöht werden, sodass dieser auf Daten zugreifen kann, wodurch die von einem Administrator konfigurierten Richtlinien umgangen werden.
<!-- LG: Use a more clear lead-in here, like "Consider the end user and admin experience"? -->
- **Gehen Sie beim Konfigurieren Ihr App mit Bedacht vor**. Dies wirkt sich direkt auf die Erfahrung von Endbenutzern und Administratoren sowie auf die Akzeptanz und die Sicherheit der Anwendung aus. Beispiel:

    - Die Datenschutzrichtlinie Ihrer Anwendung, die Nutzungsbedingungen, der Name, das Logo und die Domäne werden in Zustimmungs- und anderen Oberflächen angezeigt. Stellen Sie daher sicher, dass sie diese sorgfältig konfigurieren, damit bei Ihren Endbenutzern keine Missverständnisse entstehen.
    - Überlegen Sie sich, wer Ihrer Anwendung zustimmen soll: Endbenutzer oder Administratoren. Konfigurieren Sie die Anwendung dann so, dass [Berechtigungen entsprechend angefordert werden](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-v2-scopes).
    - Sie müssen den Unterschied zwischen [statischer, dynamische und inkrementeller Zustimmung](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-v2-compare#incremental-and-dynamic-consent) verstehen.

- **Erwägen Sie Anwendungen mit mehreren Mandanten**. Gehen Sie davon aus, dass Kunden verschiedene Anwendungs- und Zustimmungssteuerungen in unterschiedlichen Zuständen haben. Beispiel:

    - Mandantenadministratoren können die Möglichkeit für Endbenutzer zum Zustimmen von Anwendungen deaktivieren. In diesem Fall müsste ein Administrator im Namen seiner Benutzer zustimmen.
    - Mandantenadministratoren können benutzerdefinierte Autorisierungsrichtlinien festlegen, z. B., dass Benutzer nicht die Profile anderer Benutzer lesen können, oder das Beschränken der Self-Service-Gruppenerstellung auf eine eingeschränkte Gruppe von Benutzern. In diesem Fall sollte Ihre Anwendung die Fehlerantwort 403 verarbeiten können, wenn sie im Auftrag eines Benutzers handelt.

## <a name="handle-responses-effectively"></a>Effizientes Verarbeiten von Anworten

In Abhängigkeit von den Anforderungen, die an Microsoft Graph gestellt werden, sollten Ihre Anwendungen in der Lage sein, verschiedene Antworttypen zu verarbeiten. Nachfolgend finden Sie einige der wichtigsten Methoden, um sicherzustellen, dass Ihre Anwendung für die Endbenutzer zuverlässig und vorhersehbar reagiert.

### <a name="pagination"></a>Paginierung

Beim Abfragen einer Ressourcensammlung sollten Sie davon ausgehen, dass Microsoft Graph das Resultset aufgrund von serverseitigen Beschränkungen der Seitengröße auf mehreren Seiten zurückgibt. Wenn sich ein Resultset über mehrere Seiten erstreckt, gibt Microsoft Graph eine `@odata.nextLink`-Eigenschaft in der Antwort zurück, die eine URL zu der nächsten Seite mit Ergebnissen enthält.

Eine Auflistung der Nachrichten angemeldeter Benutzer:

```http
GET https://graph.microsoft.com/v1.0/me/messages
```

Würde eine Antwort mit einer `@odata.nextLink`-Eigenschaft zurückgeben, wenn das Resultset die serverseitige Beschränkung der Seitengröße überschreitet.

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$skip=23"
```

>**Hinweis:** Ihre Anwendung sollte **immer** die Möglichkeit verarbeiten, dass die Antworten paginiert sind, und die `@odata.nextLink`-Eigenschaft verwenden, um die nächste paginierte Reihe von Ergebnissen zu erhalten, bis alle Seiten des Resultsets gelesen wurden. Die letzte Seite enthält keine `@odata.nextLink`-Eigenschaft. Sie sollten die gesamte URL in die `@odata:nextLink`-Eigenschaft in Ihrer Anforderung für die nächste Seite mit Ergebnissen einschließen, wobei die gesamte URL als opake Zeichenfolge behandelt wird.

Weitere Informationen finden Sie unter [Paginierung](paging.md).

### <a name="handling-expected-errors"></a>Behandlung erwarteter Fehler

Ihre Anwendung sollte zwar alle Fehlerantworten (in den Bereichen 400 und 500) behandeln, besonderes Augenmerk liegt jedoch auf bestimmten erwarteten Fehlern und Antworten, die in der folgenden Tabelle aufgeführt sind.

| Thema   | HTTP-Fehlercode    | Bewährte Methode|
|:-----------|:--------|:----------|
| Benutzer hat keinen Zugriff | 403 | Wenn Ihre Anwendung läuft, könnte dieser Fehler auch dann auftreten, wenn diese die erforderlichen Berechtigungen über eine Zustimmungsoberfläche erhalten hat.  In diesem Fall ist es sehr wahrscheinlich, dass der angemeldete Benutzer nicht über Berechtigungen zum Zugreifen auf die angeforderte Ressource verfügt. Ihre Anwendung sollte den generischen Fehler „Zugriff verweigert“ für den angemeldeten Benutzer ausgeben. |
|Nicht gefunden (Not Found)| 404 | In bestimmten Fällen wird die angeforderte Ressource möglicherweise nicht gefunden. Vielleicht ist eine Ressource nicht vorhanden, weil sie noch nicht bereitgestellt wurde (z. B. das Foto eines Benutzers) oder weil sie gelöscht wurde. Einige gelöschte Ressourcen *können* innerhalb von 30 Tagen nach dem Löschen vollständig wiederhergestellt werden – z. B. Benutzer, Gruppen und Anwendungsressourcen, Ihre Anwendung sollte dies daher auch berücksichtigen.|
|Drosselung|429|APIs können aus unterschiedlichen Gründen jederzeit eine Drosselung vornehmen, Ihre Anwendung muss daher **immer** in der Lage sein, 429-Antworten zu behandeln. Im HTTP-Antwortheader der Fehlerantwort ist das Feld *Retry-After* enthalten. Das Zurückziehen von Anforderungen mithilfe der Verzögerung *Retry-After* ist die schnellste Möglichkeit zur Wiederherstellung nach einer Drosselung. Weitere Informationen finden Sie unter [Drosselung](throttling.md).|
|Dienst nicht verfügbar (Service Unavailable)| 503 | Dieser Fehler tritt wahrscheinlich auf, weil der Dienst ausgelastet ist. In diesem Fall sollten Sie die Strategie des Zurückziehens ähnlich wie bei Fehler 429 anwenden. Außerdem sollten Sie **immer** neue Wiederholanforderungen über eine neue HTTP-Verbindung ausführen.|

### <a name="evolvable-enums"></a>Entwickelbare Enumerationen

Clientanwendungen können durch das Hinzufügen von Membern zu einer vorhandenen Enumeration beschädigt werden. Für einige neuere Enumerationen in Microsoft Graph gibt es einen Mechanismus, der das Hinzufügen neuer Member ermöglicht, ohne das hierfür eine wesentliche Änderung erforderlich ist. In diesen neueren Enumerationen werden Sie ein *sentinel*-Element namens `unknownFutureValue` bemerken, das bekannte und unbekannte Enumerationsmember abgrenzt. Bekannte Member weisen eine niedrigeren Wert als das Sentinel-Member auf, unbekannte Member hingegen einen größeren Wert.
Unbekannte Member werden standardmäßig nicht von Microsoft Graph zurückgegeben. Wenn Ihre Anwendung jedoch so geschrieben wurde, dass das Vorkommen unbekannter Member verarbeitet wird, können unbekannte Enumerationsmember mithilfe des HTTP-Anforderungsheaders *Prefer* empfangen werden.

>**Hinweis:** Wenn Ihre Anwendung in der Lage ist, unbekannte Enumerationsmember zu verarbeiten, sollte das Abonnieren über den HTTP-Anforderungsheader *prefer* erfolgen: `Prefer: include-unknown-enum-members`.

## <a name="storing-data-locally"></a>Lokales Speichern von Daten

Im Idealfall sollte Ihre Anwendung Aufrufe von Microsoft Graph zum Abrufen von Daten in Echtzeit tätigen, wenn erforderlich. Daten sollten nur dann zwischengespeichert oder lokal gespeichert werden, wenn dies für ein bestimmtes Szenario erforderlich ist und wenn dieser Anwendungsfall von Ihren Nutzungsbedingungen und Ihrer Datenschutzbestimmung abgedeckt ist und nicht gegen die [Nutzungsbedingungen Microsoft Graph](../misc/terms-of-use.md) verstößt. Ihre Anwendung sollte auch entsprechende Aufbewahrungs- und Löschrichtlinien implementieren.

## <a name="optimizations"></a>Optimierungen

Im Allgemeinen sollten Sie aus Leistungs-, Sicherheits- und Datenschutzgründen nur die Daten abrufen, die Ihre Anwendung wirklich benötigt und nicht mehr.

### <a name="use-projections"></a>Verwenden von Prognosen

Wählen Sie nur die Eigenschaften aus, die Ihre Anwendung wirklich benötigt, da dadurch unnötiger Netzwerkverkehr und unnötige Datenverarbeitungen in Ihrer Anwendung (und im Dienst) verhindert werden.

>**Hinweis:** Verwenden Sie den `$select`-Abfrageparameter, um die von einer Abfrage zurückgegebenen Eigenschaften auf diejenigen zu beschränken, die von Ihrer App benötigt werden.

Wenn Sie z. B. die Nachrichten des angemeldeten Benutzers abrufen, können Sie angeben, dass nur die Eigenschaften **from** und **subject** zurückgegeben werden:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

### <a name="getting-minimal-responses"></a>Abrufen minimaler Antworten

Für einige Vorgänge, z. B. PUT und PATCH (und in einigen Fällen POST), können Sie die API auffordern, minimale Daten zurückzugeben, wenn die Anwendung keine Antwortnutzlast nutzen muss. Beachten Sie, dass einige Dienste bereits die Antwort 204 „Kein Inhalt“ für PUT- und PATCH-Vorgänge zurückgeben.

>**Hinweis:** Fordern Sie ggf. minimale Darstellungsantworten mithilfe eines HTTP-Anforderungsheaders an: *Prefer: return=minimal*. Beachten Sie, dass dies für Erstellungsvorgänge möglicherweise nicht geeignet ist, da Ihre Anwendung vielleicht erwartet, dass der Dienst `id` für das neu erstellte Objekt in der Antwort generiert wird.

### <a name="track-changes-delta-query-and-webhook-notifications"></a>Nachverfolgen von Änderungen: Delta-Abfrage und Webhook-Benachrichtigungen

Wenn Ihre Anwendung über Änderungen an Daten informiert sein muss, können Sie eine Webhook-Benachrichtigung erhalten, wenn sich Daten geändert haben. Dies ist effizienter als das bloße Abfragen in regelmäßigen Abständen.

Verwenden Sie [Webhook-Benachrichtigungen](../api-reference/v1.0/resources/webhooks.md), um Pushbenachrichtigungen zu erhalten, wenn sich Daten geändert werden.

Wenn Ihre Anwendung Microsoft Graph-Daten lokal zwischenspeichern oder speichern, diese Daten auf dem neuesten Stand halten oder aus anderen Gründen Änderungen an Daten verfolgen muss, sollten Sie eine Delta-Abfrage verwenden. Dadurch werden übermäßige Berechnungen von Ihrer Anwendung zum Abrufen von Daten verhindert, über die die Anwendung bereits verfügt, der Netzwerkdatenverkehr minimiert und die Wahrscheinlichkeit reduziert, dass ein Drosselungsschwellenwert erreicht wird.

Verwenden Sie eine [Delta-Abfrage](delta_query_overview.md), um Daten effizient auf dem neuesten Stand zu halten.

### <a name="using-webhooks-and-delta-query-together"></a>Gemeinsames Verwenden von Webhooks und Delta-Abfragen

Webhooks und Delta-Abfragen werden häufig in Kombination besser verwendet, denn wenn Sie eine Delta-Abfrage alleine verwenden, müssen Sie das richtige Abfrageintervall ermitteln: wenn dieses zu kurz ist, kommt es zu leeren Antworten, wodurch Ressourcen verschwendet werden, wenn es zu lang ist, führt dies zu veralteten Daten. Wenn Sie Webhook-Benachrichtigungen als Auslöser für Aufrufe von Delta-Abfragen verwenden, können Sie die Vorteile von beiden Ansätzen nutzen.

Verwenden Sie [Webhook-Benachrichtigungen](../api-reference/v1.0/resources/webhooks.md) als Auslöser für Aufrufe von Delta-Abfragen. Sie sollten auch sicherstellen, dass Ihre Anwendung einen Abfrageschwellenwert aufweist, für den Fall, dass keine Benachrichtigungen ausgelöst werden.

### <a name="batching"></a>Batchverarbeitung

Die JSON-Batchverarbeitung ermöglicht es Ihnen, Ihre Anwendung durch Kombinieren von mehreren Anforderungen in einem einzigen JSON-Objekt zu optimieren. Indem Sie die einzelnen Anforderungen in einer einzigen Batchanforderung kombinieren, können Sie die Netzwerklatenz der Anwendung erheblich reduzieren und Verbindungsressourcen einsparen.

Verwenden Sie die [Batchverarbeitung](json_batching.md), wenn eine erhebliche Netzwerklatenz wesentliche Auswirkungen auf die Leistung haben kann.

## <a name="reliability-and-support"></a>Zuverlässigkeit und Support
So stellen Sie sicher, dass Zuverlässigkeit und Support für Ihre Anwendung gewährleistet sind:

- Berücksichtigen Sie die DNS-TTL, und legen Sie die Verbindungs-TTL entsprechend fest. Dadurch wird die Verfügbarkeit im Falle eines Failovers sichergestellt.
- Öffnen Sie Verbindungen für alle angekündigten DNS-Antworten.
- Protokollieren Sie immer die *request-id* und den *timestamp* aus dem HTTP-Antwortheader. Dies ist erforderlich, wenn Fehler oder Berichterstellungsprobleme in Stack Overflow oder an den Microsoft-Kundensuport eskaliert werden.
