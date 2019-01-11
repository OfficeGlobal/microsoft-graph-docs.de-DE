---
title: Ressourcentyp androidWorkProfileNineWorkEasConfiguration
description: Durch die Bereitstellung von Konfigurationen in dieses Profil können Sie anweisen den neun Arbeit e-Mail-Client auf Geräten Android Arbeit Profil zur Kommunikation mit einem Exchange-Server und Abrufen von e-Mails, Kontakte, Kalender, Aufgaben und Notizen. Darüber hinaus können Sie auch angeben wie viel e-Mails zu synchronisieren und wie oft das Gerät synchronisiert werden sollte.
localization_priority: Normal
ms.openlocfilehash: 3bc29aabb637c38fc90054e3100aef89d6a71a3d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847369"
---
# <a name="androidworkprofilenineworkeasconfiguration-resource-type"></a>Ressourcentyp androidWorkProfileNineWorkEasConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Durch die Bereitstellung von Konfigurationen in dieses Profil können Sie anweisen den neun Arbeit e-Mail-Client auf Geräten Android Arbeit Profil zur Kommunikation mit einem Exchange-Server und Abrufen von e-Mails, Kontakte, Kalender, Aufgaben und Notizen. Darüber hinaus können Sie auch angeben wie viel e-Mails zu synchronisieren und wie oft das Gerät synchronisiert werden sollte.

Erbt vom [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste androidWorkProfileNineWorkEasConfigurations](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-list.md)|[AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Objekte.|
|[Abrufen von androidWorkProfileNineWorkEasConfiguration](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-get.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Objekts.|
|[Erstellen von androidWorkProfileNineWorkEasConfiguration](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-create.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)|Erstellen eines neuen [AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Objekts.|
|[AndroidWorkProfileNineWorkEasConfiguration löschen](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-delete.md)|Keine|Löscht eine [AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).|
|[AndroidWorkProfileNineWorkEasConfiguration aktualisieren](../api/intune-deviceconfig-androidworkprofilenineworkeasconfiguration-update.md)|[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [AndroidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Authentifizierungsmethode für Exchange ActiveSync. Geerbt von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md). Mögliche Werte sind: `usernameAndPassword` und `certificate`.|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|Dauer des Zeit-e-Mail-sollte mit synchronisiert werden. Geerbt von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md). Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|E-Mail-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird. Geerbt von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md). Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.|
|hostName|String|Exchange-Speicherort (URL), die die Mail-app mit verbindet. Geerbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)|
|requireSsl|Boolean|Gibt an, ob SSL verwendet. Geerbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|Username-Attribut, das aus AAD entnommen und vor der Installation auf dem Gerät an dieses Profil eingefügt wird. Geerbt von [AndroidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md). Mögliche Werte: sind `username`, `userPrincipalName`, `samAccountName` und `primarySmtpAddress`.|
|syncCalendar|Boolean|Schaltet den Kalender wird synchronisiert. Wenn der Wert false im Kalender auf dem Gerät deaktiviert ist.|
|syncContacts|Boolean|Schaltet die Kontakte werden synchronisiert. Wenn es sich bei Festlegung auf "false" Kontakte auf dem Gerät deaktiviert sind.|
|syncTasks|Boolean|Schaltet Aufgaben werden synchronisiert. Wenn es sich bei Festlegung auf "false" Aufgaben auf dem Gerät deaktiviert sind.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Gerät Konfiguration Installationsstatus durch Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|identityCertificate|[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)|Identity-Zertifikat. Geerbt von [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)|

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





