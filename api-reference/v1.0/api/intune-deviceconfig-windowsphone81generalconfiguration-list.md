---
title: Auflisten von „windowsPhone81GeneralConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsPhone81GeneralConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da67f8563bf689115d22cc10ad48f11e2704c51b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968042"
---
# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="e648f-103">Auflisten von „windowsPhone81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="e648f-103">List windowsPhone81GeneralConfigurations</span></span>

> <span data-ttu-id="e648f-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e648f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e648f-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="e648f-105">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e648f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e648f-106">Prerequisites</span></span>
<span data-ttu-id="e648f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e648f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e648f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e648f-109">Permission type</span></span>|<span data-ttu-id="e648f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e648f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e648f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e648f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e648f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e648f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e648f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e648f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e648f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e648f-114">Not supported.</span></span>|
|<span data-ttu-id="e648f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e648f-115">Application</span></span>|<span data-ttu-id="e648f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e648f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e648f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e648f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e648f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e648f-118">Request headers</span></span>
|<span data-ttu-id="e648f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e648f-119">Header</span></span>|<span data-ttu-id="e648f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e648f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e648f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e648f-121">Authorization</span></span>|<span data-ttu-id="e648f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e648f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e648f-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e648f-123">Accept</span></span>|<span data-ttu-id="e648f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e648f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e648f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e648f-125">Request body</span></span>
<span data-ttu-id="e648f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e648f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e648f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e648f-127">Response</span></span>
<span data-ttu-id="e648f-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e648f-128">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e648f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e648f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e648f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e648f-130">Request</span></span>
<span data-ttu-id="e648f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e648f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e648f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e648f-132">Response</span></span>
<span data-ttu-id="e648f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e648f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1842

{
  "value": [
    {
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
  ]
}
```



