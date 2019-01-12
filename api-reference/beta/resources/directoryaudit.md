---
title: Ressourcentyp directoryAudit
description: Diese Ressource stellt die Directory Audit Elemente mit seiner Sammlung
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f980208788731206dc58870635644a1f3edc4c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991783"
---
# <a name="directoryaudit-resource-type"></a>Ressourcentyp directoryAudit
Diese Ressource stellt die Directory Audit Elemente mit seiner Sammlung


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |Die Directory Audit-Elemente in der Auflistung und deren Eigenschaften aufgelistet.|
|[Abrufen von directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |Rufen Sie ein bestimmtes Verzeichnis Audit-Element und seine Eigenschaften.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|activityDateTime|DateTimeOffset|Gibt an, das Datum und die Zeit, die die Aktivität ausgeführt wurde. Der Zeitstempel-Typ ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|activityDisplayName|Zeichenfolge|Gibt den Namen der Aktivität oder der Name des Vorgangs (z. B. "Erstellen von Benutzer", "Add Mitglied der Gruppe"). Eine Liste der Aktivitäten protokolliert finden Sie in der [Liste von Azure Ad-Aktivität](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).|
|additionalDetails|[KeyValue](keyvalue.md) -Auflistung|Gibt zusätzliche Informationen für die Aktivität an.|
|category|String|Gibt an, welche Ressourcenkategorie, die von der Aktivität gerichtet ist. (Zum Beispiel: die Verwaltung von usw. Gruppe Management..)|
|correlationId|GUID|Gibt eine eindeutige ID, mit deren Aktivitäten korrelieren, die über verschiedene Dienste erstrecken. Kann in Ablaufprotokolle zwischen Diensten verwendet werden.|
|id|Zeichenfolge| Gibt die eindeutige ID für die Aktivität an. Dies ist eine GUID.|
|initiatedBy|[auditActivityInitiator](auditactivityinitiator.md)|Gibt an, dass Informationen über den Benutzer oder die app die Aktivität initiiert hat.|
|loggedByService|Zeichenfolge|Gibt an, auf dem Dienst die Aktivität initiiert, Informationen (zum Beispiel: Self-Service-Kennwortverwaltung, Core Directory, B2C, Benutzer eingeladen, Microsoft Identity Manager, privilegierten Identity Management.|
|result|string| Gibt das Ergebnis der Aktivität an. Mögliche Werte sind: `success`, `failure`, `timeout`, `unknownFutureValue`.||
|resultReason|Zeichenfolge|Gibt die Ursache für Fehler an, ob das Ergebnis "Fehler" oder "Timeout" ist.|
|targetResources|[TargetResource](targetresource.md) -Auflistung|Gibt Informationen für die Ressource der Aktivitäten geändert wurde. Ressource Zieltyp können Benutzer, Gerät, Directory, App, Rolle, Gruppe, Richtlinie oder andere sein.

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
