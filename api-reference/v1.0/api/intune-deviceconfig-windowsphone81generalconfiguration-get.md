---
title: windowsPhone81GeneralConfiguration abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb2d0ba56c8df2873116d97e0c5bb901ba7c921d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264267"
---
# <a name="get-windowsphone81generalconfiguration"></a><span data-ttu-id="93bbc-103">windowsPhone81GeneralConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="93bbc-103">Get windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="93bbc-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="93bbc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93bbc-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="93bbc-105">Read properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93bbc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="93bbc-106">Prerequisites</span></span>
<span data-ttu-id="93bbc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="93bbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="93bbc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93bbc-109">Permission type</span></span>|<span data-ttu-id="93bbc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93bbc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93bbc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93bbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="93bbc-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="93bbc-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="93bbc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93bbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93bbc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93bbc-114">Not supported.</span></span>|
|<span data-ttu-id="93bbc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93bbc-115">Application</span></span>|<span data-ttu-id="93bbc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93bbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93bbc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93bbc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93bbc-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="93bbc-118">Optional query parameters</span></span>
<span data-ttu-id="93bbc-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93bbc-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93bbc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93bbc-120">Request headers</span></span>
|<span data-ttu-id="93bbc-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="93bbc-121">Header</span></span>|<span data-ttu-id="93bbc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="93bbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93bbc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="93bbc-123">Authorization</span></span>|<span data-ttu-id="93bbc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="93bbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93bbc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="93bbc-125">Accept</span></span>|<span data-ttu-id="93bbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93bbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93bbc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93bbc-127">Request body</span></span>
<span data-ttu-id="93bbc-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="93bbc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93bbc-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="93bbc-129">Response</span></span>
<span data-ttu-id="93bbc-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93bbc-130">If successful, this method returns a `200 OK` response code and [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93bbc-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93bbc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="93bbc-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93bbc-132">Request</span></span>
<span data-ttu-id="93bbc-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93bbc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="93bbc-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="93bbc-134">Response</span></span>
<span data-ttu-id="93bbc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93bbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



