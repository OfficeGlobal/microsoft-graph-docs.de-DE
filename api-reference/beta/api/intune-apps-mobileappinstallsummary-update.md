---
title: MobileAppInstallSummary aktualisieren
description: Aktualisieren der Eigenschaften eines mobileAppInstallSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6065083d5ceb5892a95a6b12bc99657eca7d3eeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152955"
---
# <a name="update-mobileappinstallsummary"></a>MobileAppInstallSummary aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementApps.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|installedDeviceCount|Int32|Die Anzahl der Geräte, die diese APP erfolgreich installiert haben.|
|failedDeviceCount|Int32|Anzahl der Geräte, die diese APP nicht installiert haben.|
|notApplicableDeviceCount|Int32|Die Anzahl der Geräte, die für diese APP nicht anwendbar sind.|
|notInstalledDeviceCount|Int32|Anzahl der Geräte, auf denen diese APP nicht installiert ist.|
|pendingInstallDeviceCount|Int32|Anzahl der Geräte, die zur Installation dieser APP benachrichtigt wurden.|
|installedUserCount|Int32|Die Anzahl der Benutzer, deren Geräte alle für die Installation dieser APP erfolgreich waren.|
|failedUserCount|Int32|Die Anzahl der Benutzer, die über ein Gerät verfügen, für das diese APP nicht installiert werden konnte.|
|notApplicableUserCount|Int32|Die Anzahl der Benutzer, deren Geräte für diese APP nicht anwendbar waren.|
|notInstalledUserCount|Int32|Die Anzahl von Benutzern, die über 1 oder mehr Geräte verfügen, die diese APP nicht installiert haben.|
|pendingInstallUserCount|Int32|Die Anzahl der Benutzer mit mindestens 1 Gerät, die zur Installation dieser APP benachrichtigt wurden und über 0 Geräte mit Fehlern verfügen.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "06a792e9-92e9-06a7-e992-a706e992a706",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```




