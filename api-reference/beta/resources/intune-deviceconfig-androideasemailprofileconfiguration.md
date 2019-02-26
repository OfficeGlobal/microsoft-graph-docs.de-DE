---
title: androidEasEmailProfileConfiguration-Ressourcentyp
description: Durch die Bereitstellung von Konfigurationen in diesem Profil können Sie den systemeigenen e-Mail-Client auf KNOX-Geräten anweisen, mit einem Exchange-Server zu kommunizieren und e-Mails, Kontakte, Kalender, Aufgaben und Notizen zu erhalten. Darüber hinaus können Sie auch angeben, wie viele e-Mails synchronisiert werden sollen und wie oft das Gerät synchronisiert werden soll.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 497a629ee500bc522e0ab2c0eb6b7b530983b956
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175199"
---
# <a name="androideasemailprofileconfiguration-resource-type"></a>androidEasEmailProfileConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Durch die Bereitstellung von Konfigurationen in diesem Profil können Sie den systemeigenen e-Mail-Client auf KNOX-Geräten anweisen, mit einem Exchange-Server zu kommunizieren und e-Mails, Kontakte, Kalender, Aufgaben und Notizen zu erhalten. Darüber hinaus können Sie auch angeben, wie viele e-Mails synchronisiert werden sollen und wie oft das Gerät synchronisiert werden soll.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AndroidEasEmailProfileConfigurations aufListen](../api/intune-deviceconfig-androideasemailprofileconfiguration-list.md)|[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekte.|
|[AndroidEasEmailProfileConfiguration abrufen](../api/intune-deviceconfig-androideasemailprofileconfiguration-get.md)|[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekts.|
|[AndroidEasEmailProfileConfiguration erstellen](../api/intune-deviceconfig-androideasemailprofileconfiguration-create.md)|[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Erstellen eines neuen [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekts.|
|[AndroidEasEmailProfileConfiguration löschen](../api/intune-deviceconfig-androideasemailprofileconfiguration-delete.md)|Keine|Löscht eine [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).|
|[AndroidEasEmailProfileConfiguration aktualisieren](../api/intune-deviceconfig-androideasemailprofileconfiguration-update.md)|[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Aktualisieren der Eigenschaften eines [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|accountName|Zeichenfolge|Exchange ActiveSync-Kontonamen, der den Benutzern als Name des EAS-Profils (dieses) angezeigt wird.|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Authentifizierungsmethode für Exchange ActiveSync. Mögliche Werte sind: `usernameAndPassword` und `certificate`.|
|syncCalendar|Boolean|Schaltet die Synchronisierung des Kalenders ein. Wenn der Wert auf false festgelegt ist, wird der Kalender auf dem Gerät deaktiviert.|
|syncContacts|Boolean|Schaltet die Synchronisierungs Kontakte ein. Bei Festlegung auf false sind Kontakte auf dem Gerät deaktiviert.|
|syncTasks|Boolean|Schaltet Synchronisierungsaufgaben um. Bei Festlegung auf false werden Aufgaben auf dem Gerät deaktiviert.|
|syncNotes|Boolean|Schaltet die Synchronisierungs Notizen ein. Wenn der Wert auf false festgelegt ist, werden die Notizen auf dem Gerät deaktiviert.|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|Uhrzeit, zu der e-Mails synchronisiert werden sollen. Mögliche Werte sind: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth` und `unlimited`.|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|E-Mail-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird. Mögliche Werte sind: `userPrincipalName` und `primarySmtpAddress`.|
|emailSyncSchedule|[emailSyncSchedule](../resources/intune-deviceconfig-emailsyncschedule.md)|Zeitplan für die e-Mail-Synchronisierung. Mögliche Werte sind: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes` und `basedOnMyUsage`.|
|hostName|String|Exchange-Speicherort (URL), mit dem die systemeigene Mail-App eine Verbindung herstellt.|
|requireSmime|Boolean|Gibt an, ob S/MIME-Zertifikat verwendet werden soll.|
|requireSsl|Boolean|Gibt an, ob SSL verwendet werden soll.|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|UserName-Attribut, das von AAD entnommen und vor der Installation auf dem Gerät in dieses Profil eingefügt wird. Mögliche Werte: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|UserDomainname-Attribut, das von AAD ausgewählt und vor der Installation auf dem Gerät in dieses Profil eingefügt wird. Mögliche Werte sind: `fullDomainName` und `netBiosDomainName`.|
|customDomainName|Zeichenfolge|Benutzerdefinierter Domänenname, der beim Generieren eines e-Mail-Profils verwendet wird, bevor es auf dem Gerät installiert wird.|

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
|identityCertificate|[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|Identitätszertifikat.|
|smimeSigningCertificate|[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|S/MIME-Signaturzertifikat.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidEasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
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
  "accountName": "String",
  "authenticationMethod": "String",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "emailSyncSchedule": "String",
  "hostName": "String",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String"
}
```




