---
title: androidWorkProfileNineWorkEasConfiguration-Ressourcentyp
description: Durch die Bereitstellung von Konfigurationen in diesem Profil können Sie den neun Work-e-Mail-Client auf Android-Arbeitsprofil Geräten anweisen, mit einem Exchange-Server zu kommunizieren und e-Mails, Kontakte, Kalender, Aufgaben und Notizen zu erhalten. Darüber hinaus können Sie auch angeben, wie viele e-Mails synchronisiert werden sollen und wie oft das Gerät synchronisiert werden soll.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f62f18d655030da546084b69dd2edf77216eb333
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168810"
---
# <a name="androidworkprofilenineworkeasconfiguration-resource-type"></a>androidWorkProfileNineWorkEasConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Durch die Bereitstellung von Konfigurationen in diesem Profil können Sie den neun Work-e-Mail-Client auf Android-Arbeitsprofil Geräten anweisen, mit einem Exchange-Server zu kommunizieren und e-Mails, Kontakte, Kalender, Aufgaben und Notizen zu erhalten. Darüber hinaus können Sie auch angeben, wie viele e-Mails synchronisiert werden sollen und wie oft das Gerät synchronisiert werden soll.


Erbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AndroidWorkProfileNineWorkEasConfigurations aufListen](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-list.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Objekte.|
|[AndroidWorkProfileNineWorkEasConfiguration abrufen](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-get.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Objekts.|
|[AndroidWorkProfileNineWorkEasConfiguration erstellen](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-create.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)|Erstellen eines neuen [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Objekts.|
|[AndroidWorkProfileNineWorkEasConfiguration löschen](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-delete.md)|Keine|Löscht eine [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).|
|[AndroidWorkProfileNineWorkEasConfiguration aktualisieren](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-update.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)|Aktualisieren der Eigenschaften eines [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Objekts.|

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
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Authentifizierungsmethode für Exchange ActiveSync. Von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)geerbt. Mögliche Werte sind: `usernameAndPassword` und `certificate`.|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|Uhrzeit, zu der e-Mails synchronisiert werden sollen. Von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)geerbt. Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|E-Mail-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird. Von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)geerbt. Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.|
|hostName|String|Exchange-Speicherort (URL), mit dem die Mail-App eine Verbindung herstellt. Geerbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)|
|requireSsl|Boolescher Wert|Gibt an, ob SSL verwendet werden soll. Geerbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|UserName-Attribut, das von AAD entnommen und vor der Installation auf dem Gerät in dieses Profil eingefügt wird. Von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)geerbt. Mögliche Werte: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.|
|syncCalendar|Boolescher Wert|Schaltet die Synchronisierung des Kalenders ein. Bei Festlegung auf false wird der Kalender auf dem Gerät deaktiviert.|
|syncContacts|Boolescher Wert|Schaltet die Synchronisierungs Kontakte ein. Bei Festlegung auf false sind Kontakte auf dem Gerät deaktiviert.|
|syncTasks|Boolescher Wert|Schaltet Synchronisierungsaufgaben um. Bei Festlegung auf false werden Aufgaben auf dem Gerät deaktiviert.|

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
|identityCertificate|[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)|Identitätszertifikat. Geerbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileNineWorkEasConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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
  "authenticationMethod": "String",
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSsl": true,
  "usernameSource": "String",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```




