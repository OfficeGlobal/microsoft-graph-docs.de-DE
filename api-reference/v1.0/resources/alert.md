# <a name="alert-resource-type"></a>Meldung Ressourcentyp

Stellt potenzielle Sicherheitsrisiken im Mandanten des Kunden dar, die von Microsoft oder Partner-Sicherheitslösungen festgestellt wurden. Verwenden Sie Meldungen, um die Bbehandlung von Sicherheitsproblemen über alle integrierten Lösungen zu vereinheitlichen und zu optimieren. Weitere Informationen erhalten Sie unter den Beispielabfragen im [Graph-Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer).

Meldungen, die von folgendem Anbieter abgerufen werden können: Azure Security Center und Azure Active Directory-Identitäts-Schutz. Zusätzliche Anbieter von Meldungen kommen in den folgenden Monaten hinzu.

## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[Meldung abrufen](../api/alert_get.md) | [Meldung](alert.md) |Lesen der Eigenschaften und Beziehungen eines Warnungs-Objekts.|
|[Meldung aktualisieren](../api/alert_update.md) | [Meldung](alert.md) |Ein Meldungs-Objekt aktualisieren. |
|[Liste der Meldungen](../api/alert_list.md) | [Meldungs](alert.md)-Sammlung |Abruf einer Objekt-Sammlung.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|activityGroupName|Zeichenfolge|Name oder Alias der Aktivitätsgruppe (Angreifer), der diese Meldung zugeordnet ist.|
|assignedTo|Zeichenfolge|Name des Analysten, dem die Meldung zur Triage, Untersuchung oder Wartung zugewiesen ist (Unterstützt [Aktualisierung](../api/alert_update.md)).|
|azureSubscriptionId|Zeichenfolge|Die Azure-Abonnement-ID ist vorhanden, wenn diese Meldung mit einer Azure Ressource verknüpft ist.|
|AzureTenantId *|Zeichenfolge|Azure Active Directory-Mandanten-ID|
|Kategorie|Zeichenfolge|Die Kategorie der Meldung (z. B. CredentialTheft, Ransomware usw.).|
|closedDateTime|DateTimeOffset|Zeitpunkt, zu dem die Benachrichtigung geschlossen wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise könnte Ihre UTC aam 1. Jan 2014 wie folgt aussehen: `'2014-01-01T00:00:00Z'` (Unterstützt [Aktualisieren](../api/alert_update.md)).|
|cloudAppStates|[CloudAppSecurityState](cloudappsecuritystate.md) -Sammlung|Sicherheitsbezogene zustandsorientierte Informationen, die vom Anbieter über die Cloud-Anwendung(en) in Bezug auf diese Warung generiert werden.|
|Kommentare|Zeichenfolgen-Sammlung|Vom Kunden bereitgestellte Kommentare zu Meldungen (für die Meldungs-Verwaltung von Kunden) (Unterstützt [Aktualisierung](../api/alert_update.md)).|
|Konfidenz|Int32|Konfidenz der Erkennungslogik (zwischen 1 und 100 Prozent).|
|createdDateTime|DateTimeOffset|Zeitpunkt, zu dem die Meldung vom Meldungs-Anbieter erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|Beschreibung|Zeichenfolge|Beschreibung der Meldung.|
|detectionIds|Zeichenfolgen-Sammlung|Satz von Meldungen im Zusammenhang mit dieser Melde-Entität (jede Meldung wird als separate Aufzeichnung zum SIEM verschoben).|
|eventDateTime *|DateTimeOffset|Zeitpunkt, zu dem die Ereignisse auftraten, die als Auslöser für die aufgetretene Meldung dienten. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|Feedback|alertFeedback|Analysten-Feedback zur Meldung. Mögliche Werte: `unknown`, `truePositive`, `falsePositive`, `benignPositive`. ( [Unterstützt](../api/alert_update.md)Aktualisierung)|
|fileStates|[FileSecurityState](filesecuritystate.md) -Sammlung|Sicherheitsbezogene Zustandsinformationen, die vom Anbieter über die Dateien im Zusammenhang mit dieser Meldung generiert werden.|
|hostStates|[HostSecurityState](hostsecuritystate.md) -Sammlung|Sicherheitsbezogene Zustandsinformationen, die vom Anbieter über die Hosts im Zusammenhang mit dieser Meldung generiert werden.|
|ID *|Zeichenfolge|Vom Anbieter generierte GUID/eindeutige Bezeichner. (Schreibgeschützt)|
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt, zun dem die Meldungs-Entität zuletzt geändert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|malwareStates|[MalwareState](malwarestate.md) -Sammlung|Malware im Zusammenhang mit dieser Meldung zur Bedrohungsnachricht.|
|networkConnections|[NetworkConnection](networkconnection.md) -Sammlung|Sicherheitsbezogene Zustandsinformationen, die vom Anbieter über die Netzwerkverbindung(en) im Zusammenhang mit dieser Meldung generiert werden.|
|Prozesse|[Prozess](process.md) -Sammlung|Sicherheitsbezogene Zustandsinformationen, die vom Anbieter zum Prozess oder Prozessen im Zusammenhang mit dieser Meldung generiert werden.|
|recommendedActions|Zeichenfolgen-Sammlung|Vom Hersteller/Anbieter empfohlene Aktion(en), die aufgrund der Meldung durchgeführt werden müssen (zum Beispiel Isolieren der Maschine, enforce2FA, Neue Abbildung Host).|
|registryKeyStates|[RegistryKeyState](registrykeystate.md) -Sammlung|Sicherheitsbezogene Zustandsinformationen, die vom Anbieter über die Registrierungsschlüssel im Zusammenhang mit dieser Meldung generiert werden.|
|Schweregrad *|alertSeverity|Schweregrad der Meldung - vom Hersteller/Anbieter festgelegt. Mögliche Werte: `unknown`, `informational`, `low`, `medium`, `high`.|
|sourceMaterials|Zeichenfolgen-Sammlung|Hyperlinks (URIs) zum Quellmaterial in Bezug auf die Meldung, beispielsweise zur Benutzeroberfläche des Anbieters oder Protokoll-Suche usw.|
|Zustand *|alertStatus|Meldung-Zustand des Lebenszyklus (Phase). Mögliche Werte: `unknown`, `newAlert`, `inProgress`, `resolved`. ( [Unterstützt](../api/alert_update.md)Aktualisierung)|
|-Tags hinzugefügtes Markup|Zeichenfolgen-Sammlung|Benutzerdefinierbare Bezeichnungen, die auf eine Meldung angewendet werden und als Filterbedingungen dienen können (z. B. "HVA", "SAW" etc.) (Unterstützt [Aktualisierung](../api/alert_update.md)).|
|Titel *|Zeichenfolge|Titel der Meldung.|
|Auslöser|[AlertTrigger](alerttrigger.md) -Sammlung|Sicherheitsrelevante Informationen zu den spezifischen Eigenschaften, die die Meldung (Eigenschaften, die in der Meldung angezeigt werden) ausgelöst haben. Meldungen können Informationen zu mehreren Benutzern, Hosts, Dateien, IP-Adressen enthalten. Dieses Feld zeigt an, welche Eigenschaften die Generierung einer Meldung ausgelöst haben.|
|userStates|[UserSecurityState](usersecuritystate.md) -Sammlung|Sicherheitsbezogene Zustandsinformationen, die vom Anbieter über die Benutzerkonten im Zusammenhang mit dieser Meldung generiert werden.|
|vendorInformation *|[securityVendorInformation](securityvendorinformation.md)|Komplexer Typ, der Angaben zum Sicherheitsprodukt/Dienstleister, Anbieter und Unteranbieter enthält (z. B. Lieferant=Microsoft; Anbieter=Windows Defender ATP; Unteranbieter=AppLocker).|
|vulnerabilityStates|[VulnerabilityState](vulnerabilitystate.md) -Sammlung|Eine oder mehrere Sicherheitslücken im Zusammenhang mit dieser Benachrichtigung zur Bedrohungsnachricht.|
(\* Kennzeichnet ein Pflichtfeld.)

## <a name="relationships"></a>Beziehungen

Keine.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alert"
}-->

```json
{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [{"@odata.type": "microsoft.graph.cloudAppSecurityState"}],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [{"@odata.type": "microsoft.graph.fileSecurityState"}],
  "hostStates": [{"@odata.type": "microsoft.graph.hostSecurityState"}],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [{"@odata.type": "microsoft.graph.malwareState"}],
  "networkConnections": [{"@odata.type": "microsoft.graph.networkConnection"}],
  "processes": [{"@odata.type": "microsoft.graph.process"}],
  "recommendedActions": ["String"],
  "registryKeyStates": [{"@odata.type": "microsoft.graph.registryKeyState"}],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [{"@odata.type": "microsoft.graph.alertTrigger"}],
  "userStates": [{"@odata.type": "microsoft.graph.userSecurityState"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "vulnerabilityStates": [{"@odata.type": "microsoft.graph.vulnerabilityState"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->