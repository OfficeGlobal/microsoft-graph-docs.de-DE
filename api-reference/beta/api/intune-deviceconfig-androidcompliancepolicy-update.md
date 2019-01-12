---
title: Aktualisieren von „androidCompliancePolicy“
description: Aktualisieren der Eigenschaften eines androidCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 05519bbf449199104120f62201f762656f103d09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951901"
---
# <a name="update-androidcompliancepolicy"></a>Aktualisieren von „androidCompliancePolicy“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisieren der Eigenschaften eines [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)-Objekts.
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
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a>Anforderungsheader
|Header|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON Darstellung für das [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|passwordRequired|Boolescher Wert|Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts. Gültige Werte: 4 bis 16.|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|Typ der Zeichen in Kennwort. Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.|
|passwordMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts Gültige Werte: 1 bis 65535.|
|passwordPreviousPasswordBlockCount|Int32|Legt fest, wie viele der zuletzt verwendeten Kennwörter nicht erneut verwendet werden dürfen.|
|securityPreventInstallAppsFromUnknownSources|Boolescher Wert|Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.|
|securityDisableUsbDebugging|Boolescher Wert|Deaktiviert das USB-Debuggen auf Android-Geräten.|
|securityRequireVerifyApps|Boolescher Wert|Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.|
|deviceThreatProtectionEnabled|Boolescher Wert|Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll. Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.|
|securityBlockJailbrokenDevices|Boolescher Wert|Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.|
|osMinimumVersion|Zeichenfolge|Mindestversion von Android|
|osMaximumVersion|Zeichenfolge|Maximalversion von Android|
|minAndroidSecurityPatchLevel|Zeichenfolge|Mindestens geforderter Sicherheitspatchlevel von Android|
|storageRequireEncryption|Boolescher Wert|Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.|
|securityRequireSafetyNetAttestationBasicIntegrity|Boolescher Wert|Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.|
|securityRequireSafetyNetAttestationCertifiedDevice|Boolescher Wert|Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.|
|securityRequireGooglePlayServices|Boolescher Wert|Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.|
|securityRequireUpToDateSecurityProviders|Boolescher Wert|Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen. Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.|
|securityRequireCompanyPortalAppIntegrity|Boolescher Wert|Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.|
|conditionStatementId|Zeichenfolge|Id des Condition-Anweisung.|
|restrictedApps|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Benötigen Sie das Gerät nicht die angegebenen apps installiert haben. Diese Collection darf maximal 10.000 Elemente enthalten.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)-Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1535

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1705

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```





