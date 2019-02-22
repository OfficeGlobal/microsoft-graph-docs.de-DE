---
title: ImportedDeviceIdentity erstellen
description: Erstellen eines neuen importedDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb0f95f2d459b1b1583b2bdf9cc18f40ff9e03d5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154670"
---
# <a name="create-importeddeviceidentity"></a>ImportedDeviceIdentity erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

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
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das importedDeviceIdentity-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der importedDeviceIdentity erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|ID der importierten Geräte Identität|
|importedDeviceIdentifier|Zeichenfolge|Importierter Gerätebezeichner|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Typ der importierten Geräte Identität. Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Datum der letzten Änderung der Beschreibung|
|createdDateTime|DateTimeOffset|ErstellungsDatum des Geräts|
|lastContactedDateTime|DateTimeOffset|Datum der letzten Kontaktaufnahme des Geräts|
|description|Zeichenfolge|Die Beschreibung des Geräts|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Der Status des Geräts in InTune. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|Plattform|[Plattform](../resources/intune-enrollment-platform.md)|Die Plattform des Geräts. Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 332

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```




