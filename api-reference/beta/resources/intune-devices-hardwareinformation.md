---
title: Ressourcentyp hardwareInformation
description: Hardwareinformationen für ein bestimmtes Gerät.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32b6d0e637c477265a6d23f39e531ca89c7e490c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394824"
---
# <a name="hardwareinformation-resource-type"></a>Ressourcentyp hardwareInformation

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Hardwareinformationen für ein bestimmtes Gerät.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|serialNumber|Zeichenfolge|Seriennummer.|
|totalStorageSpace|Int64|Gesamtmenge des Speicherplatzes des Geräts.|
|freeStorageSpace|Int64|Freier Speicherplatz des Geräts.|
|imei|Zeichenfolge|IMEI|
|meid|Zeichenfolge|MEID|
|manufacturer|Zeichenfolge|Hersteller des Geräts.
|
|model|Zeichenfolge|Modell des Geräts.
|
|PhoneNumber|Zeichenfolge|Telefonnummer des Geräts.
|
|subscriberCarrier|Zeichenfolge|Abonnenten Netzbetreiber des Geräts|
|cellularTechnology|Zeichenfolge|Mobilfunk-Technologie des Geräts|
|wifiMac|Zeichenfolge|WLAN-MAC-Adresse des Geräts|
|operatingSystemLanguage|Zeichenfolge|Die Sprache des Betriebssystems des Geräts|
|isSupervised|Boolean|Überwachten Modus des Geräts|
|isEncrypted|Boolean|Status der Verschlüsselung des Geräts|
|isSharedDevice|Boolean|Freigegebene iPad|
|sharedDeviceCachedUsers|[SharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) -Auflistung|Alle Benutzer auf dem freigegebenen Apple-Gerät|
|tpmSpecificationVersion|Zeichenfolge|Zeichenfolge, die die Spezifikation, Version angibt.|
|operatingSystemEdition|Zeichenfolge|Zeichenfolge, die die Betriebssystem Edition angibt.|
|deviceFullQualifiedDomainName|Zeichenfolge|Gibt den vollqualifizierten Domänennamen des Geräts (falls vorhanden). Wenn das Gerät nicht Mitglied einer Domäne ist, wird eine leere Zeichenfolge zurückgegeben. |
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




