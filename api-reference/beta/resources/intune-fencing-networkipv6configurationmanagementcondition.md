---
title: Ressourcentyp networkIPv6ConfigurationManagementCondition
description: Netzwerkeinstellungen für IPv6-Konfiguration-basiertes Management Bedingungen definiert werden können, die ausgelöst wird, wenn ein Gerät bestimmte IP-Adresse erkennt. Eine IP-Config-Management-Bedingung wird nur als TRUE betrachtet werden, wenn die Netzwerkverbindung aktiv ist. IPv6-DHCP-Server-Adressen möglicherweise nicht abgeglichen wird. Dies ist, da diese Informationen, um den natürlichen Authentifizierungsdienst nicht in Windows (ca. Redstone) verfügbar macht.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 497e5ec8d2fbde5a4687b6f30afef9383f2a890b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421193"
---
# <a name="networkipv6configurationmanagementcondition-resource-type"></a>Ressourcentyp networkIPv6ConfigurationManagementCondition

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Netzwerkeinstellungen für IPv6-Konfiguration-basiertes Management Bedingungen definiert werden können, die ausgelöst wird, wenn ein Gerät bestimmte IP-Adresse erkennt. Eine IP-Config-Management-Bedingung wird nur als TRUE betrachtet werden, wenn die Netzwerkverbindung aktiv ist.
IPv6-DHCP-Server-Adressen möglicherweise nicht abgeglichen wird. Dies ist, da diese Informationen, um den natürlichen Authentifizierungsdienst nicht in Windows (ca. Redstone) verfügbar macht.


Erbt vom [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste networkIPv6ConfigurationManagementConditions](../api/intune-fencing-networkipv6configurationmanagementcondition-list.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Auflistung|Listeneigenschaften und Beziehungen der [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekte.|
|[Abrufen von networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Lesen Sie Eigenschaften und Beziehungen des [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.|
|[Erstellen von networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Erstellen eines neuen [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.|
|[NetworkIPv6ConfigurationManagementCondition löschen](../api/intune-fencing-networkipv6configurationmanagementcondition-delete.md)|Keine|Löscht eine [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).|
|[NetworkIPv6ConfigurationManagementCondition aktualisieren](../api/intune-fencing-networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Aktualisieren Sie die Eigenschaften eines [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für die Bedingung Management. System generierten Wert, die beim Erstellen zugewiesen. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Zeichenfolge|Eindeutiger Name für die Bedingung Management. In Management Bedingung Ausdrücken verwendet. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Zeichenfolge|Der Administrator definierter Name der Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|Zeichenfolge|Der Administrator definiert die Beschreibung der Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, an die Bedingung Management erstellt wurde. Generierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Die Zeit, die die Bedingung Management zuletzt geändert wurde. Aktualisierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|Zeichenfolge|ETag der Bedingung Management. Aktualisierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung|Die entsprechenden Plattformen für diese Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|ipV6Prefix|Zeichenfolge|Die IPv6-Subnetz mit verbunden sein. Diese Vorgaben unter 2001:db8:: / 32|
|ipV6Gateway|Zeichenfolge|Die IPv6-Gateway-Adresse zu. z. B. 2001:db8::1|
|ipV6DNSServerList|Zeichenfolgenauflistung|Eine IPv6-DNS-Server für den Adapter konfiguriert.|
|dnsSuffixList|Zeichenfolgenauflistung|Gültige DNS-Suffixe für das aktuelle Netzwerk. Diese Vorgaben unter seattle.contoso.com|

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




