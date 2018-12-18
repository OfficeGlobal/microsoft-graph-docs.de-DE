---
title: Ressourcentyp windowsOfficeClientSecurityConfiguration
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 51c07fa58e392523940687dd178dd2aebe94f327
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318837"
---
# <a name="windowsofficeclientsecurityconfiguration-resource-type"></a>Ressourcentyp windowsOfficeClientSecurityConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert

Erbt vom [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsOfficeClientSecurityConfigurations](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-list.md)|[WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekte.|
|[Abrufen von windowsOfficeClientSecurityConfiguration](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-get.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekts.|
|[Erstellen von windowsOfficeClientSecurityConfiguration](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-create.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Erstellen eines neuen [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekts.|
|[WindowsOfficeClientSecurityConfiguration löschen](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-delete.md)|Keines|Löscht eine [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).|
|[WindowsOfficeClientSecurityConfiguration aktualisieren](../api/intune-cirrus-windowsofficeclientsecurityconfiguration-update.md)|[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|ID des die Richtlinie Office-Client-Konfiguration. Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userPreferencePayload|Stream|Vorgaben JSON-Zeichenfolge im Binärformat, können diese Werte vom Benutzer außer Kraft gesetzt werden. Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|policyPayload|Stream|Richtlinieneinstellungen für JSON-Zeichenfolge im Binärformat, diese Werte können nicht vom Benutzer geändert werden. Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|description|String|Admin bereitgestellte Beschreibung für den Office-Client Konfigurationsrichtlinie. Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|String|Admin Namen der Richtlinie ein Office-Client-Konfiguration bereitgestellt. Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|Priorität|Int32|Prioritätswert sollte eindeutigen Wert für jede Richtlinie unter einem Mandanten sein und für konfliktlösung verwendet werden, niedrigere Werte bedeuten, dass Priorität hoch ist. Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|DateTime|Zuletzt geänderte Datetime-Stempel der Richtlinie. Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Benutzer Einchecken Zusammenfassung für die Richtlinie ein. Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|checkinStatuses|[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung|Liste der Office-Client Einchecken Status. Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung|Die Liste der zugewiesenen Gruppe für die Richtlinie ein. Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsOfficeClientSecurityConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
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



