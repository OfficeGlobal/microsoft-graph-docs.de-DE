---
title: windowsFirewallRule-Ressourcentyp
description: Eine Regel, die den Datenverkehr über die Windows-Firewall steuert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3753eeade1dce32e4332becd7575710a2f6ea1a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631539"
---
# <a name="windowsfirewallrule-resource-type"></a>windowsFirewallRule-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine Regel, die den Datenverkehr über die Windows-Firewall steuert.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Der Anzeigename der Regel. Muss nicht eindeutig sein.|
|description|Zeichenfolge|Die Beschreibung der Regel.|
|packageFamilyName|String|Der Name der paketfamilie einer Microsoft Store-Anwendung, die von der Firewallregel betroffen ist.|
|filePath|String|Der vollständige Dateipfad einer APP, die von der Firewallregel betroffen ist.|
|Wert Service Name|String|Der Name, der in Fällen verwendet wird, in denen ein Dienst, nicht eine Anwendung, Datenverkehr sendet oder empfängt.|
|Protokoll|Int32|0-255 Zahl, die das IP-Protokoll (TCP = 6, UDP = 17) darstellt. Wenn nicht angegeben, ist der Standardwert all. Gültige Werte 0 bis 255|
|localPortRanges|String collection|Liste der lokalen Portierungs Bereiche. Beispiel: "100-120", "200", "300-320". Wenn nicht angegeben, ist der Standardwert all.|
|remotePortRanges|String collection|Liste der Remote-Portierungs Bereiche. Beispiel: "100-120", "200", "300-320". Wenn nicht angegeben, ist der Standardwert all.|
|localAddressRanges|String collection|Liste der lokalen Adressen, die von der Regel abgedeckt werden. Gültige Token sind:
- "*" gibt eine beliebige lokale Adresse an. Falls vorhanden, muss es sich dabei um das einzige Token handeln, das enthalten ist.
- Ein Subnetz kann entweder mit der Subnetzmaske oder mit der Netzwerkpräfix Notation angegeben werden. Wenn weder eine Subnetzmaske noch ein Netzwerkpräfix angegeben wird, ist die Subnetzmaske standardmäßig 255.255.255.255.
- Eine gültige IPv6-Adresse.
- Ein IPv4-Adressbereich im Format "Start address-End Address" ohne Leerzeichen.
- Ein IPv6-Adressbereich im Format "Start address-End Address" ohne Leerzeichen.
Default ist eine beliebige Adresse. | | remoteAddressRanges | Zeichenfolgensammlung | Liste der Token, die die von der Regel abgedeckten Remoteadressen angeben. Bei Token wird die Groß-/Kleinschreibung nicht beachtet. Gültige Token sind:
- "*" gibt eine beliebige Remoteadresse an. Falls vorhanden, muss es sich dabei um das einzige Token handeln, das enthalten ist.
- DefaultGateway
- DHCP
- DNS
- GEWINNT
- "Intranet" (unter Windows-Versionen 1809 und höher)
- "RmtIntranet" (unter Windows-Versionen 1809 und höher)
- "Internet" (unter Windows-Versionen 1809 und höher)
- "Ply2Renders" (unter Windows-Versionen 1809 und höher)
- "LocalSubnet" gibt eine beliebige lokale Adresse im lokalen Subnetz an.
- Ein Subnetz kann entweder mit der Subnetzmaske oder mit der Netzwerkpräfix Notation angegeben werden. Wenn weder eine Subnetzmaske noch ein Netzwerkpräfix angegeben wird, ist die Subnetzmaske standardmäßig 255.255.255.255.
- Eine gültige IPv6-Adresse.
- Ein IPv4-Adressbereich im Format "Start address-End Address" ohne Leerzeichen.
- Ein IPv6-Adressbereich im Format "Start address-End Address" ohne Leerzeichen.
Default ist eine beliebige Adresse. | | profileTypes | [windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)| Gibt die Profile an, zu denen die Regel gehört. Wenn nicht angegeben, ist der Standardwert all. Mögliche Werte sind: `notConfigured`, `domain`, `private`, `public`. | | Aktion | [stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)| Die Aktion, die von der Regel erzwungen wird. Wenn nicht angegeben, ist der Standardwert zulässig. Mögliche Werte sind: `notConfigured`, `blocked`, `allowed`. | | trafficDirection | [windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)| Die datenverkehrsrichtung, für die die Regel aktiviert ist. Wenn nicht angegeben, ist der Standardwert out. Mögliche Werte sind: `notConfigured`, `out`, `in`. | | interfaceTypes | [windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)| Die Schnittstellentypen der Regel. Mögliche Werte sind: `notConfigured`, `remoteAccess`, `wireless`, `lan`. | | localUserAuthorizations | Zeichenfolge | Gibt die Liste der autorisierten lokalen Benutzer für den App-Container an. Dies ist eine Zeichenfolge im SDDL-Format (Security Descriptor Definition Language). |

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "localUserAuthorizations": "String"
}
```




