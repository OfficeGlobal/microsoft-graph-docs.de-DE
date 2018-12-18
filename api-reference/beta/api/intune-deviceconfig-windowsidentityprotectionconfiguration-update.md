---
title: WindowsIdentityProtectionConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsIdentityProtectionConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 4131672de21560311ee1c2c1f8c1eb930a3de255
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326894"
---
# <a name="update-windowsidentityprotectionconfiguration"></a>WindowsIdentityProtectionConfiguration aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisieren Sie die Eigenschaften eines [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.
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
|Header|Wert|
|:---|:---|
|Autorisierung|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung für das Objekt [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) eine JSON-Darstellung.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolesch|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Boolesch|Boolescher Wert verwendet, um erweiterte Anti-spoofing für die Spracherkennung auf Windows Hello Gesicht Authentifizierung Gesichtsausdruck Feature aktivieren.|
|pinMinimumLength|Int32|Integer-Wert, der die Mindestanzahl der Zeichen für den Windows Hello für Business PIN benötigt wird. Gültige Werte sind 4 bis 127 und kleiner als oder gleich dem Wert für die maximale PIN festlegen. Gültige Werte 4 bis 127|
|pinMaximumLength|Int32|Integer-Wert, der die maximale Anzahl der zulässigen Zeichen für die Arbeit PIN festlegt. Gültige Werte sind 4 bis 127 inklusive und größer als oder gleich dem Wert für die minimale PIN festlegen. Gültige Werte 4 bis 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Dieser Wert konfiguriert die Verwendung von Großbuchstaben in der Windows Hello für Business PIN ein. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Dieser Wert konfiguriert die Verwendung von Kleinbuchstaben in der Windows Hello für Business PIN ein. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Steuert die Möglichkeit, Sonderzeichen in der Windows Hello für Business PIN verwenden. Mögliche Werte sind: `blocked`, `required` und `allowed`.|
|pinExpirationInDays|Int32|Integer-Wert gibt den Zeitraum (in Tagen) an, dass eine PIN-Nummer verwendet werden kann, bevor das System den Benutzer es ändern müssen. Gültige Werte sind 0, 730. Gültige Werte: 0 bis 730.|
|pinPreviousBlockCount|Int32|Steuert die Möglichkeit, zu verhindern, dass Benutzer die ältere PINs verwenden. Dies muss zwischen 0 und 50, einschließlich festgelegt werden, und die aktuelle PIN des Benutzers in diese Zählung eingeschlossen ist. Wenn auf 0 gesetzt, vorherigen PINs nicht gespeichert werden. PIN-Verlauf wird nicht beibehalten, über eine PIN zurücksetzen. Gültige Werte: 0 bis 50.|
|pinRecoveryEnabled|Boolesch|Boolescher Wert, mit der einen Benutzer seine PIN mithilfe der Windows Hello für Recovery-Service Business PIN ändern kann.|
|securityDeviceRequired|Boolescher Wert|Steuert, ob ein vertrauenswürdiger Platform-Modul (TPM) für die Bereitstellung von Windows Hello für Unternehmen erforderlich ist. Ein TPM bietet einen zusätzliche Sicherheit-Vorteil, dass darauf gespeicherte Daten auf anderen Geräten verwendet werden können. Wenn auf False festgelegt, alle Geräte Windows Hello für Unternehmen bereitstellen können, auch wenn ein verwendbar TPM nicht vorhanden ist.|
|unlockWithBiometricsEnabled|Boolescher Wert|Steuert die Verwendung von biometrische Gesten, wie das Standardsymbol zurück und Fingerabdruck, als Alternative zu den Windows Hello für Business PIN an.  Wenn es sich bei Festlegung auf "false", biometrische Gesten nicht zulässig sind. Benutzer müssen eine PIN weiterhin als Sicherungskopie bei Fehlern konfigurieren.|
|useCertificatesForOnPremisesAuthEnabled|Boolesch|Boolescher Wert, mit der Windows Hello für Unternehmen von Zertifikaten auf Standortbasierte Ressourcen authentifizieren kann.|
|windowsHelloForBusinessBlocked|Boolescher Wert|Boolescher Wert, der Windows Hello für Unternehmen als Methode für die Anmeldung bei Windows blockiert.|



## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 761

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
Content-Length: 946

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





