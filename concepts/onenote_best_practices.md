# <a name="best-practices-for-working-with-the-onenote-api-in-microsoft-graph"></a>Bewährte Methoden für die Arbeit mit OneNote-APIs in Microsoft Graph.

Dieser Artikel enthält Vorschläge für die Arbeit mit OneNote-APIs in Microsoft Graph. Diese Empfehlungen basieren auf den Antworten auf häufig gestellte Fragen auf Stack Overflow und Twitter.

## <a name="use-select-to-select-the-minimum-set-of-properties-you-need"></a>Verwenden von $select, um die minimale Anzahl der benötigten Eigenschaften auszuwählen

Wenn Sie eine Ressource (z. B. Abschnitte innerhalb eines Notizbuchs) abfragen, verwende Sie eine ähnliche Abfrage wie die folgende.

```http
GET ~/notebooks/{id}/sections
```

Es werden alle Eigenschaften der Abschnitte abgerufen. Allerdings benötigen Sie möglicherweise nicht alle Eigenschaften. Sie können den `$select`-Abfragenparameter verwenden, um nur die gewünschten, Eigenschaften zurückzugeben, wie im folgenden Beispiel gezeigt.

```http
GET ~/notebooks/{id}/sections?$select=id,displayName
```

Der gleiche Ansatz gilt für andere OneNote-APIs.

## <a name="use-expand-instead-of-making-multiple-api-calls"></a>Verwenden von $expand, anstatt mehrere API-Aufrufe auszuführen

Nehmen wir an, dass Sie alle Notizbücher, Abschnitte und Abschnittsgruppen des Benutzers in einer hierarchischen Ansicht abrufen möchten. Dazu können Sie folgendermaßen vorgehen:

* Rufen Sie `GET ~/notebooks` auf, um die Liste der Notizbücher anzuzeigen.

* Rufen Sie für jedes abgerufene Notizbuch `GET ~/notebooks/{notebookId}/sections` auf, um die Liste der Abschnitte anzuzeigen.

* Rufen Sie für jedes abgerufene Notizbuch `GET ~/notebooks/{notebookId}/sectionGroups` auf, um die Liste der Abschnittsgruppen anzuzeigen.

* Optional können Sie die Abschnittsgruppen rekursiv durchlaufen.

Dies ist zwar (mit ein paar zusätzlichen sequenziellen Roundtrips zum Dienst) möglich, besserer wäre es jedoch, den `$expand`-Parameter zu verwenden. 

```http
GET ~/notebooks?$expand=sections,sectionGroups($expand=sections)
```

Dadurch werden dieselben Ergebnisse mit einer besseren Leistung in einer Netzwerkschleife erzielt.

## <a name="when-getting-all-pages-for-a-user-do-so-for-each-section-separately"></a>Wenn Sie alle Seiten eines Benutzer abrufen möchten, müssen Sie dies für jeden Abschnitt separat tun.

Obgleich Microsoft Graph über einen Endpunkt verfügt, um alle Seiten abzurufen, ist dies nicht die beste Möglichkeit, um alle Seiten, auf die der Benutzer Zugriff hat, anzuzeigen. Wenn der Benutzer zu viele Abschnitte besitzt, kann dies zu Timeouts oder Verschlechterung der Leistung führen. Es ist besser, jeden Abschnitt einzeln zu durchlaufen und die Seiten für jeden Abschnitt einzeln abzurufen.

Anstatt diesen Aufruf zu verwenden (diese API ist seitennummeriert, sodass Sie nicht alle Seiten auf einmal abrufenden können):

```http
GET ~/pages
```

Ist es besser, den folgenden Aufruf mehrmals zu verwenden (insbesondere, wenn Sie nicht alle Abschnitte benötigen):

```http
GET ~/sections/{id}/pages
```

Wenn Sie Seitenmetadaten erhalten, überschreiben Sie die standardmäßige `lastModifiedDateTime`-Sortierung. Seiten können schneller abgerufen werden, wenn Sie nicht nach `lastModifiedDateTime` sortiert werden müssen. Zu diesem Zweck können Sie nach einer anderen Eigenschaft sortieren, z. B:

```http
GET ~/sections/{id}/pages?$select=id,title,createdDateTime&$orderby=createdDateTime
```
