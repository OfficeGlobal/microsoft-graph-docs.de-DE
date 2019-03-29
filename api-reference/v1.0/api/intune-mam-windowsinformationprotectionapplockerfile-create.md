---
title: windowsInformationProtectionAppLockerFile erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLockerFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d22e4be6d282ba7750b6c896b2592ea8b0b71a62
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984037"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a>windowsInformationProtectionAppLockerFile erstellen

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

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
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das WindowsInformationProtectionAppLockerFile-Objekt ein.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLockerFile erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Der Anzeigename|
|fileHash|String|SHA256-Hash der Datei|
|file|Binär|Datei als Bytearray|
|id|String|Schlüssel der Entität|
|Version|String|Version der Entität|



## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```



