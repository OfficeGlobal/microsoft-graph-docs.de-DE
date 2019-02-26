---
title: Dem-Ressourcentyp
description: Hardware Informationen eines bestimmten Geräts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be7d87f1d596a4756b3e964cd57f29da60f1c468
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172877"
---
# <a name="hardwareinformation-resource-type"></a>Dem-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Hardware Informationen eines bestimmten Geräts.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|serialNumber|Zeichenfolge|Seriennummer.|
|totalStorageSpace|Int64|Der gesamte Speicherplatz des Geräts.|
|freeStorageSpace|Int64|Freier Speicherplatz des Geräts.|
|imei|Zeichenfolge|IMEI|
|meid|Zeichenfolge|MEID|
|manufacturer|Zeichenfolge|Hersteller des Geräts.
|
|model|Zeichenfolge|Modell des Geräts.
|
|PhoneNumber|String|Telefonnummer des Geräts.
|
|subscriberCarrier|Zeichenfolge|Teilnehmernetzbetreiber des Geräts|
|cellularTechnology|Zeichenfolge|Mobilfunktechnologie des Geräts|
|wifiMac|Zeichenfolge|WiFi-MAC-Adresse des Geräts|
|operatingSystemLanguage|Zeichenfolge|Betriebssystemsprache des Geräts|
|isSupervised|Boolean|Überwachter Modus des Geräts|
|isEncrypted|Boolean|Verschlüsselungsstatus des Geräts|
|isSharedDevice|Boolean|FreigeGebenes iPad|
|Shareddevicecachedusers wurden|[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) -Sammlung|Alle Benutzer auf dem freigegebenen Apple-Gerät|
|tpmSpecificationVersion|Zeichenfolge|Zeichenfolge, die die Spezifikationsversion angibt.|
|operatingSystemEdition|Zeichenfolge|Zeichenfolge, die die OS-Edition angibt.|
|deviceFullQualifiedDomainName|Zeichenfolge|Gibt den vollqualifizierten Domänennamen des Geräts zurück (sofern vorhanden). Wenn das Gerät nicht mit einer Domäne verbunden ist, wird eine leere Zeichenfolge zurückgegeben. |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Virtualisierungs-basierter Sicherheitshardware-Anforderungsstatus. Mögliche Werte: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Virtualisierungs-basierter Sicherheitsstatus. . Mögliche Werte sind: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements` und `other`.|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Status der LSA-Anmeldeinformationen (Local System Authority). . Mögliche Werte: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|

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




