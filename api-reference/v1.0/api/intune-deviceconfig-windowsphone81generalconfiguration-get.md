---
title: windowsPhone81GeneralConfiguration abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a31b9a02550181bc52e10979758c9c3165dc21d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965900"
---
# <a name="get-windowsphone81generalconfiguration"></a><span data-ttu-id="5cf50-103">windowsPhone81GeneralConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="5cf50-103">Get windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="5cf50-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5cf50-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cf50-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5cf50-105">Read properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cf50-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5cf50-106">Prerequisites</span></span>
<span data-ttu-id="5cf50-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cf50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cf50-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5cf50-109">Permission type</span></span>|<span data-ttu-id="5cf50-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5cf50-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cf50-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5cf50-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5cf50-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cf50-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5cf50-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5cf50-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cf50-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5cf50-114">Not supported.</span></span>|
|<span data-ttu-id="5cf50-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5cf50-115">Application</span></span>|<span data-ttu-id="5cf50-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5cf50-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cf50-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5cf50-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cf50-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5cf50-118">Optional query parameters</span></span>
<span data-ttu-id="5cf50-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5cf50-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cf50-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5cf50-120">Request headers</span></span>
|<span data-ttu-id="5cf50-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5cf50-121">Header</span></span>|<span data-ttu-id="5cf50-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5cf50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cf50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cf50-123">Authorization</span></span>|<span data-ttu-id="5cf50-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5cf50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cf50-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5cf50-125">Accept</span></span>|<span data-ttu-id="5cf50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cf50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cf50-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5cf50-127">Request body</span></span>
<span data-ttu-id="5cf50-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5cf50-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cf50-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5cf50-129">Response</span></span>
<span data-ttu-id="5cf50-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5cf50-130">If successful, this method returns a `200 OK` response code and [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cf50-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5cf50-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cf50-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5cf50-132">Request</span></span>
<span data-ttu-id="5cf50-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5cf50-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5cf50-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5cf50-134">Response</span></span>
<span data-ttu-id="5cf50-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5cf50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1740

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
    "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "applyOnlyToWindowsPhone81": true,
    "appsBlockCopyPaste": true,
    "bluetoothBlocked": true,
    "cameraBlocked": true,
    "cellularBlockWifiTethering": true,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "diagnosticDataBlockSubmission": true,
    "emailBlockAddingAccounts": true,
    "locationServicesBlocked": true,
    "microsoftAccountBlocked": true,
    "nfcBlocked": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordMinimumCharacterSetCount": 0,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "alphanumeric",
    "passwordRequired": true,
    "screenCaptureBlocked": true,
    "storageBlockRemovableStorage": true,
    "storageRequireEncryption": true,
    "webBrowserBlocked": true,
    "wifiBlocked": true,
    "wifiBlockAutomaticConnectHotspots": true,
    "wifiBlockHotspotReporting": true,
    "windowsStoreBlocked": true
  }
}
```



