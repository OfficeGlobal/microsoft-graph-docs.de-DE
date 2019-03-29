---
title: MacOsVppApp abrufen
description: Lesen von Eigenschaften und Beziehungen des macOsVppApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe5f85994c6aa46c422084e01661138cfb23dd52
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984597"
---
# <a name="get-macosvppapp"></a>MacOsVppApp abrufen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Lesen von Eigenschaften und Beziehungen des [macOsVppApp](../resources/intune-apps-macosvppapp.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

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
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [macOsVppApp](../resources/intune-apps-macosvppapp.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2141

{
  "value": {
    "@odata.type": "#microsoft.graph.macOsVppApp",
    "id": "10b95265-5265-10b9-6552-b9106552b910",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportUserLicensing": true,
      "supportDeviceLicensing": true,
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    },
    "vppTokenOrganizationName": "Vpp Token Organization Name value",
    "vppTokenAccountType": "education",
    "vppTokenAppleId": "Vpp Token Apple Id value",
    "bundleId": "Bundle Id value",
    "vppTokenId": "Vpp Token Id value",
    "revokeLicenseActionResults": [
      {
        "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
        "userId": "User Id value",
        "managedDeviceId": "Managed Device Id value",
        "totalLicensesCount": 2,
        "failedLicensesCount": 3,
        "actionFailureReason": "appleFailure",
        "actionName": "Action Name value",
        "actionState": "pending",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
      }
    ]
  }
}
```




