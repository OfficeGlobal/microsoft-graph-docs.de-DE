---
title: NetworkIPv4ConfigurationManagementCondition aktualisieren
description: Aktualisieren Sie die Eigenschaften eines networkIPv4ConfigurationManagementCondition-Objekts.
author: tfitzmac
ms.openlocfilehash: 15ced5b6e4f92d25945ab76144e5a30438bb258f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317283"
---
# <a name="update-networkipv4configurationmanagementcondition"></a>NetworkIPv4ConfigurationManagementCondition aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisieren Sie die Eigenschaften eines [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts.
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
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a>Anforderungsheader
|Header|Wert|
|:---|:---|
|Autorisierung|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung für das Objekt [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) eine JSON-Darstellung.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die Bedingung Management. System generierten Wert, die beim Erstellen zugewiesen. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|String|Eindeutiger Name für die Bedingung Management. In Management Bedingung Ausdrücken verwendet. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Der Administrator definierter Name der Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|String|Der Administrator definiert die Beschreibung der Bedingung Management. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, an die Bedingung Management erstellt wurde. Generierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Die Zeit, die die Bedingung Management zuletzt geändert wurde. Aktualisierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag der Bedingung Management. Aktualisierte Service-Seite. Geerbt von [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung|Die entsprechenden Plattformen für diese Bedingung Management. Geerbt von [ManagementCondition](../resources/intune-fencing-managementcondition.md). Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.|
|ipV4Prefix|String|Das IPv4-Subnetz mit verbunden sein. Diese Vorgaben unter 10.0.0.0/8|
|ipV4Gateway|String|Das Gateway IPv4-Adresse. z. B. 10.0.0.0|
|ipV4DHCPServer|String|Die IPv4-Adresse des DHCP-Servers für den Adapter.|
|ipV4DNSServerList|Collection von Objekten des Typs „String“|Die IPv4-DNS-Server für den Adapter konfiguriert.|
|dnsSuffixList|Collection von Objekten des Typs „String“|Gültige DNS-Suffixe für das aktuelle Netzwerk. Diese Vorgaben unter seattle.contoso.com|



## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 447

{
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```





