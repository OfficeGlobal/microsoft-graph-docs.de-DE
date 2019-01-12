---
title: Ressourcentyp networkIPv4ConfigurationManagementCondition
description: Netzwerkeinstellungen für IPv4-Konfiguration-basiertes Management Bedingungen definiert werden können, die ausgelöst wird, wenn ein Gerät bestimmte IP-Adresse erkennt. Eine IP-Config Management Bedingungen werden nur als TRUE betrachtet werden, wenn die Netzwerkverbindung aktiv ist.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 412f5de452e23eeb58f536655c4678526e996e07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962107"
---
# <a name="networkipv4configurationmanagementcondition-resource-type"></a>Ressourcentyp networkIPv4ConfigurationManagementCondition

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Netzwerkeinstellungen für IPv4-Konfiguration-basiertes Management Bedingungen definiert werden können, die ausgelöst wird, wenn ein Gerät bestimmte IP-Adresse erkennt. Eine IP-Config Management Bedingungen werden nur als TRUE betrachtet werden, wenn die Netzwerkverbindung aktiv ist.

Erbt vom [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste networkIPv4ConfigurationManagementConditions](../api/intune-fencing-networkipv4configurationmanagementcondition-list.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Auflistung|Listeneigenschaften und Beziehungen der [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekte.|
|[Abrufen von networkIPv4ConfigurationManagementCondition](../api/intune-fencing-networkipv4configurationmanagementcondition-get.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|Lesen Sie Eigenschaften und Beziehungen des [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts.|
|[Erstellen von networkIPv4ConfigurationManagementCondition](../api/intune-fencing-networkipv4configurationmanagementcondition-create.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|Erstellen eines neuen [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts.|
|[NetworkIPv4ConfigurationManagementCondition löschen](../api/intune-fencing-networkipv4configurationmanagementcondition-delete.md)|Keine|Löscht eine [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).|
|[NetworkIPv4ConfigurationManagementCondition aktualisieren](../api/intune-fencing-networkipv4configurationmanagementcondition-update.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|Aktualisieren Sie die Eigenschaften eines [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts.|

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
|ipV4Prefix|Zeichenfolge|Das IPv4-Subnetz mit verbunden sein. Diese Vorgaben unter 10.0.0.0/8|
|ipV4Gateway|Zeichenfolge|Das Gateway IPv4-Adresse. z. B. 10.0.0.0|
|ipV4DHCPServer|Zeichenfolge|Die IPv4-Adresse des DHCP-Servers für den Adapter.|
|ipV4DNSServerList|Collection von Objekten des Typs „String“|Die IPv4-DNS-Server für den Adapter konfiguriert.|
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
  "@odata.type": "microsoft.graph.networkIPv4ConfigurationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
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
  "ipV4Prefix": "String",
  "ipV4Gateway": "String",
  "ipV4DHCPServer": "String",
  "ipV4DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```





