---
title: WindowsInformationProtectionWipeActions aufListen
description: AufListen von Eigenschaften und Beziehungen der windowsInformationProtectionWipeAction-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed0e69af9061151c6fc13cc62c7ec554655d2103
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163595"
---
# <a name="list-windowsinformationprotectionwipeactions"></a>WindowsInformationProtectionWipeActions aufListen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

AufListen von Eigenschaften und Beziehungen der [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekte.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekten im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
      "id": "2620a996-a996-2620-96a9-202696a92026",
      "status": "pending",
      "targetedUserId": "Targeted User Id value",
      "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
      "targetedDeviceName": "Targeted Device Name value",
      "targetedDeviceMacAddress": "Targeted Device Mac Address value",
      "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
    }
  ]
}
```




