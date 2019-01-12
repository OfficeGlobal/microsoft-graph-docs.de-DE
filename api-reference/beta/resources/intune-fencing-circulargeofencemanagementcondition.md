---
title: Ressourcentyp circularGeofenceManagementCondition
description: Enthält Informationen zum Definieren einer kreisförmige Geo-Zauns Management Bedingung ein Interessenbereich zum Überwachen.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: bd7ae4b50ab7ec1497544fe8247f5d6d7e80e083
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925364"
---
# <a name="circulargeofencemanagementcondition-resource-type"></a>Ressourcentyp circularGeofenceManagementCondition

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Informationen zum Definieren einer kreisförmige Geo-Zauns Management Bedingung ein Interessenbereich zum Überwachen.

Erbt vom [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste circularGeofenceManagementConditions](../api/intune-fencing-circulargeofencemanagementcondition-list.md)|[CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Auflistung|Listeneigenschaften und Beziehungen der [CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekte.|
|[Abrufen von circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-get.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Lesen Sie Eigenschaften und Beziehungen des [CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekts.|
|[Erstellen von circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-create.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Erstellen eines neuen [CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekts.|
|[CircularGeofenceManagementCondition löschen](../api/intune-fencing-circulargeofencemanagementcondition-delete.md)|Keine|Löscht eine [CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).|
|[CircularGeofenceManagementCondition aktualisieren](../api/intune-fencing-circulargeofencemanagementcondition-update.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|Aktualisieren Sie die Eigenschaften eines [CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für die Bedingung Management. System generierten Wert, die beim Erstellen zugewiesen. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Zeichenfolge|Eindeutiger Name für die Bedingung Management. In Management Bedingung Ausdrücken verwendet. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Zeichenfolge|Der Administrator definierter Name der Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|Zeichenfolge|Der Administrator definiert die Beschreibung der Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, an die Bedingung Management erstellt wurde. Generierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Die Zeit, die die Bedingung Management zuletzt geändert wurde. Aktualisierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|Zeichenfolge|ETag der Bedingung Management. Aktualisierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung|Die entsprechenden Plattformen für diese Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|latitude|Gleitkommawert mit doppelter Genauigkeit|Breitengrad zwischen-90 und + 90 inklusive in Grad.|
|longitude|Gleitkommawert mit doppelter Genauigkeit|Längengrad in zwischen-180 und inklusive und + 180 Grad.|
|radiusInMeters|Single|RADIUS in Meter.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managementConditionStatements|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung|Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|

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





