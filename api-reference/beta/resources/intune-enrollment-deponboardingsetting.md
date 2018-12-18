---
title: Ressourcentyp depOnboardingSetting
description: Die DepOnboardingSetting stellt eine Instanz des Diensts Apple DEP Onboarded Sie Intune wird. Die Dienstinstanz Onboarded verwaltet ein Apple Token-zum Synchronisieren von Daten zwischen Apple und Intune.
author: tfitzmac
ms.openlocfilehash: ac38b1716dd156c95fda9cee8fb76a9f75921b0f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341160"
---
# <a name="deponboardingsetting-resource-type"></a>Ressourcentyp depOnboardingSetting

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die DepOnboardingSetting stellt eine Instanz des Diensts Apple DEP Onboarded Sie Intune wird. Die Dienstinstanz Onboarded verwaltet ein Apple Token-zum Synchronisieren von Daten zwischen Apple und Intune.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|[DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Auflistung|Listeneigenschaften und Beziehungen der [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekte.|
|[Abrufen von depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Lesen Sie Eigenschaften und Beziehungen des [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts.|
|[Erstellen von depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Erstellen eines neuen [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts.|
|[DepOnboardingSetting löschen](../api/intune-enrollment-deponboardingsetting-delete.md)|Keines|Löscht eine [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).|
|[DepOnboardingSetting aktualisieren](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Aktualisieren Sie die Eigenschaften eines [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts.|
|[GetEncryptionPublicKey-Funktion](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|String|Rufen Sie einen öffentlichen Schlüssel zum Verschlüsseln des Apple Gerät Registrierung Programms token ab|
|[UploadDepToken Aktion](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|Keines|Lädt ein neues Gerät Registrierung Programm Token hoch|
|[SyncWithAppleDeviceEnrollmentProgram Aktion](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|Keines|Zwischen Apple Gerät Registrierung Programm und Intune synchronisiert|
|[ShareForSchoolDataSyncService Aktion](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|Keine|Noch nicht dokumentiert|
|[UnshareForSchoolDataSyncService Aktion](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|UUID für das Objekt|
|appleIdentifier|String|Die Apple-ID verwendet, um das aktuelle Token abzurufen.|
|tokenExpirationDateTime|DateTimeOffset|Wenn das Token abläuft.|
|lastModifiedDateTime|DateTimeOffset|Wenn der Dienst Onboarded wurde.|
|lastSuccessfulSyncDateTime|DateTimeOffset|Wenn der Dienst letzten Syned mit Intune|
|lastSyncTriggeredDateTime|DateTimeOffset|Wenn Intune zuletzt eine Synchronisierung angefordert wird.|
|shareTokenWithSchoolDataSyncService|Boolesch|Unabhängig davon, ob die Datenausführungsverhinderung token Freigabe mit dem Schule Daten Sync-Dienst aktiviert ist.|
|lastSyncErrorCode|Int32|Fehlercode von Apple während der letzten Synchronisierung der Datenausführungsverhinderung gemeldet.|
|"TokenType"|[depTokenType](../resources/intune-enrollment-deptokentype.md)|Ruft ab oder legt ihn fest die Datenausführungsverhinderung Token. Mögliche Werte sind: `none`, `dep` und `appleSchoolManager`.|
|tokenName|String|Anzeigename für die Datenausführungsverhinderung Token|
|syncedDeviceCount|Int32|Ruft synchronisierter Anzahl der Geräte|
|defaultProfileDisplayName|String|Ruft synchronisierter Anzahl der Geräte|
|dataSharingConsentGranted|Boolesch|Stimmen Sie gewährte Zugriffsberechtigungen für die Datenfreigabe mit Apple Dep-Dienst|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Standardmäßige iOS Registrierung Profil|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Standardprofil für Mac OS-Registrierung|
|enrollmentProfiles|[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Auflistung|Die Registrierung Profile.|
|importedAppleDeviceIdentities|[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Auflistung|Die importierten Apple Gerät Identitäten.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depOnboardingSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "lastSyncTriggeredDateTime": "String (timestamp)",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1024,
  "tokenType": "String",
  "tokenName": "String",
  "syncedDeviceCount": 1024,
  "defaultProfileDisplayName": "String",
  "dataSharingConsentGranted": true
}
```





