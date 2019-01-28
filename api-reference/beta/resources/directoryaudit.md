---
title: directoryAudit-Ressourcentyp
description: Diese Ressource stellt Überwachungselemente des Verzeichnisses und seine Sammlung dar.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0f56dea1b07f0814c4b9f1295498c2555c98a2df
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573158"
---
# <a name="directoryaudit-resource-type"></a>directoryAudit-Ressourcentyp
Diese Ressource stellt Überwachungselemente des Verzeichnisses und seine Sammlung dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[List directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |Listet die Überwachungselemente des Verzeichnisses in der Sammlung und ihre Eigenschaften auf.|
|[Get directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |Gibt ein bestimmtes Überwachungselement des Verzeichnisses und seine Eigenschaften an.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|activityDateTime|DateTimeOffset|Gibt das Datum und die Uhrzeit der Ausführung der Aktivität an. Der Zeitstempeltyp liegt immer in UTC-Zeit vor. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|activityDisplayName|String|Gibt den Aktivitätsnamen oder den Vorgangsnamen an (z. B. "Benutzer erstellen", "Mitglied der Gruppe hinzufügen"). Eine Liste der protokollierten Aktivitäten finden Sie unter [Azure AD-Aktivitätsliste](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).|
|additionalDetails|[keyvalue](keyvalue.md)-Sammlung|Gibt weitere Details zur Aktivität an.|
|category|String|Gibt an, auf welche Ressourcenkategorie die Aktivität abzielt. (Beispiel: Benutzerverwaltung, Gruppenverwaltung usw.)|
|correlationId| String (Bezeichner) |Gibt eine eindeutige ID an, die bei der Korrelation von Aktivitäten hilft, die sich über verschiedene Dienste erstrecken. Kann für die Ablaufverfolgung von Protokollen über Dienste hinweg verwendet werden.|
|id|String| Gibt die eindeutige ID für die Aktivität an. Dies ist eine GUID.|
|initiatedBy|[auditActivityInitiator](auditactivityinitiator.md)|Gibt Informationen zum Benutzer oder der App an, der bzw. die die Aktivität initiiert hat.|
|loggedByService|String|Gibt Informationen dazu an, welcher Dienst die Aktivität ausgelöst hat (Beispiel: Self-Service-Kennwortverwaltung, Core Directory, B2C, Eingeladene Benutzer, Microsoft Identity Manager, Privileged Identity Management).|
|result|string| Gibt das Ergebnis der Aktivität an. Mögliche Werte sind: `success`, `failure`, `timeout`, `unknownFutureValue`.||
|resultReason|String|Gibt den Grund für den Fehler an, wenn das Ergebnis "Failure" oder "timeout" ist.|
|targetResources|[targetResource](targetresource.md)-Sammlung|Gibt Informationen dazu an, welche Ressource aufgrund der Aktivität geändert wurde. Der Zielressourcentyp kann Benutzer, Gerät, Verzeichnis, App, Rolle, Gruppe, Richtlinie oder Andere sein.

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
  "correlationId": "String (identifier)",
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
