---
title: androidWorkProfileVpnConfiguration-Ressourcentyp
description: Durch die Bereitstellung der Konfigurationen in diesem Profil können Sie das Android-Arbeitsprofil Gerät anweisen, eine Verbindung mit dem gewünschten VPN-Endpunkt herzustellen. Durch Angeben der Authentifizierungsmethode und der vom VPN-Endpunkt erwarteten Sicherheitstypen können Sie die VPN-Verbindung für Endbenutzer nahtlos ausführen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1457d63266d05fbd3d5d70ba8f7ae94eb9f46d10
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150218"
---
# <a name="androidworkprofilevpnconfiguration-resource-type"></a>androidWorkProfileVpnConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Durch die Bereitstellung der Konfigurationen in diesem Profil können Sie das Android-Arbeitsprofil Gerät anweisen, eine Verbindung mit dem gewünschten VPN-Endpunkt herzustellen. Durch Angeben der Authentifizierungsmethode und der vom VPN-Endpunkt erwarteten Sicherheitstypen können Sie die VPN-Verbindung für Endbenutzer nahtlos ausführen.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AndroidWorkProfileVpnConfigurations aufListen](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-list.md)|[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekte.|
|[AndroidWorkProfileVpnConfiguration abrufen](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-get.md)|[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekts.|
|[AndroidWorkProfileVpnConfiguration erstellen](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-create.md)|[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)|Erstellen eines neuen [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekts.|
|[AndroidWorkProfileVpnConfiguration löschen](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-delete.md)|Keine|Löscht eine [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).|
|[AndroidWorkProfileVpnConfiguration aktualisieren](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-update.md)|[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)|Aktualisieren der Eigenschaften eines [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekts.|

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
|connectionName|Zeichenfolge|Dem Benutzer angezeigter Verbindungsname.|
|connectionType|[androidWorkProfileVpnConnectionType](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|Verbindungstyp. Mögliche Werte sind: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix` und `paloAltoGlobalProtect`.|
|role|Zeichenfolge|Role, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.|
|Bereich|Zeichenfolge|Bereich, wenn der Verbindungstyp auf Pulse Secure festgelegt ist.|
|Server|[vpnServer](../resources/intune-deviceconfig-vpnserver.md) -Sammlung|Liste der VPN-Server im Netzwerk. Stellen Sie sicher, dass Endbenutzer auf diese Netzwerkspeicherorte zugreifen können. Diese Collection darf maximal 500 Elemente enthalten.|
|Fingerabdruck|Zeichenfolge|Fingerabdruck ist eine Zeichenfolge, die verwendet wird, um zu überprüfen, ob der VPN-Server vertrauenswürdig ist, was nur beim Verbindungstyp Check Point Capsule VPN gilt.|
|customData|[keyValue](../resources/intune-deviceconfig-keyvalue.md)-Sammlung|Benutzerdefinierte Daten, wenn der Verbindungstyp auf Citrix festgelegt ist. Diese Auflistung kann maximal 25 Elemente enthalten.|
|customKeyValueData|[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung|Benutzerdefinierte Daten, wenn der Verbindungstyp auf Citrix festgelegt ist. Diese Auflistung kann maximal 25 Elemente enthalten.|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Authentifizierungsmethode. Mögliche Werte: `certificate`, `usernameAndPassword`.|

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
|identityCertificate|[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)|Identitätszertifikat für die Clientauthentifizierung, wenn die Authentifizierungsmethode das Zertifikat ist.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
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
  "connectionType": "String",
  "role": "String",
  "realm": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "String",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "authenticationMethod": "String"
}
```




