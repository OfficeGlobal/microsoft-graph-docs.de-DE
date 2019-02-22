---
title: mobileAppTroubleshootingEvent-Ressourcentyp
description: Beschreibt die mobileAppTroubleshootingEvent-Ressource der Microsoft Graph-API für InTune, die mehrere Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cfa126fea86c7edb302953efc3b88376f2d68a09
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162944"
---
# <a name="mobileapptroubleshootingevent-resource-type"></a>mobileAppTroubleshootingEvent-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Ereignis, das den Installationsstatus einer Benutzer-Geräteanwendung für die Geräteverwaltung und die Problembehandlung von Ereignis Workflows darstellt.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MobileAppTroubleshootingEvents aufListen](../api/intune-shared-mobileapptroubleshootingevent-list.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekte.|
|[MobileAppTroubleshootingEvent abrufen](../api/intune-shared-mobileapptroubleshootingevent-get.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.|
|[MobileAppTroubleshootingEvent erstellen](../api/intune-shared-mobileapptroubleshootingevent-create.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Erstellen eines neuen [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.|
|[MobileAppTroubleshootingEvent löschen](../api/intune-shared-mobileapptroubleshootingevent-delete.md)|Keine|Löscht eine [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).|
|[MobileAppTroubleshootingEvent aktualisieren](../api/intune-shared-mobileapptroubleshootingevent-update.md)|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Aktualisieren der Eigenschaften eines [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|UUID für das Objekt.|
|**Problembehandlung**|
|Zusatzinformationen|[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung|Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen über das von [DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) geerbte Problem Behandlungs Ereignis bereitstellen.|
|applicationId|Zeichenfolge|InTune-Anwendungsbezeichner.|
|correlationId|Zeichenfolge|ID, die zum Nachverfolgen des Fehlers im Dienst verwendet wird. |
|eventDateTime|DateTimeOffset|Uhrzeit, zu der das Ereignis aufgetreten ist. |
|eventName|Zeichenfolge|Ereignis Name, der dem Problem Behandlungs Ereignis entspricht. Optional|
|Geschichte|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) -Sammlung|InTune-Problem Behandlungs Historie für mobile Anwendungen|
|managedDeviceIdentifier|Zeichenfolge|Von Intune erstellter oder erfasster Gerätebezeichner|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur. Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|userId|Zeichenfolge|Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|**deviceManagement**|
|appLogCollectionRequests|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Sammlung|Die Collection-Eigenschaft von AppLogUploadRequest.|


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
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
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




