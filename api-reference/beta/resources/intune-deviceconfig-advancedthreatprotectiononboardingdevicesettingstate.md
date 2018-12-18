---
title: Ressourcentyp advancedThreatProtectionOnboardingDeviceSettingState
description: ATP Onboarding Zustand für ein bestimmtes Gerät.
author: tfitzmac
ms.openlocfilehash: eecdcc1cbaf9c783da6dcf902281aa6394a842a2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310871"
---
# <a name="advancedthreatprotectiononboardingdevicesettingstate-resource-type"></a>Ressourcentyp advancedThreatProtectionOnboardingDeviceSettingState

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

ATP Onboarding Zustand für ein bestimmtes Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste advancedThreatProtectionOnboardingDeviceSettingStates](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-list.md)|[AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Auflistung|Listeneigenschaften und Beziehungen der [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekte.|
|[Abrufen von advancedThreatProtectionOnboardingDeviceSettingState](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-get.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Lesen Sie Eigenschaften und Beziehungen des [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.|
|[Erstellen von advancedThreatProtectionOnboardingDeviceSettingState](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-create.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Erstellen eines neuen [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.|
|[AdvancedThreatProtectionOnboardingDeviceSettingState löschen](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-delete.md)|Keines|Löscht eine [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).|
|[AdvancedThreatProtectionOnboardingDeviceSettingState aktualisieren](../api/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate-update.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Aktualisieren Sie die Eigenschaften eines [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|platformType|[deviceType](../resources/intune-shared-devicetype.md)|Gerätetyp-Plattform. Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.|
|setting|String|Klassenname und Eigenschaftenname der Einstellung|
|settingName|String|Gemeldeter Einstellungsname|
|deviceId|String|Gemeldete Geräte-ID|
|deviceName|String|Gemeldeter Gerätename|
|userId|String|Gemeldete Benutzer-ID|
|userEmail|String|Gemeldete Benutzer-E-Mail-Adresse|
|userName|String|Gemeldeter Benutzername|
|userPrincipalName|String|Gemeldeter Benutzerprinzipalname|
|deviceModel|String|Gemeldetes Gerätemodell|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Der Compliance-Zustand der Einstellung. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
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





