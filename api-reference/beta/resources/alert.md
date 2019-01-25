---
title: Warnung Ressourcentyp
description: Stellt die potenzielle Sicherheitsrisiken in Mandant des Kunden, die von Microsoft oder Partner sicherheitslösungen angegeben haben. Verwenden Sie Warnungen zu vereinheitlichen und Problem sicherheitsverwaltung über alle integrierten Lösungen zu optimieren. Finden Sie weitere Informationen finden Sie unter der Beispielabfragen im Graph-Explorer.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c7973522b8593d38724ee40374f40d58d3408ff6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526200"
---
# <a name="alert-resource-type"></a>Warnung Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die potenzielle Sicherheitsrisiken in Mandant des Kunden, die von Microsoft oder Partner sicherheitslösungen angegeben haben. Verwenden Sie Warnungen zu vereinheitlichen und Problem sicherheitsverwaltung über alle integrierten Lösungen zu optimieren. Finden Sie weitere Informationen finden Sie unter der Beispielabfragen im [Graph-Explorer](https://developer.microsoft.com/graph/graph-explorer).

Warnungen können von anderen Anbietern aufgeführt, die in der [Microsoft Graph-Sicherheit (Übersicht)](security-api-overview.md)abgerufen werden.

## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp|Beschreibung|
|:---------------|:--------|:----------|
|[Warnung erhalten](../api/alert-get.md) | Alert |Lesen Sie Eigenschaften und die Beziehungen eines alert-Objekts.|
|[Warnung aktualisieren](../api/alert-update.md) | Alert |Ein alert-Objekt zu aktualisieren. |
|[Warnungen auflisten](../api/alert-list.md) | [Warnung](alert.md) -Auflistung |Rufen Sie eine Auflistung der alert-Objekts.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|activityGroupName|String|Name oder Alias der Aktivitätsgruppe (Angreifer) wird diese Warnung zugeordnet.|
|assignedTo|String|Name des der Analyst die Benachrichtigung wird für die Ursachenanalyse, Untersuchung oder Remediation (unterstützt [Aktualisieren](../api/alert-update.md)) zugewiesen.|
|azureSubscriptionId|String|Azure-Abonnement-ID vorhanden, wenn diese Warnung zu einer Azure Ressource verknüpft ist.|
|azureTenantId |String|Azure Active Directory-Mandanten-ID Erforderlich. |
|category|String|Die Kategorie der Warnung (z. B. CredentialTheft, Ransomware usw.).|
|closedDateTime|DateTimeOffset|Zeitpunkt, an dem die Benachrichtigung geschlossen wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Beispielsweise könnte Uhr UTC auf 1 Jan 2014 wie folgt aussehen: `'2014-01-01T00:00:00Z'` (unterstützt [Aktualisieren](../api/alert-update.md)).|
|cloudAppStates|[CloudAppSecurityState](cloudappsecuritystate.md) -Auflistung|Sicherheitsbezogene Statusinformationen vom Anbieter über die Cloud Anwendung/s mit dieser Warnung generiert ist.|
|comments|Zeichenfolgenauflistung|Kunden bereitgestellten Kommentare auf Benachrichtigung (für Kunden alert Management) (unterstützt [Aktualisieren](../api/alert-update.md)).|
|confidence|Int32|Vertrauen die Erkennungslogik (zwischen 1 und 100 Prozent).|
|createdDateTime |DateTimeOffset|Zeitpunkt, in dem die Benachrichtigung durch den Anbieter alert erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Erforderlich.|
|description|Zeichenfolge|Beschreibung der Warnung.|
|detectionIds|Zeichenfolgenauflistung|Festlegen von Warnungen im Zusammenhang mit dieser Warnung Entität (jede Warnung wird in der SIEM als separater Datensatz verschoben).|
|eventDateTime |DateTimeOffset|Zeitpunkt, an dem die Ereignisse, die als den Triggern die Benachrichtigung generiert bedient stattgefunden hat. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Erforderlich.|
|Feedback|alertFeedback|Analyst Feedback auf die Benachrichtigung. Mögliche Werte: sind `unknown`, `truePositive`, `falsePositive` und `benignPositive`. ( [Aktualisieren](../api/alert-update.md)unterstützt)|
|fileStates|[FileSecurityState](filesecuritystate.md) -Auflistung|Sicherheitsbezogene Statusinformationen vom Anbieter über die Dateien im Zusammenhang mit dieser Benachrichtigung generiert ist.|
|hostStates|[HostSecurityState](hostsecuritystate.md) -Auflistung|Sicherheitsbezogene Statusinformationen vom Anbieter über die Hosts im Zusammenhang mit dieser Benachrichtigung generiert ist.|
|id |string|Anbieter generierte GUID/Eindeutiger Bezeichner. Schreibgeschützt. Erforderlich.|
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt, an dem die Warnung Entität zuletzt geändert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|malwareStates|[MalwareState](malwarestate.md) -Auflistung|Malware im Zusammenhang mit dieser Benachrichtigung zur Bedrohungsanalyse.|
|networkConnections|[NetworkConnection](networkconnection.md) -Auflistung|Sicherheitsbezogene Statusinformationen vom Anbieter über die Netzwerkschnittstelle(n) im Zusammenhang mit dieser Benachrichtigung generiert ist.|
|Prozesse|[Prozess](process.md) -Auflistung|Sicherheitsbezogene Statusinformationen vom Anbieter zu Prozesse im Zusammenhang mit dieser Benachrichtigung generiert ist.|
|recommendedActions|Zeichenfolgenauflistung|Hersteller-Anbieter empfohlen unternommen werden aufgrund der Warnung (beispielsweise isolieren Machine, enforce2FA, neu abbilden Host).|
|registryKeyStates|[RegistryKeyState](registrykeystate.md) -Auflistung|Sicherheitsbezogene Statusinformationen mit vom Anbieter zu den Registrierungsschlüsseln generiert in Bezug auf diese Warnung.|
|Severity |alertSeverity|Warnung Schweregrad - vom Hersteller-Anbieter festgelegt. Mögliche Werte sind: `unknown`, `informational`, `low`, `medium` und `high`. Erforderlich.|
|sourceMaterials|Zeichenfolgenauflistung|Hyperlinks (URIs) zu Quellmaterials in Bezug auf die Benachrichtigung beispielsweise des Anbieters-Benutzeroberfläche für Warnungen oder Protokoll Suche usw..|
|status |alertStatus|Warnung Lebenszyklusstatus (Phase). Mögliche Werte: sind `unknown`, `newAlert`, `inProgress` und `resolved`. (unterstützt [Aktualisieren](../api/alert-update.md)). Erforderlich.|
|tags|Zeichenfolgenauflistung|Benutzer definierbare Beschriftungen, die angewendet werden soll, auf eine Warnung und dienen als Filter Bedingung (zum Beispiel "HVA", "MAUERN" usw.) (unterstützt [Aktualisieren](../api/alert-update.md)).|
|title |String|Titel der Warnung. Erforderlich.|
|Trigger|[AlertTrigger](alerttrigger.md) -Auflistung|Sicherheitsrelevante Informationen zu den spezifischen Eigenschaften, die die Benachrichtigung (Eigenschaften, die in der Benachrichtigung angezeigt wird) ausgelöst. Warnungen können Informationen zu mehreren Benutzern, Hosts, Dateien, Ip-Adressen enthalten. Dieses Feld zeigt an, welche Eigenschaften die Auslösung einer Warnung ausgelöst.|
|userStates|[UserSecurityState](usersecuritystate.md) -Auflistung|Sicherheitsbezogene Statusinformationen mit generiert vom Anbieter über die Benutzerkonten in Bezug auf diese Warnung.|
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|Komplexer Typ, das Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider enthält (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker). Erforderlich.|
|vulnerabilityStates|[VulnerabilityState](vulnerabilitystate.md) -Auflistung|Eine oder mehrere Sicherheitslücken im Zusammenhang mit dieser Benachrichtigung zur Bedrohungsanalyse.|

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
