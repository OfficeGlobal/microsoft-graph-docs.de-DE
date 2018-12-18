---
title: Ressourcentyp windows10VpnConfiguration
description: Durch die Konfigurationen in dieses Profil bereitstellen können Sie das Windows-10-Gerät (desktop oder mobilen) zur gewünschten Endpunkt für VPN-Verbindung anweisen. Durch Angeben von erwartet die Authentifizierungstypen-Methode und der Sicherheit durch VPN-Endpunkt, dass Sie die VPN-Verbindung nahtlos für Endbenutzer vornehmen können.
author: tfitzmac
ms.openlocfilehash: 1dbbdb5a7065214ab6a290215f2c6016f8ad74bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340698"
---
# <a name="windows10vpnconfiguration-resource-type"></a>Ressourcentyp windows10VpnConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Durch die Konfigurationen in dieses Profil bereitstellen können Sie das Windows-10-Gerät (desktop oder mobilen) zur gewünschten Endpunkt für VPN-Verbindung anweisen. Durch Angeben von erwartet die Authentifizierungstypen-Methode und der Sicherheit durch VPN-Endpunkt, dass Sie die VPN-Verbindung nahtlos für Endbenutzer vornehmen können.

Erbt vom [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windows10VpnConfigurations](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekte.|
|[Abrufen von windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.|
|[Erstellen von windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Erstellen eines neuen [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.|
|[Windows10VpnConfiguration löschen](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|Keines|Löscht eine [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).|
|[Windows10VpnConfiguration aktualisieren](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
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
|connectionName|String|Name der Verbindung für den Benutzer angezeigt. Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|Server|[VpnServer](../resources/intune-deviceconfig-vpnserver.md) -Auflistung|Liste der VPN-Server im Netzwerk. Stellen Sie sicher, dass Endbenutzer diese Netzwerkadressen zugreifen können. Diese Collection darf maximal 500 Elemente enthalten. Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|customXml|Binär|Benutzerdefinierte XML-Befehle, die die VPN-Verbindung konfiguriert. (UTF8 codiert Bytearray) Geerbt von [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|profileTarget|[windows10VpnProfileTarget](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|Profil Zieltyp. Mögliche Werte sind: `user`, `device` und `autoPilotDevice`.|
|connectionType|[windows10VpnConnectionType](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|Verbindungstyp. Mögliche Werte: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.|
|enableSplitTunneling|Boolesch|Split-tunneling zu aktivieren.|
|enableAlwaysOn|Boolesch|Aktivieren Sie Always On-Modus.|
|enableDeviceTunnel|Boolesch|Aktivieren Sie Gerät Tunnel.|
|enableDnsRegistration|Boolesch|Aktivieren Sie die IP-Adressregistrierung mit internen DNS.|
|dnsSuffixes|Collection von Objekten des Typs „String“|Geben Sie die DNS-Suffixe hinzufügen zu DNS-Suchliste Kurznamen ordnungsgemäß weitergeleitet.|
|authenticationMethod|[windows10VpnAuthenticationMethod](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|Authentifizierungsmethode. Mögliche Werte sind: `certificate`, `usernameAndPassword` und `customEapXml`.|
|rememberUserCredentials|Boolesch|Beachten Sie die Anmeldeinformationen des Benutzers.|
|enableConditionalAccess|Boolesch|Aktivieren Sie bedingte Zugriff.|
|enableSingleSignOnWithAlternateCertificate|Boolesch|Aktivieren Sie einmaliges Anmelden (SSO) mit anderen Zertifikats.|
|singleSignOnEku|[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)|Einmaliges Anmelden erweiterte Schlüsselverwendung (EKU).|
|singleSignOnIssuerHash|String|Einmaliges Anmelden Aussteller Hash.|
|eapXml|Binär|Extensible Authentication-Protokoll (EAP) XML. (UTF8-codiertes Bytearray)|
|proxyServer|[windows10VpnProxyServer](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|Proxy-Server.|
|associatedApps|[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) -Auflistung|Zugehörige Apps. Diese Collection darf maximal 10.000 Elemente enthalten.|
|onlyAssociatedAppsCanUseConnection|Boolesch|Nur zugeordnete Apps können Verbindung (pro app VPN) verwenden.|
|windowsInformationProtectionDomain|String|Windows Informationen Schutz (WIP) Domäne, die diese Verbindung zugeordnet.|
|trafficRules|[VpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) -Auflistung|Datenverkehr Regeln. Diese Sammlung kann bis zu 1000 Elemente enthalten.|
|Routen|[VpnRoute](../resources/intune-deviceconfig-vpnroute.md) -Auflistung|Routen (optional für Drittanbieter-Anbieter). Diese Sammlung kann bis zu 1000 Elemente enthalten.|
|dnsRules|[VpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) -Auflistung|DNS-Regeln. Diese Sammlung kann bis zu 1000 Elemente enthalten.|

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
|identityCertificate|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Identity-Zertifikat für die Clientauthentifizierung beim Authentifizierungsmethode Zertifikat ist.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "connectionName": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary",
  "profileTarget": "String",
  "connectionType": "String",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "String"
  ],
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "String",
    "objectIdentifier": "String"
  },
  "singleSignOnIssuerHash": "String",
  "eapXml": "binary",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "String",
      "identifier": "String"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "String",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "String",
      "protocols": 1024,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "appId": "String",
      "appType": "String",
      "routingPolicyType": "String",
      "claims": "String"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "String",
      "prefixSize": 1024
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "String",
      "servers": [
        "String"
      ],
      "proxyServerUri": "String"
    }
  ]
}
```





