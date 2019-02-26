---
title: managementCondition-Ressourcentyp
description: Verwaltungsbedingungen sind Ereignisse, die dynamisch ausgelöst werden können, beispielsweise Geofences, Zeit Zäune und Netzwerk Zäune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 594716867cec1dcef9e0fee87af21fb63af99df0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163105"
---
# <a name="managementcondition-resource-type"></a>managementCondition-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Verwaltungsbedingungen sind Ereignisse, die dynamisch ausgelöst werden können, beispielsweise Geofences, Zeit Zäune und Netzwerk Zäune.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ManagementConditions aufListen](../api/intune-fencing-managementcondition-list.md)|[managementCondition](../resources/intune-fencing-managementcondition.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [managementCondition](../resources/intune-fencing-managementcondition.md) -Objekte.|
|[ManagementCondition abrufen](../api/intune-fencing-managementcondition-get.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)|Lesen von Eigenschaften und Beziehungen des [managementCondition](../resources/intune-fencing-managementcondition.md) -Objekts.|
|[getManagementConditionsForPlatform-Funktion](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|[managementCondition](../resources/intune-fencing-managementcondition.md) -Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutiger Bezeichner für die Verwaltungsbedingung. Vom System generierter Wert, der bei der Erstellung zugewiesen wird.|
|uniqueName|Zeichenfolge|Eindeutiger Name für die Verwaltungsbedingung. Wird in Verwaltungs Bedingungsausdrücken verwendet.|
|displayName|Zeichenfolge|Der Administrator definierte Name der Verwaltungsbedingung.|
|description|Zeichenfolge|Die vom Administrator definierte Beschreibung der Verwaltungsbedingung.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde. Generierte Dienstseite.|
|modifiedDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde. Aktualisierte Dienstseite.|
|eTag|Zeichenfolge|ETag der Verwaltungsbedingung. Aktualisierte Dienstseite.|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung|Die entsprechenden Plattformen für diese Verwaltungsbedingung.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Sammlung|Die der Verwaltungsbedingung zugeordneten Verwaltungs Bedingungsanweisungen.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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




