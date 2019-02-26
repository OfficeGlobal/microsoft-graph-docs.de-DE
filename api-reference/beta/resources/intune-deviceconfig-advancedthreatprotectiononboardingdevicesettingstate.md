---
title: advancedThreatProtectionOnboardingDeviceSettingState-Ressourcentyp
description: ATP-Onboarding-Status für ein bestimmtes Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 488473f3bea28a6f12bd79fbe9d6e21d669eaad9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171834"
---
# <a name="advancedthreatprotectiononboardingdevicesettingstate-resource-type"></a>advancedThreatProtectionOnboardingDeviceSettingState-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

ATP-Onboarding-Status für ein bestimmtes Gerät.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AdvancedThreatProtectionOnboardingDeviceSettingStates aufListen](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-list.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekte.|
|[AdvancedThreatProtectionOnboardingDeviceSettingState abrufen](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-get.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Lesen von Eigenschaften und Beziehungen des [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.|
|[AdvancedThreatProtectionOnboardingDeviceSettingState erstellen](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-create.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Erstellen eines neuen [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.|
|[AdvancedThreatProtectionOnboardingDeviceSettingState löschen](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-delete.md)|Keine|Löscht eine [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).|
|[AdvancedThreatProtectionOnboardingDeviceSettingState aktualisieren](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-update.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Aktualisieren der Eigenschaften eines [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität|
|platformType|[deviceType](../resources/intune-shared-devicetype.md)|Geräte Plattformtyp. Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.|
|setting|Zeichenfolge|Klassenname und Eigenschaftenname der Einstellung|
|settingName|Zeichenfolge|Gemeldeter Einstellungsname|
|deviceId|Zeichenfolge|Gemeldete Geräte-ID|
|deviceName|Zeichenfolge|Gemeldeter Gerätename|
|userId|Zeichenfolge|Gemeldete Benutzer-ID|
|userEmail|String|Gemeldete Benutzer-E-Mail-Adresse|
|userName|Zeichenfolge|Gemeldeter Benutzername|
|userPrincipalName|String|Gemeldeter Benutzerprinzipalname|
|deviceModel|Zeichenfolge|Gemeldetes Gerätemodell|
|state|[Wurde](../resources/intune-shared-compliancestatus.md)|Der Kompatibilitätsstatus der Einstellung. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
  "id": "String (identifier)",
  "platformType": "String",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```




