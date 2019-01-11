---
title: deviceManagementTroubleshootingEvent-Ressourcentyp
description: Ereignis, das einen allgemeinen Fehler darstellt
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 629483de20b903d2c7f361552cfd998af9858101
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861264"
---
# <a name="devicemanagementtroubleshootingevent-resource-type"></a>deviceManagementTroubleshootingEvent-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ereignis, das einen allgemeinen Fehler darstellt
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagementTroubleshootingEvents auflisten](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-list.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekte.|
|[deviceManagementTroubleshootingEvent abrufen](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-get.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.|
|[deviceManagementTroubleshootingEvent erstellen](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-create.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Erstellen eines neuen [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.|
|[deviceManagementTroubleshootingEvent löschen](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-delete.md)|Keine|Löscht ein [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt.|
|[deviceManagementTroubleshootingEvent aktualisieren](../api/intune-troubleshooting-devicemanagementtroubleshootingevent-update.md)|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Aktualisieren der Eigenschaften eines [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|UUID für das Objekt|
|eventDateTime|DateTimeOffset|Uhrzeit, zu der das Ereignis aufgetreten ist.|
|correlationId|String|ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String"
}
```



