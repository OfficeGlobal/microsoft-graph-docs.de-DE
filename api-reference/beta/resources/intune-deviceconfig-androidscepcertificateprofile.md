---
title: androidScepCertificateProfile-Ressourcentyp
description: Android SCEP-Zertifikatprofil
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2e61a1cffd3518720b3a46f89f46e543659d6de
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148328"
---
# <a name="androidscepcertificateprofile-resource-type"></a>androidScepCertificateProfile-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Android SCEP-Zertifikatprofil


Erbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AndroidScepCertificateProfiles aufListen](../api/intune-deviceconfig-androidscepcertificateprofile-list.md)|[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekte.|
|[AndroidScepCertificateProfile abrufen](../api/intune-deviceconfig-androidscepcertificateprofile-get.md)|[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)|Lesen von Eigenschaften und Beziehungen des [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts.|
|[AndroidScepCertificateProfile erstellen](../api/intune-deviceconfig-androidscepcertificateprofile-create.md)|[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)|Erstellen eines neuen [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts.|
|[AndroidScepCertificateProfile löschen](../api/intune-deviceconfig-androidscepcertificateprofile-delete.md)|Keine|Löscht eine [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).|
|[AndroidScepCertificateProfile aktualisieren](../api/intune-deviceconfig-androidscepcertificateprofile-update.md)|[androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md)|Aktualisieren der Eigenschaften eines [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Eigenschaften renewalthresholdpercentage|Int32|Schwellenwert für die Zertifikaterneuerung. Gültige Werte 1 bis 99 geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|
|subjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Format des Zertifikatsantrags Teller namens. Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt. Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Alternativer Namenstyp des Zertifikats betreffs. Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt. Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|certificateValidityPeriodValue|Int32|Wert für den Gültigkeitszeitraum des Zertifikats. Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|
|Certificatevalidityperiodscale wurden|[Certificatevalidityperiodscale wurden](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Skalierung für den Gültigkeitszeitraum des Zertifikats. Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt. Mögliche Werte sind: `days`, `months` und `years`.|
|extendedKeyUsages|[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung|EKU-Einstellungen (Extended Key Usage). Diese Collection darf maximal 500 Elemente enthalten. Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|
|scepServerUrls|String collection|SCEP-Server-URL (s)|
|subjectNameFormatString|Zeichenfolge|Benutzerdefiniertes Format, das mit SubjectNameFormat = Custom verwendet werden soll. Beispiel: CN = {{Email Adresse}}, E = {Email Adresse}}, OU = Enterprise users, O = Contoso Corporation, L = Redmond, ST = WA, C = US|
|keyUsage|[keyUsages](../resources/intune-deviceconfig-keyusages.md)|SCEP-Schlüsselverwendung. Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.|
|keySize|[keySize](../resources/intune-deviceconfig-keysize.md)|SCEP-Schlüsselgröße. Mögliche Werte sind: `size1024` und `size2048`.|
|hashAlgorithm|[hashAlgorithm](../resources/intune-deviceconfig-hashalgorithms.md)|SCEP-Hash Algorithmus. Mögliche Werte sind: `sha1` und `sha2`.|
|subjectAlternativeNameFormatString|Zeichenfolge|Benutzerdefinierte Zeichenfolge, die das AAD-Attribut definiert.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|rootCertificate|[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)|Vertrauenswürdiges Stammzertifikat. Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|
|managedDeviceCertificateStates|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Sammlung|Zertifikatstatus für Geräte|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidScepCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "renewalThresholdPercentage": 1024,
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ],
  "scepServerUrls": [
    "String"
  ],
  "subjectNameFormatString": "String",
  "keyUsage": "String",
  "keySize": "String",
  "hashAlgorithm": "String",
  "subjectAlternativeNameFormatString": "String"
}
```




