---
title: windows10CompliancePolicy aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4d24c0d964fd43e12c4fcd9a3ff91a0bcd1238b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172268"
---
# <a name="update-windows10compliancepolicy"></a>windows10CompliancePolicy aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisiert die Eigenschaften von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

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
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekts an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|id|string|Schlüssel der Entität Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|passwordRequired|Boolescher Wert|Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.|
|passwordBlockSimple|Boolescher Wert|Gibt an, ob einfache Kennwörter erlaubt sind.|
|passwordRequiredToUnlockFromIdle|Boolean|Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.|
|passwordMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird|
|passwordExpirationDays|Int32|Zeitraum in Tagen bis zum Ablaufen des Kennworts|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.|
|requireHealthyDeviceReport|Boolean|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.|
|osMinimumVersion|Zeichenfolge|Mindestversion von Windows 10|
|osMaximumVersion|Zeichenfolge|Maximalversion von Windows 10|
|mobileOsMinimumVersion|Zeichenfolge|Mindestversion von Windows Phone|
|mobileOsMaximumVersion|Zeichenfolge|Maximalversion von Windows Phone|
|earlyLaunchAntiMalwareDriverEnabled|Boolescher Wert|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.|
|bitLockerEnabled|Boolescher Wert|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.|
|secureBootEnabled|Boolescher Wert|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.|
|codeIntegrityEnabled|Boolean|Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.|
|storageRequireEncryption|Boolean|Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.|
|activeFirewallRequired|Boolescher Wert|Aktive Firewall auf Windows-Geräten erforderlich.|
|defenderEnabled|Boolescher Wert|Windows Defender-Antischadsoftware auf Windows-Geräten erforderlich.|
|defenderVersion|Zeichenfolge|Mindestversion von Windows Defender Antischadsoftware auf Windows-Geräten|
|signatureOutOfDate|Boolescher Wert|Windows Defender-Antischadsoftware-Signatur muss auf Windows-Geräten auf dem neuesten Stand sein.|
|rtpEnabled|Boolescher Wert|Windows Defender-Antischadsoftware-Echtzeitschutz auf Windows-Geräten erforderlich.|
|antivirusRequired|Boolescher Wert|Erfordern Sie eine Antivirus-Lösung, die mit Windows Decurity Center registriert ist, um ein-und zu überwachen (beispielsweise Symantec, Windows Defender).|
|antiSpywareRequired|Boolescher Wert|Fordern Sie eine beliebige antiSpywarelösung an, die mit Windows Decurity Center registriert ist, um eingeschaltet und überwacht zu werden (z. b. Symantec, Windows Defender).|
|validOperatingSystemBuildRanges|[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) -Sammlung|Die gültigen buildbereiche des Betriebssystems auf Windows-Geräten. Diese Collection darf maximal 10.000 Elemente enthalten.|
|deviceThreatProtectionEnabled|Boolescher Wert|Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Mindestrisiko für Geräte Bedrohungsstufe zum Melden der Nichtkonformität. Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.|
|configurationManagerComplianceRequired|Boolescher Wert|Beachten Sie, dass der SCCM-Konformitätsstatus für den InTune-KonformitätsStatus berücksichtigt werden muss.|



## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1666

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1838

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true
}
```




