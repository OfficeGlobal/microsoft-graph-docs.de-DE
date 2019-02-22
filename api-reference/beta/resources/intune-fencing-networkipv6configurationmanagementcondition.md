---
title: networkIPv6ConfigurationManagementCondition-Ressourcentyp
description: Es können konfigurationsbasierte IPv6-Verwaltungsbedingungen definiert werden, die ausgelöst werden, wenn ein Gerät bestimmte IP-Netzwerkeinstellungen erkennt. Eine IP-Konfigurations Verwaltungsbedingung wird nur dann als TRUE betrachtet, wenn die Netzwerkverbindung aktiv ist. IPv6-DHCP-Serveradressen werden möglicherweise nicht abgeglichen. Dies liegt daran, dass Windows (circa Redstone) diese Informationen nicht für den natürlichen Authentifizierungsdienst verfügbar macht.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 132c61b9a3203cf1d04a2d2cbfc6a8d6a9e19552
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147775"
---
# <a name="networkipv6configurationmanagementcondition-resource-type"></a>networkIPv6ConfigurationManagementCondition-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Es können konfigurationsbasierte IPv6-Verwaltungsbedingungen definiert werden, die ausgelöst werden, wenn ein Gerät bestimmte IP-Netzwerkeinstellungen erkennt. Eine IP-Konfigurations Verwaltungsbedingung wird nur dann als TRUE betrachtet, wenn die Netzwerkverbindung aktiv ist.
IPv6-DHCP-Serveradressen werden möglicherweise nicht abgeglichen. Dies liegt daran, dass Windows (circa Redstone) diese Informationen nicht für den natürlichen Authentifizierungsdienst verfügbar macht.


Erbt von [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[NetworkIPv6ConfigurationManagementConditions aufListen](../api/intune-fencing-networkipv6configurationmanagementcondition-list.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekte.|
|[NetworkIPv6ConfigurationManagementCondition abrufen](../api/intune-fencing-networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Lesen von Eigenschaften und Beziehungen des [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.|
|[NetworkIPv6ConfigurationManagementCondition erstellen](../api/intune-fencing-networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Erstellen eines neuen [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.|
|[NetworkIPv6ConfigurationManagementCondition löschen](../api/intune-fencing-networkipv6configurationmanagementcondition-delete.md)|Keine|Löscht eine [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).|
|[NetworkIPv6ConfigurationManagementCondition aktualisieren](../api/intune-fencing-networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Aktualisieren der Eigenschaften eines [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutiger Bezeichner für die Verwaltungsbedingung. Vom System generierter Wert, der bei der Erstellung zugewiesen wird. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Zeichenfolge|Eindeutiger Name für die Verwaltungsbedingung. Wird in Verwaltungs Bedingungsausdrücken verwendet. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Zeichenfolge|Der Administrator definierte Name der Verwaltungsbedingung. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|Zeichenfolge|Die vom Administrator definierte Beschreibung der Verwaltungsbedingung. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Verwaltungsbedingung erstellt wurde. Generierte Dienstseite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Verwaltungsbedingung zuletzt geändert wurde. Aktualisierte Dienstseite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|Zeichenfolge|ETag der Verwaltungsbedingung. Aktualisierte Dienstseite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung|Die entsprechenden Plattformen für diese Verwaltungsbedingung. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|ipV6Prefix|Zeichenfolge|Das IPv6-Subnetz, mit dem eine Verbindung hergestellt werden soll. z. b. 2001: db8::/32|
|ipV6Gateway|Zeichenfolge|Die IPv6-Gateway-Adresse für. z. b. 2001: db8:: 1|
|ipV6DNSServerList|String collection|Ein für den Adapter konfigurierter IPv6-DNS-Server.|
|dnsSuffixList|String collection|Gültige DNS-Suffixe für das aktuelle Netzwerk. beispielsweise Seattle.contoso.com|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Sammlung|Die der Verwaltungsbedingung zugeordneten Verwaltungs Bedingungsanweisungen. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|

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




