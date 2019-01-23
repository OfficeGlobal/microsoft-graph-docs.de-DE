---
title: Ressourcentyp managementConditionStatement
description: Eine Management Condition-Anweisung ist eine Gruppe von Management-Bedingungen, die aktivieren/Geräte-Anwendung Konfigurationen deaktivieren, wenn alle darin enthaltenen Management erfüllt werden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3292dae241a3f79cc7d3417c93ccc1187c8b8d17
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395993"
---
# <a name="managementconditionstatement-resource-type"></a>Ressourcentyp managementConditionStatement

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Eine Management Condition-Anweisung ist eine Gruppe von Management-Bedingungen, die aktivieren/Geräte-Anwendung Konfigurationen deaktivieren, wenn alle darin enthaltenen Management erfüllt werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste managementConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung|Listeneigenschaften und Beziehungen der [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekte.|
|[Abrufen von managementConditionStatement](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Lesen Sie Eigenschaften und Beziehungen des [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.|
|[Erstellen von managementConditionStatement](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Erstellen eines neuen [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.|
|[ManagementConditionStatement löschen](../api/intune-fencing-managementconditionstatement-delete.md)|Keine|Löscht eine [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).|
|[ManagementConditionStatement aktualisieren](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Aktualisieren Sie die Eigenschaften eines [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.|
|[GetManagementConditionStatementExpressionString-Funktion](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|Noch nicht dokumentiert|
|[GetManagementConditionStatementsForPlatform-Funktion](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für die Verwaltung Condition-Anweisung. System generierten Wert, die beim Erstellen zugewiesen.|
|displayName|Zeichenfolge|Der Administrator definierter Name der Bedingung-Anweisung Management.|
|description|Zeichenfolge|Der Administrator definiert die Beschreibung der Management Condition-Anweisung.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, an die Management Condition-Anweisung erstellt wurde. Generierte Service-Seite.|
|modifiedDateTime|DateTimeOffset|Der Zeitpunkt der letzten Änderung die Management Condition-Anweisung. Aktualisierte Service-Seite.|
|Ausdruck|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|Die Verwaltung Bedingungsausdruck-Anweisung verwendet, um ausgewertet werden soll, wenn eine Management Anweisung Bedingung wurde aktiviert/deaktiviert.|
|eTag|Zeichenfolge|ETag der Management Condition-Anweisung. Aktualisierte Service-Seite.|
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




