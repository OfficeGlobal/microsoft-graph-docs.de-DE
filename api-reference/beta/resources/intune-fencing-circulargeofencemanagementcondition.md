---
title: circularGeofenceManagementCondition-Ressourcentyp
description: Enthält die Informationen zum Definieren einer kreisförmigen Geofence-Verwaltungsbedingung, eines zu überwachenden Bereichs.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ff137d36478950315b1debe10ffe841f4ba0bf8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154180"
---
# <a name="circulargeofencemanagementcondition-resource-type"></a>circularGeofenceManagementCondition-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält die Informationen zum Definieren einer kreisförmigen Geofence-Verwaltungsbedingung, eines zu überwachenden Bereichs.


Erbt von [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[CircularGeofenceManagementConditions aufListen](../api/intune-fencing-circulargeofencemanagementcondition-list.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekte.|
|[CircularGeofenceManagementCondition abrufen](../api/intune-fencing-circulargeofencemanagementcondition-get.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Lesen von Eigenschaften und Beziehungen des [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekts.|
|[CircularGeofenceManagementCondition erstellen](../api/intune-fencing-circulargeofencemanagementcondition-create.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Erstellen eines neuen [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekts.|
|[CircularGeofenceManagementCondition löschen](../api/intune-fencing-circulargeofencemanagementcondition-delete.md)|Keine|Löscht eine [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).|
|[CircularGeofenceManagementCondition aktualisieren](../api/intune-fencing-circulargeofencemanagementcondition-update.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Aktualisieren der Eigenschaften eines [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutiger Bezeichner für die Verwaltungsbedingung. Vom System generierter Wert, der bei der Erstellung zugewiesen wird. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Zeichenfolge|Eindeutiger Name für die Verwaltungsbedingung. Wird in Verwaltungs Bedingungsausdrücken verwendet. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Zeichenfolge|Der Administrator definierte Name der Verwaltungsbedingung. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|Zeichenfolge|Die vom Administrator definierte Beschreibung der Verwaltungsbedingung. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde. Generierte Dienstseite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde. Aktualisierte Dienstseite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|Zeichenfolge|ETag der Verwaltungsbedingung. Aktualisierte Dienstseite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung|Die entsprechenden Plattformen für diese Verwaltungsbedingung. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|latitude|Double|Latitude in Grad, zwischen-90 und + 90 inklusive.|
|longitude|Gleitkommawert mit doppelter Genauigkeit|Längengrad, zwischen-180 und + 180 inklusive.|
|radiusInMeters|Einzel|Radius in Meter.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Sammlung|Die der Verwaltungsbedingung zugeordneten Verwaltungs Bedingungsanweisungen. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.circularGeofenceManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```




