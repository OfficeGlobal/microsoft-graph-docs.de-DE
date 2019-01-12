---
title: deviceManagementTroubleshootingEvent-Ressourcentyp
description: Ereignis, das einen allgemeinen Fehler darstellt
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd4fbf5448b9bd5347fd7cb4f7cfe5ef96790247
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917538"
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
|correlationId|Zeichenfolge|ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde.|

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



