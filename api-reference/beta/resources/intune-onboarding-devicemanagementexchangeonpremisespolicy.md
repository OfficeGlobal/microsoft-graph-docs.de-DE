---
title: Ressourcentyp deviceManagementExchangeOnPremisesPolicy
description: Singleton-Entität, die die für einen Mandanten konfigurierte Richtlinie für Exchange Verbindungspfad darstellt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1c4f513242694228b53268772d9b2910fa40bbd2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990334"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a>Ressourcentyp deviceManagementExchangeOnPremisesPolicy

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Singleton-Entität, die die für einen Mandanten konfigurierte Richtlinie für Exchange Verbindungspfad darstellt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von deviceManagementExchangeOnPremisesPolicy](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekts.|
|[DeviceManagementExchangeOnPremisesPolicy aktualisieren](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|Aktualisieren Sie die Eigenschaften eines [DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Noch nicht dokumentiert|
|notificationContent|Binär|Der Text der Benachrichtigung, die Benutzern unter Quarantäne gestellte e-Mails durch diese Richtlinie gesendet wird. Hierbei handelt es sich um UTF8 codiert HTML-Byte-Array.|
|defaultAccessLevel|[deviceManagementExchangeAccessLevel](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|Access-Standardzustand in Exchange. Diese Regel gilt global für die gesamte Exchange-Organisation. Mögliche Werte: sind `none`, `allow`, `block` und `quarantine`.|
|accessRules|[DeviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) -Auflistung|Die Liste der Gerätezugriffs Regeln im Exchange. Die Access-Regeln gelten global für die gesamte Exchange-Organisation|
|knownDeviceClasses|[DeviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) -Auflistung|Die Liste der Geräteklassen bekannt, dass Exchange|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Die Exchange-Einstellungen für den lokalen, bedingten Zugriff. Für den lokalen, bedingten Zugriff müssen Geräte registriert und für den E-Mail-Zugriff kompatibel sein.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeOnPremisesPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "String (identifier)",
  "notificationContent": "binary",
  "defaultAccessLevel": "String",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "String",
        "type": "String"
      },
      "accessLevel": "String"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "String",
      "type": "String"
    }
  ]
}
```





