---
title: Ressourcentyp locationManagementCondition
description: Enthält Informationen zum Definieren einer Speicherort Management Bedingung ein Interessenbereich zum Überwachen.
ms.openlocfilehash: 45f6fedf55c7a45147b9a8d988823666a4dc9988
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065630"
---
# <a name="locationmanagementcondition-resource-type"></a>Ressourcentyp locationManagementCondition

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Informationen zum Definieren einer Speicherort Management Bedingung ein Interessenbereich zum Überwachen.

Erbt vom [managementCondition](../resources/intune-fencing-managementcondition.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste locationManagementConditions](../api/intune-fencing-locationmanagementcondition-list.md)|[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Auflistung|Listeneigenschaften und Beziehungen der [LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Objekte.|
|[Abrufen von locationManagementCondition](../api/intune-fencing-locationmanagementcondition-get.md)|[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)|Lesen Sie Eigenschaften und Beziehungen des [LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die Bedingung Management. System generierten Wert, die beim Erstellen zugewiesen. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|String|Eindeutiger Name für die Bedingung Management. In Management Bedingung Ausdrücken verwendet. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Der Administrator definierter Name der Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|String|Der Administrator definiert die Beschreibung der Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, an die Bedingung Management erstellt wurde. Generierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Die Zeit, die die Bedingung Management zuletzt geändert wurde. Aktualisierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag der Bedingung Management. Aktualisierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung|Die entsprechenden Plattformen für diese Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managementConditionStatements|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung|Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





