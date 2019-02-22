---
title: managementConditionStatement-Ressourcentyp
description: Eine Management Condition-Anweisung ist eine Gruppe von Verwaltungsbedingungen, die Geräte/Anwendungskonfigurationen aktivieren/deaktivieren, wenn alle enthaltenen Verwaltungsbedingungen erfüllt sind.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41b696ee92b3098ea06c55c923fb3058706414ce
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167473"
---
# <a name="managementconditionstatement-resource-type"></a>managementConditionStatement-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine Management Condition-Anweisung ist eine Gruppe von Verwaltungsbedingungen, die Geräte/Anwendungskonfigurationen aktivieren/deaktivieren, wenn alle enthaltenen Verwaltungsbedingungen erfüllt sind.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ManagementConditionStatements aufListen](../api/intune-fencing-managementconditionstatement-list.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekte.|
|[ManagementConditionStatement abrufen](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Lesen von Eigenschaften und Beziehungen des [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.|
|[ManagementConditionStatement erstellen](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Erstellen eines neuen [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.|
|[ManagementConditionStatement löschen](../api/intune-fencing-managementconditionstatement-delete.md)|Keine|Löscht eine [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).|
|[ManagementConditionStatement aktualisieren](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Aktualisieren der Eigenschaften eines [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.|
|[getManagementConditionStatementExpressionString-Funktion](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|Noch nicht dokumentiert|
|[getManagementConditionStatementsForPlatform-Funktion](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutiger Bezeichner für die Verwaltungs Bedingungsanweisung. Vom System generierter Wert, der bei der Erstellung zugewiesen wird.|
|displayName|Zeichenfolge|Der vom Administrator definierte Name der Verwaltungs Bedingungsanweisung.|
|description|Zeichenfolge|Die vom Administrator definierte Beschreibung der Verwaltungs Bedingungsanweisung.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Verwaltungs Bedingungsanweisung erstellt wurde. Generierte Dienstseite.|
|modifiedDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Anweisung für die Verwaltungsbedingung zuletzt geändert wurde. Aktualisierte Dienstseite.|
|Ausdruck|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|Der Ausdruck der Verwaltungs Bedingungsanweisung, mit dem ausgewertet wird, ob eine Anweisung für die Verwaltungsbedingung aktiviert/deaktiviert wurde.|
|eTag|Zeichenfolge|ETag der Verwaltungs Bedingungsanweisung. Aktualisierte Dienstseite.|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung|Die entsprechenden Plattformen für diese Verwaltungs Bedingungsanweisung.
Dies wird berechnet anhand der Verwaltungsbedingungen, die mit der Verwaltungs Bedingungsanweisung verbunden sind, und dem Auffinden der Schnittstelle der entsprechenden Plattformen.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md) -Sammlung|Die Verwaltungsbedingungen, die der Anweisung für die Verwaltungsbedingung zugeordnet sind.|

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




