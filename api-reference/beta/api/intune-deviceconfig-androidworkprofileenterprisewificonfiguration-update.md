---
title: AndroidWorkProfileEnterpriseWiFiConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines androidWorkProfileEnterpriseWiFiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5def1cb85d57c3d4a90fa573444b646f54d31117
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152332"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a>AndroidWorkProfileEnterpriseWiFiConfiguration aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) -Objekts.

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
Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)erforderlich sind.

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
|networkName|Zeichenfolge|Netzwerk Name geerbt von [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)|
|SSID|Zeichenfolge|Dies ist der Name des WLAN-Netzwerks, das auf alle Geräte übertragen wird. Geerbt von [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)|
|connectAutomatically|Boolescher Wert|Verbinden Sie sich automatisch, wenn sich dieses Netzwerk in Reichweite befindet. Wenn Sie diesen Wert auf true festlegen, wird die Benutzereingabe übersprungen, und das Gerät wird automatisch mit dem WLAN verbunden. Geerbt von [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolescher Wert|Wenn dieser Wert auf "true" festgelegt ist, wird das Gerät gezwungen, eine Verbindung mit einem Netzwerk herzustellen, das seine SSID nicht auf alle Geräte übermittelt. Geerbt von [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)|
|wiFiSecurityType|[androidWiFiSecurityType](../resources/intune-deviceconfig-androidwifisecuritytype.md)|Gibt an, ob der WLAN-Endpunkt einen EAP-basierten Sicherheitstyp verwendet. Von [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)geerbt. Mögliche Werte sind: `open` und `wpaEnterprise`.|
|eapType|[androidEapType](../resources/intune-deviceconfig-androideaptype.md)|Gibt den Typ des EAP-Protokolls an, das auf dem WLAN-Endpunkt (Router) festgelegt ist. Mögliche Werte sind: `eapTls`, `eapTtls` und `peap`.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Gibt die AuthentifizierungsMethode an, die der Client (Gerät) verwenden muss, wenn der EAP-Typ auf PEAP oder EAP-TTLS konfiguriert ist. Mögliche Werte sind: `certificate` und `usernameAndPassword`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Nicht-EAP-Methode für die Authentifizierung (innere Identität) bei EAP-TTLS und AuthenticationMethod ist username und Password. Mögliche Werte: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|Nicht-EAP-Methode für die Authentifizierung (innere Identität), wenn EAP-Typ PEAP und AuthenticationMethod der Benutzername und das Kennwort ist. Mögliche Werte sind: `none` und `microsoftChapVersionTwo`.|
|Outeridentityprivacytemporaryvalue wurden|Zeichenfolge|Aktivieren Sie Identitätsdatenschutz (äußere Identität), wenn der EAP-Typ für EAP-TTLS oder PEAP konfiguriert ist. Die hier angegebene Zeichenfolge wird verwendet, um den Benutzernamen einzelner Benutzer zu maskieren, wenn Sie versuchen, eine Verbindung mit dem WLAN herzustellen.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 776

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 948

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




