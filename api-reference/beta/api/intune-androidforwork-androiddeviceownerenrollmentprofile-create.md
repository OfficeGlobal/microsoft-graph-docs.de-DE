---
title: Androiddeviceownerenrollmentprofile hinzugefügt erstellen
description: Erstellen eines neuen Androiddeviceownerenrollmentprofile hinzugefügt-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2034ac39671f5e949c93bc9e2b6468aa7895959
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984842"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a>Androiddeviceownerenrollmentprofile hinzugefügt erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekts.

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
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das Androiddeviceownerenrollmentprofile hinzugefügt-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der Androiddeviceownerenrollmentprofile hinzugefügt erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|accountId|String|Mandanten-GUID, zu der das Registrierungsprofil gehört.|
|id|String|Eindeutige GUID des Registrierungsprofils.|
|displayName|Zeichenfolge|Anzeigename des Registrierungsprofils.|
|description|Zeichenfolge|Beschreibung des Registrierungsprofils.|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Registrierungsprofils.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Registrierungsprofils.|
|tokenValue|String|Wert des zuletzt für das Registrierungsprofil erstellten Tokens.|
|tokenCreationDateTime|DateTimeOffset|Datum der Erstellung des zuletzt erstellten Tokens.|
|tokenExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens.|
|enrolledDeviceCount|Int32|Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte.|
|qrCodeContent|String|Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird.|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
Content-type: application/json
Content-length: 565

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 737

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```




