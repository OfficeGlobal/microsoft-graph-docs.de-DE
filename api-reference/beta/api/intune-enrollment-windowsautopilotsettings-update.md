---
title: WindowsAutopilotSettings aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsAutopilotSettings-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8087ce2a3d7fd02eb6cc118d75082382bcddd58d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877651"
---
# <a name="update-windowsautopilotsettings"></a>WindowsAutopilotSettings aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisieren Sie die Eigenschaften eines [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung für das Objekt [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) eine JSON-Darstellung.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|GUID des Objekts|
|lastSyncDateTime|DateTimeOffset|Zuletzt Daten synchronisieren Datum-Uhrzeit mit DDS-Dienst.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Zuletzt Daten synchronisieren Datum-Uhrzeit mit DDS-Dienst.|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Gibt den Status der Synchronisierung mit Gerät Daten Synchronisierungsdiensts (DDS). Mögliche Werte sind: `unknown`, `inProgress`, `completed` und `failed`.|



## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 167

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "08c16770-6770-08c1-7067-c1087067c108",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```





