---
title: windowsOfficeClientConfiguration-Ressourcentyp
description: Entität, in der die Office-Richtlinieneinstellungen für Windows beschrieben werden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 61b64b53fb5a4000b0e8c5366c5a821c6941ce61
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147740"
---
# <a name="windowsofficeclientconfiguration-resource-type"></a>windowsOfficeClientConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Entität, in der die Office-Richtlinieneinstellungen für Windows beschrieben werden.

Erbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsOfficeClientConfigurations aufListen](../api/intune-cirrus-windowsofficeclientconfiguration-list.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) -Objekte.|
|[WindowsOfficeClientConfiguration abrufen](../api/intune-cirrus-windowsofficeclientconfiguration-get.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) -Objekts.|
|[WindowsOfficeClientConfiguration erstellen](../api/intune-cirrus-windowsofficeclientconfiguration-create.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Erstellen eines neuen [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) -Objekts.|
|[WindowsOfficeClientConfiguration löschen](../api/intune-cirrus-windowsofficeclientconfiguration-delete.md)|Keine|Löscht eine [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).|
|[WindowsOfficeClientConfiguration aktualisieren](../api/intune-cirrus-windowsofficeclientconfiguration-update.md)|[windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)|Aktualisieren der Eigenschaften eines [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|ID der Office-Client Konfigurationsrichtlinie. Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)|
|userPreferencePayload|Stream|Einstellungs Einstellungen JSON-Zeichenfolge im Binärformat können diese Werte vom Benutzer außer Kraft gesetzt werden. Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)|
|policyPayload|Stream|JSON-Zeichenfolge für Richtlinieneinstellungen im Binärformat können diese Werte nicht vom Benutzer geändert werden. Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)|
|description|Zeichenfolge|Administrator: Beschreibung der Office-Client Konfigurationsrichtlinie. Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|Zeichenfolge|Vom Administrator bereitgestellter Name der Office-Client Konfigurationsrichtlinie. Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)|
|Priorität|Int32|Der Prioritätswert sollte für jede Richtlinie unter einem Mandanten eindeutig sein und für die Konfliktlösung verwendet werden, niedrigere Werte bedeuten eine hohe Priorität. Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|DateTime|Datum der letzten Änderung der Richtlinie. Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Zusammenfassung der Benutzer Einchecken für die Richtlinie. Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)|
|checkinStatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Sammlung|Liste der Office-Client Eincheckstatus. Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Sammlung|Die Liste der Gruppenzuweisungen für die Richtlinie. Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsOfficeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```



