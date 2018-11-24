# <a name="activity-resource-type"></a>Ressourcentyp Aktivität

Stellt eine einzelne Aktivität in einer app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel. Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als [Historienelement](projectrome_historyitem.md) erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.

Sie können Aktivitäten in Microsoft Graph, damit Benutzer zurückerhalten, was sie für mehrere Geräte in ihrer app getan haben. Aktivitäten, die Ihre app erstellt auf Geräten alle Benutzer angezeigt werden, und für Benutzer als deep-Links auf bestimmte Inhalte Ihrer App verfügbar gemacht. Sie können bestimmte Inhalte Ihrer App als Ziel Ausdrücken, die in Windows und den Zugriff auf iOS und Android-Geräte über Cortana Benachrichtigungen präsentiert wird.

Da jeder app anders ist, ist es Ihnen zu verstehen, die beste Möglichkeit zum Zuordnen von Aktionen innerhalb der Anwendung auf die Benutzeraktivitäten, die in Cortana und Zeitachse angezeigt wird. Beispielsweise Spiele möglicherweise eine Aktivität für jede Kampagne erstellen, Erstellen von apps Dokument möglicherweise eine Aktivität für jedes Dokument erstellen und Line-of-Business-apps möglicherweise eine Aktivität für jeden Workflow erstellen.

Ihre Benutzeraktivitäten werden in Cortana und Windows-Zeitachsen Benutzererlebnis präsentiert werden die konzentriert sich eine Erhöhung Benutzer Produktivität und Effizienz durch Unterstützung bei der ähnliche Inhalte zu erhalten, die sie in der Vergangenheit gearbeitet.

## <a name="methods"></a>Methoden

|Methode | Rückgabetyp | Beschreibung|
|:------|:------------|:-----------|
|[Erstellen oder Ersetzen Sie die Aktivität](../api/projectrome_put_activity.md) | [Aktivität](projectrome_activity.md) |Erstellt oder eine vorhandene Aktivität (Upsert) ersetzt. Die AppActivityId URL-sichere (alle Zeichen mit Ausnahme der RFC 2396 nicht reservierte Zeichen in ihre hexadezimale Darstellung konvertiert werden müssen) sein muss, aber die ursprünglichen AppActivityId benötigt keinen URL-sicheren. |
|[Aktivität löschen](../api/projectrome_delete_activity.md) | Kein Inhalt | Löscht die angegebene Aktivität für diesen Benutzer von Ihrer app aus.|
|[Abrufen von Aktivitäten](../api/projectrome_get_activities.md) | Auflistung von [Aktivitäten](projectrome_activity.md) | Ruft die Aktivitäten für Ihre app für einen bestimmten Benutzer ab.|
|[Aktuelle Aktivitäten abrufen](../api/projectrome_get_recent_activities.md) | Auflistung von [Aktivitäten](projectrome_activity.md) | Ruft die neuesten Aktivitäten für Ihre app für einen bestimmten Benutzer, sortiert und basierend auf der am häufigsten zuletzt erstellte oder aktualisierte [HistoryItems](projectrome_historyitem.md)ab.|

## <a name="properties"></a>Eigenschaften

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|userTimezone | Zeichenfolge | Optional. Die Zeitzone, in der das Gerät des Benutzers verwendet, um die Aktivität generieren zum Zeitpunkt der Erstellung Aktivität gefunden wurde; Werte, die zur Unterstützung der plattformübergreifende Darstellung als Olson-IDs angegeben.|
|createdDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, wenn das Objekt auf dem Server erstellt wurde. |
|lastModifiedDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, wenn das Objekt auf dem Server geändert wurde. |
|id | Zeichenfolge | Server generierte ID für die URL-Adressen verwendet.|
|appActivityId | Zeichenfolge | Erforderlich. Die eindeutige Aktivitäts-ID im Kontext der app - vom Anrufer und unveränderlich danach bereitgestellt.|
|activitySourceHost | Zeichenfolge | Erforderlich. URL für die Domäne, die die Zuordnung plattformübergreifende Identität für die app darstellt. Zuordnung ist gespeicherte entweder als JSON-Datei für die Domäne gehostet oder über Windows-Entwicklungscenter konfigurierbar. Die Datei JSON heißt Cross-Plattform-app-IDs und befindet sich am Stamm der Domäne HTTPS, entweder auf die Domäne der obersten Ebene oder enthalten eine Sub-Domäne. Zum Beispiel: https://contoso.com oder https://myapp.contoso.com, jedoch NICHT https://myapp.contoso.com/somepath. Sie müssen einen eindeutigen Dateinamen und Domäne (oder Sub Domäne) pro plattformübergreifende app-Identität verfügen. Beispielsweise ist eine separate Datei und eine Domäne für Word und PowerPoint erforderlich.|
|appDisplayName | Zeichenfolge | Optional. Kurze Beschreibung der app verwendet, um die Aktivität für die Verwendung in Fällen generiert werden, wenn die app nicht auf das lokale Gerät des Benutzers installiert ist.|
|activationUrl | Zeichenfolge | Erforderlich. So starten Sie die Aktivität im systemeigenen optimal dargestellt durch die AppId verwendete URL. Starten eine webbasierten app möglicherweise, wenn keine systemeigene Anwendung vorhanden ist.|
|fallbackUrl | Zeichenfolge | Optional. URL zum Starten der Aktivitätsfeeds in einer webbasierten-app verwendet werden, falls verfügbar.|
|contentUrl | Zeichenfolge | Optional. Verwendet den Fall, dass der Inhalt außerhalb einer systemeigenen oder webbasierte app-Benutzeroberfläche (beispielsweise einen Zeiger auf ein Element in einem RSS-Feed) gerendert werden kann.|
|visualElements| [visualInfo](../resources/projectrome_visualinfo.md) | Erforderlich. Das Objekt mit Informationen zum Rendern der Aktivitätsfeeds in die UX.|
|ContentInfo dar | Nicht typisierte JSON-Objekt | Optional. Eine benutzerdefinierte Datenelement - JSON-LD extensible Beschreibung des Inhalts entsprechend [schema.org](https://schema.org) Syntax.|
|expirationDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, wenn das Objekt auf dem Server abgelaufen.|
|status | status | Vom Server festgelegt. Einen Statuscode verwendet, um gültige Objekte identifizieren. Werte: aktiv, aktualisiert, gelöscht, ignoriert.|

## <a name="relationships"></a>Beziehungen

|Beziehung | Typ | Beschreibung|
|:------------|:-----|:-----------|
|historyItems| [ActivityHistoryItem](../resources/projectrome_historyitem.md) -Auflistung | Optional. NavigationProperty/Kapselung; Navigationseigenschaft der Aktivität HistoryItems.|

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
