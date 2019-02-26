---
title: managedDeviceCertificateState-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49ec8d739c3018a9aaace7dd0d972a1ac1c87141
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164778"
---
# <a name="manageddevicecertificatestate-resource-type"></a>managedDeviceCertificateState-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Noch nicht dokumentiert.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ManagedDeviceCertificateStates aufListen](../api/intune-deviceconfig-manageddevicecertificatestate-list.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekte.|
|[ManagedDeviceCertificateState abrufen](../api/intune-deviceconfig-manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Lesen von Eigenschaften und Beziehungen des [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts.|
|[ManagedDeviceCertificateState erstellen](../api/intune-deviceconfig-manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Erstellen eines neuen [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts.|
|[ManagedDeviceCertificateState löschen](../api/intune-deviceconfig-manageddevicecertificatestate-delete.md)|Keine|Löscht eine [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).|
|[ManagedDeviceCertificateState aktualisieren](../api/intune-deviceconfig-manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Aktualisieren der Eigenschaften eines [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|Deviceplatform wurde|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|Geräteplattform. Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.|
|certificateKeyUsage|[keyUsages](../resources/intune-deviceconfig-keyusages.md)|Schlüsselverwendung. Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.|
|certificateValidityPeriodUnits|[Certificatevalidityperiodscale wurden](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Gültigkeitszeitraum Einheiten. Mögliche Werte sind: `days`, `months` und `years`.|
|certificateIssuanceState|[certificateIssuanceStates](../resources/intune-deviceconfig-certificateissuancestates.md)|VeröffentlichungsStatus. Mögliche Werte sind: `unknown`, `challengeIssued`, `challengeIssueFailed` `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` `enrollmentNotNeeded` `revoked`,,,,,,,, `removedFromCollection`,, `installed` ,,,,,, `renewVerified` `installFailed` `issueFailed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.|
|certificateKeyStorageProvider|[keyStorageProviderOption](../resources/intune-deviceconfig-keystorageprovideroption.md)|Schlüsselspeicheranbieter. Mögliche Werte: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|certificateSubjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Format des Antragstellernamens. Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateSubjectAlternativeNameFormat|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Format für alternative Antragstellernamen. Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Widerrufen des Status. Mögliche Werte: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateProfileDisplayName|Zeichenfolge|Anzeigename des Zertifikat Profils|
|deviceDisplayName|Zeichenfolge|Anzeigename des Geräts|
|userDisplayName|Zeichenfolge|Anzeigename des Benutzers.
|
|certificateExpirationDateTime|DateTimeOffset|Zertifikatablaufdatum|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|Letzte Änderung des Zertifikat Ausstellungs Status|
|lastCertificateStateChangeDateTime|DateTimeOffset|Letzte Änderung des Zertifikat Ausstellungs Status|
|certificateIssuer|Zeichenfolge|Aussteller|
|certificateThumbprint|Zeichenfolge|Fingerabdruck|
|certificateSerialNumber|Zeichenfolge|Seriennummer|
|certificateKeyLength|Int32|Schlüssellänge|
|certificateEnhancedKeyUsage|Zeichenfolge|Erweiterte Schlüsselverwendung|
|certificateValidityPeriod|Int32|Gültigkeitszeitraum|
|certificateSubjectNameFormatString|Zeichenfolge|Formatzeichenfolge für den Antragstellernamen für benutzerdefinierte Antragstellernamen Formate|
|certificateSubjectAlternativeNameFormatString|Zeichenfolge|Formatzeichenfolge für alternative Antragstellernamen für benutzerdefinierte Formate|
|certificateIssuanceDateTime|DateTimeOffset|Veröffentlichungsdatum|
|certificateErrorCode|Int32|Fehlercode|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceCertificateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "String (identifier)",
  "devicePlatform": "String",
  "certificateKeyUsage": "String",
  "certificateValidityPeriodUnits": "String",
  "certificateIssuanceState": "String",
  "certificateKeyStorageProvider": "String",
  "certificateSubjectNameFormat": "String",
  "certificateSubjectAlternativeNameFormat": "String",
  "certificateRevokeStatus": "String",
  "certificateProfileDisplayName": "String",
  "deviceDisplayName": "String",
  "userDisplayName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateLastIssuanceStateChangedDateTime": "String (timestamp)",
  "lastCertificateStateChangeDateTime": "String (timestamp)",
  "certificateIssuer": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateKeyLength": 1024,
  "certificateEnhancedKeyUsage": "String",
  "certificateValidityPeriod": 1024,
  "certificateSubjectNameFormatString": "String",
  "certificateSubjectAlternativeNameFormatString": "String",
  "certificateIssuanceDateTime": "String (timestamp)",
  "certificateErrorCode": 1024
}
```




