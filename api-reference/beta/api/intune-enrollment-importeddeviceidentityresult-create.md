---
title: ImportedDeviceIdentityResult erstellen
description: Erstellen eines neuen importedDeviceIdentityResult-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa58ab82f0e86b9ad83b0fd1759886ae3ddfda09
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965886"
---
# <a name="create-importeddeviceidentityresult"></a>ImportedDeviceIdentityResult erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekts.

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
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das importedDeviceIdentityResult-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der importedDeviceIdentityResult erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|ID der von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten importierten Geräte Identität|
|importedDeviceIdentifier|String|Von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbte importierte Gerätebezeichner|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Typ der importierten Geräte Identität, die von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt wurde. Mögliche Werte sind: `unknown`, `imei` und `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Datum der letzten Änderung der von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Beschreibung|
|createdDateTime|DateTimeOffset|ErstellungsDatum des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts|
|lastContactedDateTime|DateTimeOffset|Datum der letzten Kontaktaufnahme des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts|
|description|Zeichenfolge|Die Beschreibung des von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) geerbten Geräts|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Der Status des Geräts in InTune, das von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt wurde. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|Plattform|[Plattform](../resources/intune-enrollment-platform.md)|Die Plattform des Geräts. Von [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)geerbt. Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.|
|status|Boolescher Wert|Status der importierten Geräte Identität|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```




