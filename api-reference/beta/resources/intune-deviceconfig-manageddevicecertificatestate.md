---
title: Ressourcentyp managedDeviceCertificateState
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 087bd1e6ed1eb9c065d1c2f0f3a03941d77cc7bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844044"
---
# <a name="manageddevicecertificatestate-resource-type"></a>Ressourcentyp managedDeviceCertificateState

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste managedDeviceCertificateStates](../api/intune-deviceconfig-manageddevicecertificatestate-list.md)|[ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Auflistung|Listeneigenschaften und Beziehungen der [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekte.|
|[Abrufen von managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Lesen Sie Eigenschaften und Beziehungen des [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts.|
|[Erstellen von managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Erstellen eines neuen [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts.|
|[ManagedDeviceCertificateState löschen](../api/intune-deviceconfig-manageddevicecertificatestate-delete.md)|Keine|Löscht eine [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).|
|[ManagedDeviceCertificateState aktualisieren](../api/intune-deviceconfig-manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Aktualisieren Sie die Eigenschaften eines [ManagedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|devicePlatform|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|Geräteplattform. Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.|
|certificateKeyUsage|[keyUsages](../resources/intune-deviceconfig-keyusages.md)|Enhanced Key Usage. Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.|
|certificateValidityPeriodUnits|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Gültigkeit Period Einheiten. Mögliche Werte sind: `days`, `months` und `years`.|
|certificateIssuanceState|[certificateIssuanceStates](../resources/intune-deviceconfig-certificateissuancestates.md)|Veröffentlichungslizenzen Zustand. Mögliche Werte sind: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.|
|certificateKeyStorageProvider|[keyStorageProviderOption](../resources/intune-deviceconfig-keystorageprovideroption.md)|Wichtige Speicheranbieter. Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.|
|certificateSubjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Format des Antragstellernamen. Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateSubjectAlternativeNameFormat|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Subject alternative Name-Format. Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|REVOKE-Status. Mögliche Werte sind: `none`, `pending`, `issued`, `failed` und `revoked`.|
|certificateProfileDisplayName|String|Profil der Anzeigename des Zertifikats|
|deviceDisplayName|String|Anzeigename des Geräts|
|userDisplayName|String|Anzeigename des Benutzers.
|
|certificateExpirationDateTime|DateTimeOffset|Ablaufdatum des Zertifikats|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|Änderung des letzten Zertifikat Veröffentlichungslizenzen|
|lastCertificateStateChangeDateTime|DateTimeOffset|Änderung des letzten Zertifikat Veröffentlichungslizenzen|
|certificateIssuer|String|Aussteller|
|certificateThumbprint|String|Fingerabdruck|
|Zertifikatsseriennummer|String|Seriennummer|
|certificateKeyLength|Int32|Schlüssellänge|
|certificateEnhancedKeyUsage|String|Erweiterte Schlüsselverwendung|
|certificateValidityPeriod|Int32|Gültigkeitsdauer|
|certificateSubjectNameFormatString|String|Subject Name Formatzeichenfolge für benutzerdefinierte Subject Namensformate|
|certificateSubjectAlternativeNameFormatString|String|Subject alternative Name Formatzeichenfolge für benutzerdefinierte Formate|
|certificateIssuanceDateTime|DateTimeOffset|Veröffentlichungslizenzen Datum|
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





