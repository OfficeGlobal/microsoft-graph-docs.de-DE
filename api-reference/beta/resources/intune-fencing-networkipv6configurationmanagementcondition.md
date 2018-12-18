---
title: Ressourcentyp networkIPv6ConfigurationManagementCondition
description: Netzwerkeinstellungen für IPv6-Konfiguration-basiertes Management Bedingungen definiert werden können, die ausgelöst wird, wenn ein Gerät bestimmte IP-Adresse erkennt. Eine IP-Config-Management-Bedingung wird nur als TRUE betrachtet werden, wenn die Netzwerkverbindung aktiv ist.
author: tfitzmac
ms.openlocfilehash: de74fddad090993f6829180ba6f5eaea9cdaf59a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305740"
---
# <a name="networkipv6configurationmanagementcondition-resource-type"></a>Ressourcentyp networkIPv6ConfigurationManagementCondition

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Netzwerkeinstellungen für IPv6-Konfiguration-basiertes Management Bedingungen definiert werden können, die ausgelöst wird, wenn ein Gerät bestimmte IP-Adresse erkennt. Eine IP-Config-Management-Bedingung wird nur als TRUE betrachtet werden, wenn die Netzwerkverbindung aktiv ist.
IPv6-DHCP-Server-Adressen möglicherweise nicht abgeglichen wird. Dies ist, da diese Informationen, um den natürlichen Authentifizierungsdienst nicht in Windows (ca. Redstone) verfügbar macht.

Erbt vom [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste networkIPv6ConfigurationManagementConditions](../api/intune-fencing-networkipv6configurationmanagementcondition-list.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Auflistung|Listeneigenschaften und Beziehungen der [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekte.|
|[Abrufen von networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Lesen Sie Eigenschaften und Beziehungen des [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.|
|[Erstellen von networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Erstellen eines neuen [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.|
|[NetworkIPv6ConfigurationManagementCondition löschen](../api/intune-fencing-networkipv6configurationmanagementcondition-delete.md)|Keines|Löscht eine [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).|
|[NetworkIPv6ConfigurationManagementCondition aktualisieren](../api/intune-fencing-networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Aktualisieren Sie die Eigenschaften eines [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die Bedingung Management. System generierten Wert, die beim Erstellen zugewiesen. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|String|Eindeutiger Name für die Bedingung Management. In Management Bedingung Ausdrücken verwendet. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Der Administrator definierter Name der Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|String|Der Administrator definiert die Beschreibung der Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, an die Bedingung Management erstellt wurde. Generierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Die Zeit, die die Bedingung Management zuletzt geändert wurde. Aktualisierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag der Bedingung Management. Aktualisierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung|Die entsprechenden Plattformen für diese Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|ipV6Prefix|String|Die IPv6-Subnetz mit verbunden sein. Diese Vorgaben unter 2001:db8:: / 32|
|ipV6Gateway|String|Die IPv6-Gateway-Adresse zu. z. B. 2001:db8::1|
|ipV6DNSServerList|Collection von Objekten des Typs „String“|Eine IPv6-DNS-Server für den Adapter konfiguriert.|
|dnsSuffixList|Collection von Objekten des Typs „String“|Gültige DNS-Suffixe für das aktuelle Netzwerk. Diese Vorgaben unter seattle.contoso.com|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managementConditionStatements|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung|Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv6ConfigurationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "ipV6Prefix": "String",
  "ipV6Gateway": "String",
  "ipV6DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```





