---
title: depOnboardingSetting-Ressourcentyp
description: Die depOnboardingSetting stellt eine Instanz des Apple DEP-Diensts dar, die an InTune übertragen wird. Die onboarded-Dienstinstanz verwaltet ein Apple-Token, mit dem Daten zwischen Apple und InTune synchronisiert werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a3c19a791f97b7cb40bdd2398fec4c1812fdcde
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145283"
---
# <a name="deponboardingsetting-resource-type"></a>depOnboardingSetting-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die depOnboardingSetting stellt eine Instanz des Apple DEP-Diensts dar, die an InTune übertragen wird. Die onboarded-Dienstinstanz verwaltet ein Apple-Token, mit dem Daten zwischen Apple und InTune synchronisiert werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DepOnboardingSettings aufListen](../api/intune-enrollment-deponboardingsetting-list.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekte.|
|[DepOnboardingSetting abrufen](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Lesen von Eigenschaften und Beziehungen des [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts.|
|[DepOnboardingSetting erstellen](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Erstellen eines neuen [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts.|
|[DepOnboardingSetting löschen](../api/intune-enrollment-deponboardingsetting-delete.md)|Keine|Löscht eine [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).|
|[DepOnboardingSetting aktualisieren](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Aktualisieren der Eigenschaften eines [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts.|
|[getEncryptionPublicKey-Funktion](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|Zeichenfolge|Abrufen eines öffentlichen Schlüssels zum Verschlüsseln des Apple-Geräte Registrierungsprogramm-Tokens|
|[uploadDepToken-Aktion](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|Keine|Lädt ein neues Token für das Geräte Registrierungsprogramm hoch|
|[syncWithAppleDeviceEnrollmentProgram-Aktion](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|Keine|Synchronisierung zwischen dem Apple-Geräte Registrierungsprogramm und InTune|
|[shareForSchoolDataSyncService-Aktion](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|Keine|Noch nicht dokumentiert|
|[unshareForSchoolDataSyncService-Aktion](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|UUID für das Objekt|
|appleIdentifier|String|Die Apple-ID, die zum Abrufen des aktuellen Tokens verwendet wird.|
|tokenExpirationDateTime|DateTimeOffset|Wenn das Token abläuft.|
|lastModifiedDateTime|DateTimeOffset|Wenn der Dienst an Bord war.|
|lastSuccessfulSyncDateTime|DateTimeOffset|Wenn der Dienst zuletzt mit InTune syned|
|lastSyncTriggeredDateTime|DateTimeOffset|Wenn InTune eine Synchronisierung zuletzt angefordert hat.|
|shareTokenWithSchoolDataSyncService|Boolescher Wert|Gibt an, ob die DEP-Token-Freigabe mit dem School Data Sync-Dienst aktiviert ist.|
|Lastsyncerrorcode wurden|Int32|Fehlercode, der von Apple während der letzten DEP-Synchronisierung gemeldet wurde.|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|Ruft den Typ der DEP-Token ab oder legt ihn fest. Mögliche Werte sind: `none`, `dep` und `appleSchoolManager`.|
|Tokenname|Zeichenfolge|Anzeige Name für DEP-Token|
|syncedDeviceCount|Int32|Ruft die Anzahl synchronisierter Geräte ab.|
|dataSharingConsentGranted|Boolescher Wert|Einwilligung zur Datenfreigabe mit Apple DEP Service|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Standardmäßiges iOS-Registrierungsprofil|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Standardmäßiges MacOs-Registrierungsprofil|
|enrollmentProfiles|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Sammlung|Die Registrierungs Profile.|
|importedAppleDeviceIdentities|[importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Sammlung|Die importierten Apple-Geräte Identitäten.|

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
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




