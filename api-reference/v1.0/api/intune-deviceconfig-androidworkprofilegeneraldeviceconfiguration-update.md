---
title: AndroidWorkProfileGeneralDeviceConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidWorkProfileGeneralDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7568bd59aa728391779dda6ee24a5e15d5c165ea
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971024"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a>AndroidWorkProfileGeneralDeviceConfiguration aktualisieren

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementConfiguration.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|passwordBlockFingerprintUnlock|Boolescher Wert|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|
|passwordBlockTrustAgents|Boolean|Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts. Gültige Werte: 1 bis 365.|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird. Gültige Werte 1 bis 16|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|Typ der zulässigen Datenfreigabe. Mögliche Werte sind: `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.|
|workProfileBlockNotificationsWhileDeviceLocked|Boolescher Wert|Gibt an, ob Benachrichtigungen blockiert werden sollen, während das Gerät gesperrt ist.|
|workProfileBlockAddingAccounts|Boolescher Wert|Verhindern, dass Benutzerkonten im Arbeitsprofil hinzufügen/entfernen.|
|workProfileBluetoothEnableContactSharing|Boolescher Wert|Bluetooth-Geräte können auf Enterprise-Kontakte zugreifen.|
|workProfileBlockScreenCapture|Boolescher Wert|Blockieren der Bildschirmaufzeichnung im Arbeitsprofil.|
|workProfileBlockCrossProfileCallerId|Boolescher Wert|Blockieren der Anzeige von Arbeitsprofil-Anrufer-ID im persönlichen Profil.|
|workProfileBlockCamera|Boolescher Wert|Arbeitsprofil Kamera blockieren.|
|workProfileBlockCrossProfileContactsSearch|Boolescher Wert|Blockieren der Verfügbarkeit von Arbeitsprofil Kontakten im persönlichen Profil|
|workProfileBlockCrossProfileCopyPaste|Boolescher Wert|Boolescher Wert, der angibt, ob die Einstellung Cross profile Copy/Paste nicht zulassen aktiviert ist.|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.|
|Eigenschaften workprofilepasswordblockfingerprintunlock|Boolescher Wert|Gibt an, ob die Fingerabdruck Sperre für das Arbeitsprofil blockiert werden soll.|
|workProfilePasswordBlockTrustAgents|Boolescher Wert|Gibt an, ob die Smart Lock-und andere Trust-Agents für das Arbeitsprofil blockiert werden sollen.|
|workProfilePasswordExpirationDays|Int32|Anzahl der Tage vor Ablauf des Arbeitsprofil Kennworts. Gültige Werte: 1 bis 365.|
|workProfilePasswordMinimumLength|Int32|Minimale Länge des Arbeitsprofil Kennworts. Gültige Werte: 4 bis 16.|
|workProfilePasswordMinNumericCharacters|Int32|Minimale Anzahl von numerischen Zeichen, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinNonLetterCharacters|Int32|Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinLetterCharacters|Int32|Mindestanzahl von Buchstaben, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|Minimale Anzahl von Kleinbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|Minimale Anzahl von Großbuchstaben, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinSymbolCharacters|Int32|Minimale Anzahl von Symbolen, die im Arbeitsprofil Kennwort erforderlich sind. Gültige Werte 1 bis 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.|
|workProfilePasswordPreviousPasswordBlockCount|Int32|Anzahl der vorherigen Arbeitsprofil Kennwörter, die blockiert werden sollen. Gültige Werte: 0 bis 24.|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Anzahl der zulässigen Anmeldefehler vor dem Entfernen des Arbeitsprofils und aller gelöschten Unternehmensdaten. Gültige Werte 1 bis 16|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Typ des erforderlichen Arbeitsprofil Kennworts. Mögliche Werte: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|Workprofilerequirepassword wurden|Boolescher Wert|Kennwort ist erforderlich oder nicht für das Arbeitsprofil|
|securityRequireVerifyApps|Boolean|Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```



