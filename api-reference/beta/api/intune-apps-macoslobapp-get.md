---
title: Abrufen von macOSLobApp
description: Lesen Sie Eigenschaften und Beziehungen des MacOSLobApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06b66861f475d20c1bf10ac4ebacee5781fb2b2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414718"
---
# <a name="get-macoslobapp"></a><span data-ttu-id="cfaef-103">Abrufen von macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="cfaef-103">Get macOSLobApp</span></span>

> <span data-ttu-id="cfaef-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cfaef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cfaef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cfaef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfaef-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cfaef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfaef-107">Lesen Sie Eigenschaften und Beziehungen des [MacOSLobApp](../resources/intune-apps-macoslobapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cfaef-107">Read properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfaef-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cfaef-108">Prerequisites</span></span>
<span data-ttu-id="cfaef-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cfaef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cfaef-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cfaef-111">Permission type</span></span>|<span data-ttu-id="cfaef-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cfaef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfaef-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cfaef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cfaef-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfaef-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cfaef-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cfaef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfaef-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cfaef-116">Not supported.</span></span>|
|<span data-ttu-id="cfaef-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cfaef-117">Application</span></span>|<span data-ttu-id="cfaef-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cfaef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfaef-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfaef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfaef-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cfaef-120">Optional query parameters</span></span>
<span data-ttu-id="cfaef-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cfaef-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfaef-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cfaef-122">Request headers</span></span>
|<span data-ttu-id="cfaef-123">Header</span><span class="sxs-lookup"><span data-stu-id="cfaef-123">Header</span></span>|<span data-ttu-id="cfaef-124">Wert</span><span class="sxs-lookup"><span data-stu-id="cfaef-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfaef-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cfaef-125">Authorization</span></span>|<span data-ttu-id="cfaef-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cfaef-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfaef-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cfaef-127">Accept</span></span>|<span data-ttu-id="cfaef-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cfaef-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfaef-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cfaef-129">Request body</span></span>
<span data-ttu-id="cfaef-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cfaef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfaef-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfaef-131">Response</span></span>
<span data-ttu-id="cfaef-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [MacOSLobApp](../resources/intune-apps-macoslobapp.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cfaef-132">If successful, this method returns a `200 OK` response code and [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfaef-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cfaef-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfaef-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfaef-134">Request</span></span>
<span data-ttu-id="cfaef-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cfaef-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="cfaef-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfaef-136">Response</span></span>
<span data-ttu-id="cfaef-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cfaef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1846

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSLobApp",
    "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
    "bundleId": "Bundle Id value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
      "v10_7": true,
      "v10_8": true,
      "v10_9": true,
      "v10_10": true,
      "v10_11": true,
      "v10_12": true,
      "v10_13": true
    },
    "buildNumber": "Build Number value",
    "versionNumber": "Version Number value",
    "childApps": [
      {
        "@odata.type": "microsoft.graph.macOSLobChildApp",
        "bundleId": "Bundle Id value",
        "buildNumber": "Build Number value",
        "versionNumber": "Version Number value"
      }
    ],
    "identityVersion": "Identity Version value",
    "md5HashChunkSize": 0,
    "md5Hash": [
      "Md5Hash value"
    ],
    "ignoreVersionDetection": true
  }
}
```




