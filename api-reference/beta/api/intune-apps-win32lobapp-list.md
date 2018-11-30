---
title: Liste win32LobApps
description: Listeneigenschaften und Beziehungen der win32LobApp-Objekte.
ms.openlocfilehash: ffb4e677ab7481e0bdab94f7300c9ba20e04f8fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065998"
---
# <a name="list-win32lobapps"></a><span data-ttu-id="9c6d0-103">Liste win32LobApps</span><span class="sxs-lookup"><span data-stu-id="9c6d0-103">List win32LobApps</span></span>

> <span data-ttu-id="9c6d0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c6d0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c6d0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c6d0-107">Listeneigenschaften und Beziehungen der [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-107">List properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c6d0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9c6d0-108">Prerequisites</span></span>
<span data-ttu-id="9c6d0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c6d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c6d0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c6d0-111">Permission type</span></span>|<span data-ttu-id="9c6d0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c6d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c6d0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c6d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c6d0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c6d0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9c6d0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c6d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c6d0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c6d0-116">Not supported.</span></span>|
|<span data-ttu-id="9c6d0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c6d0-117">Application</span></span>|<span data-ttu-id="9c6d0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c6d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c6d0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c6d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9c6d0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c6d0-120">Request headers</span></span>
|<span data-ttu-id="9c6d0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9c6d0-121">Header</span></span>|<span data-ttu-id="9c6d0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9c6d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c6d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c6d0-123">Authorization</span></span>|<span data-ttu-id="9c6d0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9c6d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c6d0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c6d0-125">Accept</span></span>|<span data-ttu-id="9c6d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c6d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c6d0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c6d0-127">Request body</span></span>
<span data-ttu-id="9c6d0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c6d0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c6d0-129">Response</span></span>
<span data-ttu-id="9c6d0-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9c6d0-130">If successful, this method returns a `200 OK` response code and a collection of [win32LobApp](../resources/intune-apps-win32lobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c6d0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c6d0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c6d0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c6d0-132">Request</span></span>
<span data-ttu-id="9c6d0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="9c6d0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c6d0-134">Response</span></span>
<span data-ttu-id="9c6d0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2689

{
  "value": [
    {
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
  ]
}
```




