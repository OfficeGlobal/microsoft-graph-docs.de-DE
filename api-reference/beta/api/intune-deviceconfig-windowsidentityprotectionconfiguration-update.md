---
title: WindowsIdentityProtectionConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines windowsIdentityProtectionConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c12b12fd24298500b3e73eb5380ecc1d6844ee34
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972494"
---
# <a name="update-windowsidentityprotectionconfiguration"></a>WindowsIdentityProtectionConfiguration aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.

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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|useSecurityKeyForSignin|Boolescher Wert|Boolescher Wert, der zum Aktivieren des Windows Hello-Sicherheitsschlüssels als Anmeldeinformationen verwendet wird.|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Boolescher Wert|Boolescher Wert, mit dem Enhanced Anti-Spoofing für die Erkennung von gesichtsfunktionen unter Windows Hello Face Authentication aktiviert wird.|
|pinMinimumLength|Int32|Ganzzahliger Wert, der die Mindestanzahl von Zeichen für die Windows-Hello for Business-PIN festlegt. Gültige Werte sind 4 bis 127 inklusive und kleiner als oder gleich dem Wert, der für die maximale PIN festgelegt ist. Gültige Werte 4 bis 127|
|pinMaximumLength|Int32|Ganzzahliger Wert, der die maximale Anzahl der zulässigen Zeichen für die Arbeits-PIN festlegt. Gültige Werte sind 4 bis 127 inklusive und größer oder gleich dem Wert, der für die minimale PIN festgelegt ist. Gültige Werte 4 bis 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Dieser Wert konfiguriert die Verwendung von Großbuchstaben in der Windows Hello for Business-PIN. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Dieser Wert konfiguriert die Verwendung von Kleinbuchstaben in der Windows Hello for Business-PIN. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Steuert die Möglichkeit, Sonderzeichen in der Windows Hello for Business-PIN zu verwenden. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinExpirationInDays|Int32|Ganzzahliger Wert gibt den Zeitraum (in Tagen) an, an dem eine PIN verwendet werden kann, bevor das System den Benutzer zum Ändern benötigt. Gültige Werte sind 0 bis 730 inklusive. Gültige Werte: 0 bis 730.|
|pinPreviousBlockCount|Int32|Steuert, wie verhindert werden kann, dass Benutzer frühere PINs verwenden. Dieser muss zwischen 0 und 50 einschließlich festgelegt werden, und die aktuelle PIN des Benutzers ist in dieser Anzahl enthalten. Bei Festlegung auf 0 werden frühere PINs nicht gespeichert. Der PIN-Verlauf wird nicht durch eine PIN-Zurücksetzung beibehalten. Gültige Werte: 0 bis 50.|
|pinRecoveryEnabled|Boolescher Wert|Boolescher Wert, der es einem Benutzer ermöglicht, seine PIN mithilfe des Windows Hello for Business-PIN-Wiederherstellungs Diensts zu ändern.|
|securityDeviceRequired|Boolescher Wert|Steuert, ob ein Trusted Platform Module (TPM) für die Einrichtung von Windows Hello for Business erforderlich ist. Ein TPM bietet einen zusätzlichen Sicherheitsvorteil, da darin gespeicherte Daten nicht auf anderen Geräten verwendet werden können. Wenn dieser Wert auf false festgelegt ist, können alle Geräte Windows Hello for Business auch dann zur Verfügung stellen, wenn kein TPM verfügbar ist.|
|unlockWithBiometricsEnabled|Boolean|Steuert die Verwendung von biometrischen Gesten wie Gesicht und Fingerabdruck als Alternative zur Windows Hello for Business-PIN.  Wenn dieser Wert auf false festgelegt ist, sind biometrische Gesten nicht zulässig. Benutzer müssen bei Fehlern weiterhin eine PIN als Sicherung konfigurieren.|
|useCertificatesForOnPremisesAuthEnabled|Boolescher Wert|Boolescher Wert, der es Windows Hello for Business ermöglicht, Zertifikate zur Authentifizierung lokaler Ressourcen zu verwenden.|
|windowsHelloForBusinessBlocked|Boolean|Boolescher Wert, der Windows Hello for Business als Methode für die Anmeldung an Windows blockiert.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 810

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 982

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```




