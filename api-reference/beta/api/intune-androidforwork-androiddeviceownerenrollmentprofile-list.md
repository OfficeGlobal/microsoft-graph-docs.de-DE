---
title: AndroidDeviceOwnerEnrollmentProfiles aufListen
description: AufListen von Eigenschaften und Beziehungen der Androiddeviceownerenrollmentprofile hinzugefügt-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6c9164a02f7e94484ee254227bf1ec50d201ee7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980446"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a>AndroidDeviceOwnerEnrollmentProfiles aufListen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

AufListen von Eigenschaften und Beziehungen der [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekte.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekten im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 838

{
  "value": [
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
  ]
}
```




