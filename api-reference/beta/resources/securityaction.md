---
title: SecurityAction-Ressourcentyp
description: Ergreifen Sie Sofortmaßnahmen, um Bedrohungen mithilfe der Microsoft Graph-Sicherheits-SecurityAction-Entität zu schützen. Wenn ein Sicherheitsanalytiker einen neuen Indikator ermittelt, beispielsweise eine bösartige Datei, eine URL, eine Domäne oder eine IP-Adresse, kann der Schutz sofort in Ihren Microsoft-Sicherheitslösungen aktiviert werden. Aufrufen einer Aktion für einen bestimmten Anbieter, siehe alle ausgeführten Aktionen und Abbrechen einer Aktion, falls erforderlich. Testen Sie Sicherheitsaktionen mit Windows Defender ATP (demnächst), um bösartige Aktivitäten auf Ihren Windows-Endpunkten mithilfe von Eigenschaften zu blockieren, die in Warnungen oder bei Untersuchungen identifiziert wurden.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 405f12c2cf484651f8bcefc791c9dd24dae410bd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366987"
---
# <a name="securityaction-resource-type"></a>SecurityAction-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ergreifen Sie Sofortmaßnahmen, um Bedrohungen mithilfe der Microsoft Graph-Sicherheits-SecurityAction-Entität zu schützen. Wenn ein Sicherheitsanalytiker einen neuen Indikator ermittelt, beispielsweise eine bösartige Datei, eine URL, eine Domäne oder eine IP-Adresse, kann der Schutz sofort in Ihren Microsoft-Sicherheitslösungen aktiviert werden. Aufrufen einer Aktion für einen bestimmten Anbieter, siehe alle ausgeführten Aktionen und Abbrechen einer Aktion, falls erforderlich. Testen Sie Sicherheitsaktionen mit [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) (demnächst), um bösartige Aktivitäten auf Ihren Windows-Endpunkten mithilfe von Eigenschaften zu blockieren, die in Warnungen oder bei Untersuchungen identifiziert wurden.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp | Beschreibung |
|:-------------|:------------|:------------|
| [SecurityAction abrufen](../api/securityaction-get.md) | [securityAction](securityaction.md) | Lesen von Eigenschaften und Beziehungen des SecurityAction-Objekts. |
| [Erstellen von SecurityAction](../api/securityactions-post.md) | [securityAction](securityaction.md) | Erstellen Sie eine neue SecurityAction, indem Sie in der securityActions-Auflistung veröffentlichen. |
| [SecurityActions aufListen](../api/securityactions-list.md) | [SecurityAction](securityaction.md) -Auflistung | Rufen Sie eine SecurityAction-Objektsammlung ab. |
|[Abbrechen von SecurityAction](../api/securityaction-cancelsecurityaction.md)|Keine|Abbrechen eines Sicherheits Vorgangs.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|actionReason|Zeichenfolge|Grund für den Aufruf dieser Aktion.|
|appId|Zeichenfolge|Die Anwendungs-ID der aufrufenden Anwendung, die die Aktion gesendet hat (POST). Die Anwendungs-ID sollte aus dem auth-Token extrahiert und nicht manuell von der aufrufenden Anwendung eingegeben werden.|
|azureTenantId|Zeichenfolge|Azure-Mandanten-ID der Entität, um zu bestimmen, zu welchem Mandanten die Entität gehört (Unterstützung für mehrere Mandanten). Die azureTenantId sollte aus dem auth-Token extrahiert und nicht manuell von der aufrufenden Anwendung eingegeben werden.|
|completedDateTime|DateTimeOffset|Zeitstempel, als die Aktion abgeschlossen wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|createdDateTime|DateTimeOffset|Zeitstempel, wenn die Aktion erstellt wird. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|errorInfo|[resultInfo](resultinfo.md)| Fehlerinformationen, wenn die Aktion fehlschlägt.|
|id|string| Wird vom System erstellt, wenn die Aktion aufgenommen wird. Generierte GUID/eindeutiger Bezeichner. Schreibgeschützt.|
|lastActionDateTime|DateTimeOffset| Zeitstempel, als diese Aktion zuletzt aktualisiert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|name|Zeichenfolge| Name der Aktion.|
|parameters|[keyValuePair](keyvaluepair.md)-Sammlung| Auflistung von Parametern (Schlüssel-Wert-Paare), die zum Aufrufen der Aktion erforderlich sind, beispielsweise URL oder fileHash zum Blockieren usw.). **Erforderlich**|
|Staaten|[securityActionState](securityactionstate.md) -Sammlung|Sammlung von securityActionState, um den Verlauf einer Aktion beizubehalten.|
|status|string| Status der Aktion. Mögliche Werte: `NotStarted`, `Running`, `Completed`, `Failed`.|
|user|Zeichenfolge| Der Benutzerprinzipalname des angemeldeten Benutzers, der die Aktion gesendet hat (POST). Der Benutzer sollte aus dem auth-Token extrahiert werden und nicht manuell von der aufrufenden Anwendung eingegeben werden.|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|Komplexer Typ mit Details zum Sicherheitsprodukt/-Dienstanbieter, Anbieter und unter Anbieter (z. b. Vendor = Microsoft; Provider = Windows Defender ATP; Sub-Provider = AppLocker).|

## <a name="relationships"></a>Beziehungen

Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "actionReason": "String",
  "appId": "String",
  "azureTenantId": "String",
  "clientContext": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "errorInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "states": [{"@odata.type": "microsoft.graph.securityActionState"}],
  "status": "string",
  "user": "String",
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->