# <a name="activity-resource-type"></a>Ressourcentyp Aktivität

Stellt eine einzelne Aktivität in einer App dar -  beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel. Wenn ein Benutzer diese Aktivität einbezieht, wird das Engagement als [Element des Ereignisprotokolls](projectrome_historyitem.md) erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wenn der Benutzer diese Aktivität im Laufe er Zeit erneut einbezieht, werden mehrere Elemente des Ereignisprotokolls als eine einzelne Benutzeraktivität aufgezeichnet.

Sie können Aktivitäten in Microsoft Graph verwenden, um Benutzern zu ermöglichen, auf mehreren Geräten zu dem zurückzukehren, was sie in ihrer App getan haben. Aktivitäten, die von Ihrer App erstellt werden, erscheinen auf allen Geräten der Nutzer und werden Nutzern als Deep Links zu bestimmten Inhalten in Ihrer App angezeigt. Sie können bestimmte Inhalte in Ihrer App als Ziel darstellen, das in Windows angezeigt wird und auf iOS- und Android-Geräten über Cortana-Benachrichtigungen zugänglich ist.

Da jede App anders ist, müssen Sie wissen, wie Sie Aktionen in Ihrer Anwendung am besten auf Benutzeraktivitäten abbilden, die in Cortana und Timeline angezeigt werden. Beispielsweise können Spiele für jede Kampagne eine Aktivität erstellen, während die Erstellung von Dokumenten-Apps möglicherweise eine Aktivität für jedes einzigartige Dokument erstellen, und Branchen-Apps können für jeden Workflow eine Aktivität erstellen.

Ihre Benutzeraktivitäten werden in den Benutzererfahrungen von Cortana und der Windows-Zeitachse angezeigt, die darauf ausgerichtet sind, die Produktivität und Effizienz der Benutzer zu erhöhen, indem sie ihnen helfen, zu Inhalten zurückzukehren, an denen sie in der Vergangenheit gearbeitet haben.

## <a name="methods"></a>Methoden

|Methode | Rückgabetyp | Beschreibung|
|:------|:------------|:-----------|
|[Aktivität erstellen oder ersetzen](../api/projectrome_put_activity.md) | [activity](projectrome_activity.md) |Erstellt oder ersetzt eine vorhandene Aktivität (Upsert). Die appActivityId muss URL-sicher sein (alle Zeichen außer RFC 2396 nicht reservierten Zeichen müssen in ihre hexadezimale Darstellung konvertiert werden), aber die ursprüngliche appActivityId muss nicht URL-sicher sein. |
|[Eine Aktivität löschen](../api/projectrome_delete_activity.md) | Kein Inhalt | Löscht die angegebene Aktivität für diesen Benutzer von Ihrer App aus.|
|[Aktivitäten abrufen](../api/projectrome_get_activities.md) | Sammlung von [Aktivitäten](projectrome_activity.md) | Ruft die Aktivitäten für Ihre App für einen bestimmten Benutzer ab.|
|[Aktuelle Aktivitäten abrufen](../api/projectrome_get_recent_activities.md) | Sammlung von [Aktivitäten](projectrome_activity.md) | Ruft die aktuellste Aktivitäten für Ihre App für einen bestimmten Benutzer ab, sortiert und basierend auf der am häufigsten zuletzt erstellten oder aktualisierten [HistoryItems](projectrome_historyitem.md).|

