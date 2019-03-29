---
title: WindowsPrivacyDataAccessControlItem aktualisieren
description: Aktualisieren der Eigenschaften eines windowsPrivacyDataAccessControlItem-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f865b3349662309e4bb4821e4911289df579d9b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984317"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a>WindowsPrivacyDataAccessControlItem aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekts.

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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Der Schlüssel von WindowsPrivacyDataAccessControlItem.|
|Access Level|[windowsPrivacyDataAccessLevel](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|Dies gibt eine Zugriffsebene für die Datenschutzkategorie an, der die angegebene Anwendung zugewiesen wird. Mögliche Werte sind: `notConfigured`, `forceAllow`, `forceDeny` und `userInControl`.|
|dataCategory|[windowsPrivacyDataCategory](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|Dies gibt eine Datenschutzkategorie an, auf die die spezifische Zugriffssteuerung angewendet werden soll. Mögliche Werte sind: `notConfigured`, `accountInfo`, `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `email` `location` `messaging` `microphone` `motion` `notifications` `phone`,,,,,,,, `radios`,, `trustedDevices` ,,,,,, `tasks` `syncWithDevices` `diagnosticsInfo` .|
|appPackageFamilyName|String|Der Name der Paketfamilie einer Windows-app. Wenn diese Einstellung festgelegt ist, gilt die Zugriffsebene für die angegebene Anwendung.|
|appDisplayName|String|Der Name der Paketfamilie einer Windows-app. Wenn diese Einstellung festgelegt ist, gilt die Zugriffsebene für die angegebene Anwendung.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "03b15556-5556-03b1-5655-b1035655b103",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```




