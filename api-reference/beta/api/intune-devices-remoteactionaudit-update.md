---
title: Remote Action Audit aktualisieren
description: Aktualisieren der Eigenschaften eines Remote Action Audit-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6105145c9e284c1f522c85f6a1237dcb2320fa28
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170224"
---
# <a name="update-remoteactionaudit"></a>Remote Action Audit aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Berichts-ID.|
|deviceDisplayName|Zeichenfolge|InTune-Gerätename.|
|userName|Zeichenfolge|\[veraltet verwenden\] Sie stattdessen Eigenschaften initiatedbyuserprincipalname.|
|Eigenschaften initiatedbyuserprincipalname|Zeichenfolge|Benutzer, der die Geräte Aktion initiiert hat, Format ist UPN.|
|Aktion|[Remote-Steuerung](../resources/intune-devices-remoteaction.md)|Der Name der Aktion. Mögliche Werte sind: `unknown`, `factoryReset`, `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures`,,,,,,,, `factoryResetKeepEnrollmentData`,, `shutDown` ,,,,,, `updateDeviceAccount` `automaticRedeployment` `locateDevice` .|
|requestDateTime|DateTimeOffset|Zeitpunkt der Ausgabe der Aktion in UTC.|
|deviceOwnerUserPrincipalName|Zeichenfolge|UPN des Geräte Besitzers.|
|deviceIMEI|Zeichenfolge|IMEI des Geräts.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Aktionsstatus. Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [Remote Action Audit](../resources/intune-devices-remoteactionaudit.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```