## <a name="properties"></a>Eigenschaften

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|userTimezone | Zeichenfolge | Optional. Die Zeitzone, in der das Gerät des Benutzers zum Generieren der Aktivität verwendet wurde, in der es sich zum Zeitpunkt der Erstellung der Aktivität befand. Werte, die als Olson-IDs bereitgestellt werden, um die plattformübergreifende Darstellung zu unterstützen.|
|createdDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, als das Objekt auf dem Server erstellt wurde. |
|lastModifiedDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, als das Objekt auf dem Server geändert wurde. |
|ID | Zeichenfolge | Vom Server generierte ID, verwendet für die URL-Adressierung.|
|appActivityId | Zeichenfolge | Erforderlich. Die eindeutige Aktivitäts-ID im Kontext der App - vom Anrufer geliefert und unveränderlich danach bereitgestellt.|
|activitySourceHost | Zeichenfolge | Erforderlich. URL für die Domäne, die die plattformübergreifende Identitätszuordnung für die App darstellt. Die Zuordnung wird entweder als JSON-Datei in der Domäne gespeichert oder kann über das Windows-Entwicklungscenter konfiguriert werden. Die JSON-Datei heißt plattformübergreifende App-IDs und wird im Stammverzeichnis Ihrer HTTPS-Domäne entweder in der Top-Level-Domäne gehostet oder enthält eine Sub-Domäne. Zum Beispiel: https://contoso.com oder https://myapp.contoso.com, jedoch NICHT https://myapp.contoso.com/somepath. Sie benötigen eine eindeutige Datei und Domäne (oder Sub-Domäne) pro plattformübergreifende App-Identität. Beispielsweise ist eine separate Datei und eine Domäne für Word und PowerPoint erforderlich.|
|AppDisplayName | Zeichenfolge | Optional. Kurze Beschreibung der App, die zum Generieren der Aktivität verwendet wird, wenn die App nicht auf dem lokalen Gerät des Benutzers installiert ist.|
|activationUrl | Zeichenfolge | Erforderlich. URL, die zum Starten der Aktivität in der von der App-Id dargestellten besten systemeigenen Erfahrung verwendet wird. Startet möglicherweise eine webbasierte App, wenn keine systemeigene App vorhanden ist.|
|fallbackUrl | Zeichenfolge | Optional. URL, die zum Starten der Aktivität in einer webbasierten App verwendet wird, falls verfügbar.|
|contentUrl | Zeichenfolge | Optional. Wird verwendet, wenn der Inhalt außerhalb einer nativen oder webbasierten App-Erfahrung gerendert werden kann (z.B. ein Zeiger auf ein Element in einem RSS-Feed).|
|visualElements| [visualInfo](../resources/projectrome_visualinfo.md) | Erforderlich. Das Objekt mit Informationen zum Rendern der Aktivität in der UX.|
|contentInfo | Nicht typisiertes JSON-Objekt | Optional. Ein benutzerdefiniertes Datenelement - JSON-LD erweiterbare Beschreibung des Inhalts entsprechend der [schema.org](http://schema.org) Syntax.|
|expirationDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, wenn das Objekt auf dem Server abgelaufen ist.|
|Status | status | Vom Server festgelegt. Ein Statuscode, der dazu verwendet wird, um gültige Objekte identifizieren. Werte: aktiv, aktualisiert, gelöscht, ignoriert.|

## <a name="relationships"></a>Beziehungen

|Beziehung | Typ | Beschreibung|
|:------------|:-----|:-----------|
|historyItems| [ActivityHistoryItem](../resources/projectrome_historyitem.md) -Sammlung | Optional. NavigationProperty / Eindämmung; Navigationseigenschaft zu den historyItems der Aktivität.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "appDisplayName",
    "fallbackUrl",
    "contentUrl",
    "contentInfo",
    "visualElements",
    "historyItems"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.userActivity",
  "@odata.annotations": [
    {
      "capabilities": {
        "countable": false,
        "selectable": false,
        "skippable": false
      }
    }
  ]
}-->

```json
{
    "appActivityId": "String",
    "activitySourceHost": "String (host name/domain/URL)",
    "userTimezone": "String",
    "appDisplayName": "String",
    "activationUrl": "String (URL)",
    "contentUrl": "String (URL)",
    "fallbackUrl": "String (URL)",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "expirationDateTime": "DateTimeOffset",
    "id": "String",
    "status": "active | updated | deleted | ignored",
    "contentInfo": { "@odata.type": "microsoft.graph.Json" },
    "visualElements": { "@odata.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.activityHistoryItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
