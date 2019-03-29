---
title: EmbeddedSIMDeviceState aktualisieren
description: Aktualisieren der Eigenschaften eines embeddedSIMDeviceState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8307ebc185a6543b706befc433b7e26b17702b38
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981979"
---
# <a name="update-embeddedsimdevicestate"></a>EmbeddedSIMDeviceState aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekts.

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
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für den Status des eingebetteten SIM-Geräts. Vom System generierter Wert, der bei der Erstellung zugewiesen wird.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem der Status des eingebetteten SIM-Geräts erstellt wurde. Generierte Dienstseite.|
|modifiedDateTime|DateTimeOffset|Zeitpunkt, zu dem der Status des eingebetteten SIM-Geräts zuletzt geändert wurde. Aktualisierte Dienstseite.|
|lastSyncDateTime|DateTimeOffset|Zeitpunkt, zu dem das eingebettete SIM-Gerät zuletzt eingecheckt hat. Aktualisierte Dienstseite.|
|universalIntegratedCircuitCardIdentifier|String|Der universelle integrierte Leiterkarten Bezeichner (UICCID), der die Hardware identifiziert, auf der ein Profil bereitgestellt werden soll.|
|deviceName|String|Gerätename, für den das Abonnement vorgesehen wurde (z. b. DESKTOP-JOE)|
|userName|String|Benutzername, für den das Abonnement z. b. joe@contoso.com wurde|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|Der Status des auf das Gerät angewendeten Profil Vorgangs. Mögliche Werte: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|String|Beschreibung des Zustands der Einrichtung.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "908884a3-84a3-9088-a384-8890a3848890",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```




