---
title: Abrufen von win32LobApp
description: Lesen Sie Eigenschaften und Beziehungen des win32LobApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d80b0003f744c8f75ba2a219c951e4aa2c9db670
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397071"
---
# <a name="get-win32lobapp"></a><span data-ttu-id="88208-103">Abrufen von win32LobApp</span><span class="sxs-lookup"><span data-stu-id="88208-103">Get win32LobApp</span></span>

> <span data-ttu-id="88208-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="88208-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88208-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88208-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88208-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="88208-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88208-107">Lesen Sie Eigenschaften und Beziehungen des [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="88208-107">Read properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88208-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="88208-108">Prerequisites</span></span>
<span data-ttu-id="88208-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="88208-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88208-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="88208-111">Permission type</span></span>|<span data-ttu-id="88208-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="88208-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88208-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="88208-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88208-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88208-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="88208-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="88208-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88208-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88208-116">Not supported.</span></span>|
|<span data-ttu-id="88208-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="88208-117">Application</span></span>|<span data-ttu-id="88208-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88208-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88208-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="88208-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88208-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="88208-120">Optional query parameters</span></span>
<span data-ttu-id="88208-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="88208-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88208-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="88208-122">Request headers</span></span>
|<span data-ttu-id="88208-123">Header</span><span class="sxs-lookup"><span data-stu-id="88208-123">Header</span></span>|<span data-ttu-id="88208-124">Wert</span><span class="sxs-lookup"><span data-stu-id="88208-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88208-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="88208-125">Authorization</span></span>|<span data-ttu-id="88208-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="88208-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88208-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="88208-127">Accept</span></span>|<span data-ttu-id="88208-128">application/json</span><span class="sxs-lookup"><span data-stu-id="88208-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88208-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="88208-129">Request body</span></span>
<span data-ttu-id="88208-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="88208-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88208-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="88208-131">Response</span></span>
<span data-ttu-id="88208-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [win32LobApp](../resources/intune-apps-win32lobapp.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="88208-132">If successful, this method returns a `200 OK` response code and [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88208-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="88208-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="88208-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="88208-134">Request</span></span>
<span data-ttu-id="88208-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="88208-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="88208-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="88208-136">Response</span></span>
<span data-ttu-id="88208-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="88208-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2626

{
  "value": {
    "@odata.type": "#microsoft.graph.win32LobApp",
    "id": "9607b530-b530-9607-30b5-079630b50796",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "installCommandLine": "Install Command Line value",
    "uninstallCommandLine": "Uninstall Command Line value",
    "applicableArchitectures": "x86",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true,
      "v10_1607": true,
      "v10_1703": true,
      "v10_1709": true,
      "v10_1803": true
    },
    "minimumFreeDiskSpaceInMB": 8,
    "minimumMemoryInMB": 1,
    "minimumNumberOfProcessors": 9,
    "minimumCpuSpeedInMHz": 4,
    "detectionRules": [
      {
        "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
        "check32BitOn64System": true,
        "keyPath": "Key Path value",
        "valueName": "Value Name value",
        "detectionType": "exists",
        "operator": "equal",
        "detectionValue": "Detection Value value"
      }
    ],
    "installExperience": {
      "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
      "runAsAccount": "user"
    },
    "returnCodes": [
      {
        "@odata.type": "microsoft.graph.win32LobAppReturnCode",
        "returnCode": 10,
        "type": "success"
      }
    ],
    "msiInformation": {
      "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
      "productCode": "Product Code value",
      "productVersion": "Product Version value",
      "upgradeCode": "Upgrade Code value",
      "requiresReboot": true,
      "packageType": "perUser"
    },
    "setupFilePath": "Setup File Path value"
  }
}
```




