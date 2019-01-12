---
title: Ressourcentyp mobileAppTroubleshootingEvent
description: Ereignis, das eine Anwendung für Benutzer Geräte darstellt installieren Status.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d26873b90941f27538a5c71e113a92bb5af1bf26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977325"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>Ressourcentyp mobileAppTroubleshootingEvent

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ereignis, das eine Anwendung für Benutzer Geräte darstellt installieren Status.

Erbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste mobileAppTroubleshootingEvents](../api/intune-troubleshooting-mobileapptroubleshootingevent-list.md)|[MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) -Auflistung|Listeneigenschaften und Beziehungen der [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) -Objekte.|
|[Abrufen von mobileAppTroubleshootingEvent](../api/intune-troubleshooting-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|Lesen Sie Eigenschaften und Beziehungen des [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) -Objekts.|
|[Erstellen von mobileAppTroubleshootingEvent](../api/intune-troubleshooting-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|Erstellen eines neuen [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) -Objekts.|
|[MobileAppTroubleshootingEvent löschen](../api/intune-troubleshooting-mobileapptroubleshootingevent-delete.md)|Keine|Löscht eine [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md).|
|[MobileAppTroubleshootingEvent aktualisieren](../api/intune-troubleshooting-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)|Aktualisieren Sie die Eigenschaften eines [MobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|eventDateTime|DateTimeOffset|Uhrzeit, zu der das Ereignis aufgetreten ist. Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|correlationId|Zeichenfolge|ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde. Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|managedDeviceIdentifier|Zeichenfolge|Von Intune erstellter oder erfasster Gerätebezeichner|
|userId|Zeichenfolge|Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.|
|applicationId|Zeichenfolge|Intune Anwendungsbezeichner.|
|Verlauf|[MobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) -Auflistung|Intune Mobile Anwendung Problembehandlung Historienelement|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "userId": "String",
  "applicationId": "String",
  "history": [
    {
      "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem",
      "occurrenceDateTime": "String (timestamp)"
    }
  ]
}
```





