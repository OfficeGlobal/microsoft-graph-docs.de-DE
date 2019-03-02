---
title: Warnungs Ressourcentyp
description: Stellt potenzielle Sicherheitsprobleme innerhalb eines Kundenmandanten dar, die von Microsoft oder Partner-Sicherheitslösungen identifiziert wurden. Verwenden Sie Warnungen, um das Sicherheitsproblem Management für alle integrierten Lösungen zu vereinheitlichen und zu rationalisieren. Weitere Informationen finden Sie in den Beispielabfragen im Graph-Explorer.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8fa945cc69b3bc7779ae9ce23e2ee672c48eb1f8
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30364577"
---
# <a name="alert-resource-type"></a>Warnungs Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt potenzielle Sicherheitsprobleme innerhalb eines Kundenmandanten dar, die von Microsoft oder Partner-Sicherheitslösungen identifiziert wurden. Verwenden Sie Warnungen, um das Sicherheitsproblem Management für alle integrierten Lösungen zu vereinheitlichen und zu rationalisieren. Weitere Informationen finden Sie in den Beispielabfragen im [Graph-Explorer](https://developer.microsoft.com/graph/graph-explorer).

Benachrichtigungen können von verschiedenen Sicherheitsanbietern abgerufen werden, die in der [Microsoft Graph-Sicherheitsübersicht](security-api-overview.md)aufgeführt sind.

## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[Warnung erhalten](../api/alert-get.md) | [alert](alert.md) |Liest die Eigenschaften und Beziehungen eines Alert-Objekts.|
|[Warnung aktualisieren](../api/alert-update.md) | [alert](alert.md) |Aktualisieren eines Alert-Objekts. |
|[Warnungen auflisten](../api/alert-list.md) | [Warnungs](alert.md) Sammlung |Rufen Sie eine Alert-Objektsammlung ab.|
|[Warnungen aktualisieren](../api/alert-updatealerts.md)|[Warnungs](alert.md) Sammlung|Aktualisieren Sie mehrere Warnungs Objekte.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|activityGroupName|Zeichenfolge|Name oder Alias der Aktivitätsgruppe (Angreifer), auf die diese Warnung zurückzuführen ist.|
|assignedTo|Zeichenfolge|Name des Analysten, dem die Warnung für Triage, Untersuchung oder Korrektur zugewiesen ist (unterstützt [Update](../api/alert-update.md)).|
|azureSubscriptionId|Zeichenfolge|Azure-Abonnement-ID, vorhanden, wenn diese Warnung mit einer Azure-Ressource verknüpft ist.|
|azureTenantId |Zeichenfolge|Azure Active Directory-Mandanten-ID. Erforderlich. |
|category|String|Kategorie der Warnung (beispielsweise credentialTheft, Ransomware usw.).|
|closedDateTime|DateTimeOffset|Zeitpunkt, zu dem die Warnung geschlossen wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: `'2014-01-01T00:00:00Z'` (unterstützt [Update](../api/alert-update.md)).|
|cloudAppStates|[cloudAppSecurityState](cloudappsecuritystate.md) -Sammlung|Sicherheitsbezogene Stateful-Informationen, die vom Anbieter über die Cloud-Anwendung/s mit dieser Warnung generiert wurden.|
|comments|String collection|Vom Kunden bereitgestellte Kommentare zu Alert (für die Kunden Benachrichtigungsverwaltung) (unterstützt [Update](../api/alert-update.md)).|
|confidence|Int32|Zuverlässigkeit der Erkennungslogik (Prozentsatz zwischen 1-100).|
|createdDateTime |DateTimeOffset|Zeitpunkt, zu dem die Warnung vom Warnungs Anbieter erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Erforderlich.|
|description|String|Warnungsbeschreibung.|
|detectionIds|String collection|Eine Gruppe von Warnungen im Zusammenhang mit dieser Benachrichtigungs Entität (jede Warnung wird als separater Datensatz in SIEM gedrückt).|
|eventDateTime |DateTimeOffset|Zeitpunkt, zu dem die Ereignisse, die als Auslöser dienten, um die Warnung zu generieren, aufgetreten sind. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Erforderlich.|
|Feedback|alertFeedback|Analysten Feedback zu der Warnung. Mögliche Werte: `unknown`, `truePositive`, `falsePositive`, `benignPositive`. (unterstützt [Update](../api/alert-update.md))|
|dateiStates|[fileSecurityState](filesecuritystate.md) -Sammlung|Vom Anbieter generierte sicherheitsbezogene Statusinformationen zu den Dateien, die mit dieser Warnung verbunden sind.|
|historyStates|[alertHistoryState](alerthistorystate.md) -Sammlung| Eine Auflistung von **alertHistoryStates** , die ein Überwachungsprotokoll aller an einer Warnung vorgenommenen Aktualisierungen umfasst. |
|hostStates|[hostSecurityState](hostsecuritystate.md) -Sammlung|Sicherheitsrelevante Statusinformationen, die vom Anbieter über die mit dieser Warnung verknüpften Hosts generiert wurden.|
|id |string|Vom Anbieter generierte GUID/Unique Identifier. Schreibgeschützt. Erforderlich.|
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt, zu dem die Benachrichtigungs Entität zuletzt geändert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|malwareStates|[malwareState](malwarestate.md) -Sammlung|Threat Intelligence im Zusammenhang mit Schadsoftware zu dieser Warnung.|
|networkConnections|[Network Connection](networkconnection.md) -Sammlung|Vom Anbieter generierte sicherheitsbezogene Statusinformationen zu den Netzwerkverbindungen, die mit dieser Warnung verbunden sind.|
|Prozesse|[Prozess](process.md) Sammlung|Vom Anbieter generierte sicherheitsbezogene Statusinformationen zu dem Prozess oder den Prozessen im Zusammenhang mit dieser Warnung.|
|recommendedActions|String collection|Empfohlene Aktion des Anbieters/Anbieters als Ergebnis der Warnung (beispielsweise isolieren von Computer, enforce2FA, reimage Host).|
|registryKeyStates|[registryKeyState](registrykeystate.md) -Sammlung|Vom Anbieter generierte sicherheitsbezogene Statusinformationen zu den Registrierungsschlüsseln, die mit dieser Warnung verbunden sind.|
|Schweregrad |alertSeverity|Warnungsschweregrad – festgelegt nach Anbieter/Anbieter. Mögliche Werte: `unknown`, `informational`, `low`, `medium`, `high`. Erforderlich.|
|sourceMaterials|String collection|Hyperlinks (URIs) zum Quellmaterial im Zusammenhang mit der Warnung, beispielsweise die Benutzeroberfläche des Anbieters für Warnungen oder die Protokollsuche usw.|
|status |alertStatus|Status des Warnungs Lebenszyklus (Stufe). Mögliche Werte: `unknown`, `newAlert`, `inProgress`, `resolved`. (unterstützt [Update](../api/alert-update.md)). Erforderlich.|
|tags|String-Sammlung|Benutzerdefinierbare Bezeichnungen, die auf eine Warnung angewendet werden können und als Filterbedingungen dienen können (beispielsweise "HVA", "SAW" usw.) (unterstützt [Update](../api/alert-update.md)).|
|title |Zeichenfolge|Warnungs Titel. Erforderlich.|
|löst|[alertTrigger](alerttrigger.md) -Sammlung|Sicherheitsbezogene Informationen zu den spezifischen Eigenschaften, die die Warnung ausgelöst haben (Eigenschaften, die in der Warnung angezeigt werden). Warnungen enthalten möglicherweise Informationen zu mehreren Benutzern, Hosts, Dateien und IP-Adressen. Dieses Feld gibt an, welche Eigenschaften die Warnungsgenerierung ausgelöst haben.|
|userStates|[userSecurityState](usersecuritystate.md) -Sammlung|Vom Anbieter generierte sicherheitsbezogene Statusinformationen zu den Benutzerkonten, die mit dieser Warnung verbunden sind.|
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|Komplexer Typ, der Details zum Sicherheitsprodukt/-Dienstanbieter,-Anbieter und-subprovider enthält (beispielsweise Vendor = Microsoft; Provider = Windows Defender ATP; subProvider = AppLocker). Erforderlich.|
|vulnerabilityStates|[vulnerabilityState](vulnerabilitystate.md) -Sammlung|Threat Intelligence in Bezug auf eine oder mehrere Sicherheitsanfälligkeiten im Zusammenhang mit dieser Warnung.|

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
  "historyStates": [{"@odata.type": "microsoft.graph.alertHistoryState"}],
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
<!--
{
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/alert.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
