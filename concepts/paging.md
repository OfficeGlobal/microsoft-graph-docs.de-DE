
# <a name="paging-microsoft-graph-data-in-your-app"></a>Paging der Microsoft Graph-Daten in Ihrer App 

Einige Abfragen in Microsoft Graph geben mehrere Seiten von Daten zurück, entweder aufgrund von serverseitigem Paging oder aufgrund der Verwendung des `$top`-Abfrageparameters, um die Seitengröße in einer Anforderung gezielt zu begrenzen. Wenn ein Resultset mehrere Seiten umfasst, gibt Microsoft Graph eine `@odata.nextLink`-Eigenschaft in der Antwort, die eine URL zu der nächsten Seite mit Ergebnissen enthält. 

Die folgende URL fordert beispielsweise alle Benutzer in einer Organisation mit einer Seitengröße von 5 an, die mit dem `$top`-Abfrageparameter angegeben wurde.

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

Wenn das Ergebnis mehr als fünf Benutzer enthält, gibt Microsoft Graph eine `odata:nextLink`-Eigenschaft, die der folgenden ähnelt, zusammen mit der ersten Seite von Benutzern zurück.

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

Sie können die nächste Seite der Ergebnisse abrufen, indem Sie den URL-Wert der `@odata:nextLink`-Eigenschaft an Microsoft Graph senden. 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

Microsoft Graph gibt weiterhin einen Verweis auf die nächste Seite von Daten in der `@odata:nextLink`-Eigenschaft mit jeder Antwort zurück, bis alle Seiten des Ergebnisses gelesen wurden.

>**Wichtig:** Sie sollten die gesamte URL in die `@odata:nextLink`-Eigenschaft in Ihrer Anforderung für die nächste Seite der Ergebnisse einschließen. In Abhängigkeit von der API, für die die Abfrage ausgeführt wird, enthält der `@odata:nextLink`-URL-Wert entweder den Abfrageparameter  `$skiptoken` oder `$skip`. Die URL enthält auch alle anderen Abfrageparameter, die in der ursprünglichen Anforderung vorhanden sind. Versuchen Sie nicht, den Wert `$skiptoken` oder `$skip` zu extrahieren und ihn in einer anderen Anforderungen zu verwenden. 

Das Paging-Verhalten variiert in den unterschiedlichen Microsoft Graph-APIs. Sie sollten beim Arbeiten mit ausgelagerten Daten die folgenden Punkte berücksichtigen:

- Unterschiedliche APIs weisen möglicherweise unterschiedliche Standard- und Maximalgrößen für Seiten aufweisen.
- Unterschiedliche APIs verhalten sich möglicherweise unterschiedlich, wenn Sie eine Seitengröße (über den `$top`-Abfrageparameter) angeben, der die maximale Seitengröße für diese API überschreitet. Je nach API wird die angeforderte Seitengröße möglicherweise ignoriert, sie kann standardmäßig die maximale Seitengröße für diese API aufweisen, oder Microsoft Graph gibt einen Fehler zurück.  
- Nicht alle Ressourcen oder Beziehungen unterstützen Paging. Abfragen von [directoryRoles](../api-reference/v1.0/resources/directoryrole.md) unterstützen beispielsweise kein Paging. Dies umfasst das Lesen von Rollenobjekten und Rollenmitgliedern.
- Einige Microsoft Graph-APIs unterstützen Rückwärts-Paging durch Anfügen des `previous-page`-Abfrageparameters (`&previous-page=true`) an den URL-Wert der `@odata:nextLink`-Eigenschaft. Nachdem Sie diesen Parameter an eine Anforderung angefügt haben, ist dieser im `@odata:nextLink`-URL-Wert in nachfolgenden Antworten enthalten. Das Rückwärts-Paging ist weiterhin möglich, bis eine Antwort mit einem leeren Ergebnis zurückgegeben wird. Durch Paging wird weiterhin ein Fehler zurückgegeben. Alternativ können Sie das Vorwärts-Paging von der aktuellen Antwort fortsetzen, indem Sie den `previous-page`-Parameter entfernen, wenn Sie die Anforderung für die nächste Seite von Ergebnissen senden. 

