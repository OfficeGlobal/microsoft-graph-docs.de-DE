---
title: Ressourcentyp managementConditionStatement
description: Eine Management Condition-Anweisung ist eine Gruppe von Management-Bedingungen, die aktivieren/Geräte-Anwendung Konfigurationen deaktivieren, wenn alle darin enthaltenen Management erfüllt werden.
author: tfitzmac
ms.openlocfilehash: ca0966edd64166479361f42816e36fd278dbc6b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347677"
---
# <a name="managementconditionstatement-resource-type"></a>Ressourcentyp managementConditionStatement

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Management Condition-Anweisung ist eine Gruppe von Management-Bedingungen, die aktivieren/Geräte-Anwendung Konfigurationen deaktivieren, wenn alle darin enthaltenen Management erfüllt werden.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste managementConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung|Listeneigenschaften und Beziehungen der [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekte.|
|[Abrufen von managementConditionStatement](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Lesen Sie Eigenschaften und Beziehungen des [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.|
|[Erstellen von managementConditionStatement](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Erstellen eines neuen [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.|
|[ManagementConditionStatement löschen](../api/intune-fencing-managementconditionstatement-delete.md)|Keines|Löscht eine [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).|
|[ManagementConditionStatement aktualisieren](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Aktualisieren Sie die Eigenschaften eines [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.|
|[GetManagementConditionStatementExpressionString-Funktion](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|Noch nicht dokumentiert|
|[GetManagementConditionStatementsForPlatform-Funktion](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die Verwaltung Condition-Anweisung. System generierten Wert, die beim Erstellen zugewiesen.|
|displayName|String|Der Administrator definierter Name der Bedingung-Anweisung Management.|
|description|String|Der Administrator definiert die Beschreibung der Management Condition-Anweisung.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, an die Management Condition-Anweisung erstellt wurde. Generierte Service-Seite.|
|modifiedDateTime|DateTimeOffset|Der Zeitpunkt der letzten Änderung die Management Condition-Anweisung. Aktualisierte Service-Seite.|
|Ausdruck|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|Die Verwaltung Bedingungsausdruck-Anweisung verwendet, um ausgewertet werden soll, wenn eine Management Anweisung Bedingung wurde aktiviert/deaktiviert.|
|eTag|String|ETag der Management Condition-Anweisung. Aktualisierte Service-Seite.|
|applicablePlatforms|[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung|Die entsprechenden Plattformen für diese Management Condition-Anweisung.
Dieser Wert ergibt Suche die Management Bedingungen verknüpft ist, für die Verwaltung von Bedingung-Anweisung die Warteschlange gestellt und Schnittpunkt der Plattformen.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managementConditions|[ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung|Die Management-Bedingungen, die die Verwaltung Condition-Anweisung zugeordnet sind.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





