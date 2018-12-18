---
title: Ressourcentyp hardwareInformation
description: Hardwareinformationen für ein bestimmtes Gerät.
author: tfitzmac
ms.openlocfilehash: c483aa800d920a50392d21c326cd20dea7b72e18
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334524"
---
# <a name="hardwareinformation-resource-type"></a>Ressourcentyp hardwareInformation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Hardwareinformationen für ein bestimmtes Gerät.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|serialNumber|String|Seriennummer.|
|totalStorageSpace|Int64|Gesamtmenge des Speicherplatzes des Geräts.|
|freeStorageSpace|Int64|Freier Speicherplatz des Geräts.|
|imei|String|IMEI|
|meid|String|MEID|
|manufacturer|String|Hersteller des Geräts.
|
|model|String|Modell des Geräts.
|
|PhoneNumber|String|Telefonnummer des Geräts.
|
|subscriberCarrier|String|Abonnenten Netzbetreiber des Geräts|
|cellularTechnology|String|Mobilfunk-Technologie des Geräts|
|wifiMac|String|WLAN-MAC-Adresse des Geräts|
|operatingSystemLanguage|String|Die Sprache des Betriebssystems des Geräts|
|isSupervised|Boolescher Wert|Überwachten Modus des Geräts|
|isEncrypted|Boolescher Wert|Status der Verschlüsselung des Geräts|
|isSharedDevice|Boolesch|Freigegebene iPad|
|sharedDeviceCachedUsers|[SharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) -Auflistung|Alle Benutzer auf dem freigegebenen Apple-Gerät|
|tpmSpecificationVersion|String|Zeichenfolge, die die Spezifikation, Version angibt.|
|operatingSystemEdition|String|Zeichenfolge, die die Betriebssystem Edition angibt.|
|deviceFullQualifiedDomainName|String|Gibt den vollqualifizierten Domänennamen des Geräts (falls vorhanden). Wenn das Gerät nicht Mitglied einer Domäne ist, wird eine leere Zeichenfolge zurückgegeben. |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Virtualisierung-basierte Hardware Anforderung Sicherheitsstatus. Mögliche Werte sind: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM` und `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Virtualisierung-basierte Sicherheitsstatus. . Mögliche Werte sind: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements` und `other`.|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Lokales System Autorität (LSA) Anmeldeinformationen Guard Status. . Mögliche Werte sind: `running`, `rebootRequired`, `notLicensed`, `notConfigured` und `virtualizationBasedSecurityNotRunning`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```





