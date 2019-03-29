---
title: managedIOSLobApp abrufen
description: Lesen von Eigenschaften und Beziehungen des managedIOSLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb615f9c416029e122852c0396a7c03a604905ed
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969526"
---
# <a name="get-managedioslobapp"></a><span data-ttu-id="74117-103">managedIOSLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="74117-103">Get managedIOSLobApp</span></span>

> <span data-ttu-id="74117-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="74117-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74117-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="74117-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74117-106">Lesen von Eigenschaften und Beziehungen des [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="74117-106">Read properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74117-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="74117-107">Prerequisites</span></span>
<span data-ttu-id="74117-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74117-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74117-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74117-110">Permission type</span></span>|<span data-ttu-id="74117-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74117-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74117-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74117-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74117-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="74117-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="74117-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74117-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74117-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74117-115">Not supported.</span></span>|
|<span data-ttu-id="74117-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74117-116">Application</span></span>|<span data-ttu-id="74117-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74117-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74117-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74117-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74117-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="74117-119">Optional query parameters</span></span>
<span data-ttu-id="74117-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="74117-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74117-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74117-121">Request headers</span></span>
|<span data-ttu-id="74117-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="74117-122">Header</span></span>|<span data-ttu-id="74117-123">Wert</span><span class="sxs-lookup"><span data-stu-id="74117-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74117-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="74117-124">Authorization</span></span>|<span data-ttu-id="74117-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="74117-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74117-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="74117-126">Accept</span></span>|<span data-ttu-id="74117-127">application/json</span><span class="sxs-lookup"><span data-stu-id="74117-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74117-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74117-128">Request body</span></span>
<span data-ttu-id="74117-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="74117-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74117-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="74117-130">Response</span></span>
<span data-ttu-id="74117-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74117-131">If successful, this method returns a `200 OK` response code and [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74117-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74117-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="74117-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74117-133">Request</span></span>
<span data-ttu-id="74117-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74117-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="74117-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="74117-135">Response</span></span>
<span data-ttu-id="74117-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74117-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1727

{
  "value": {
    "@odata.type": "#microsoft.graph.managedIOSLobApp",
    "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "bundleId": "Bundle Id value",
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
      "v8_0": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true,
      "v12_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value",
    "identityVersion": "Identity Version value"
  }
}
```




