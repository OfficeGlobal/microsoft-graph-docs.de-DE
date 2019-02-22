---
title: Für-Ressourcentyp
description: Office-Client Konfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a8371da85ee4bbc54943a8fbb29ec99dcb49a49
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150561"
---
# <a name="officeclientconfiguration-resource-type"></a>Für-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Office-Client Konfiguration.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[OfficeClientConfigurations aufListen](../api/intune-cirrus-officeclientconfiguration-list.md)|[für](../resources/intune-cirrus-officeclientconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [für](../resources/intune-cirrus-officeclientconfiguration.md) -Objekte.|
|[Für abrufen](../api/intune-cirrus-officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [für](../resources/intune-cirrus-officeclientconfiguration.md) -Objekts.|
|[assign-Aktion](../api/intune-cirrus-officeclientconfiguration-assign.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Sammlung|Ersetzen Sie alle Zielgruppen für eine Richtlinie.|
|[updatePriorities-Aktion](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|Keine|Aktualisieren der Richtlinien Prioritäten.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|ID der Office-Client Konfigurationsrichtlinie.|
|userPreferencePayload|Stream|Einstellungs Einstellungen JSON-Zeichenfolge im Binärformat können diese Werte vom Benutzer außer Kraft gesetzt werden.|
|policyPayload|Stream|JSON-Zeichenfolge für Richtlinieneinstellungen im Binärformat können diese Werte nicht vom Benutzer geändert werden.|
|description|Zeichenfolge|Noch nicht dokumentiert|
|displayName|Zeichenfolge|Administrator: Beschreibung der Office-Client Konfigurationsrichtlinie.|
|lastModifiedDateTime|DateTime|Datum der letzten Änderung der Richtlinie.|
|Priorität|Int32|Der Prioritätswert sollte für jede Richtlinie unter einem Mandanten eindeutig sein und für die Konfliktlösung verwendet werden, niedrigere Werte bedeuten eine hohe Priorität.|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Zusammenfassung der Benutzer Einchecken für die Richtlinie.|
|checkinStatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Sammlung|Liste der Office-Client Eincheckstatus.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Sammlung|Die Liste der Gruppenzuweisungen für die Richtlinie.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
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



