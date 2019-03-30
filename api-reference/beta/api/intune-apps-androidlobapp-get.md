---
title: androidLobApp abrufen
description: Lesen von Eigenschaften und Beziehungen des androidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2506bb62f4b932dbd3c9e4f3fc63a4d2bf2ba7e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989316"
---
# <a name="get-androidlobapp"></a><span data-ttu-id="5bd82-103">androidLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="5bd82-103">Get androidLobApp</span></span>

> <span data-ttu-id="5bd82-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5bd82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bd82-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5bd82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bd82-106">Lesen von Eigenschaften und Beziehungen des [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5bd82-106">Read properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bd82-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5bd82-107">Prerequisites</span></span>
<span data-ttu-id="5bd82-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bd82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bd82-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5bd82-110">Permission type</span></span>|<span data-ttu-id="5bd82-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5bd82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bd82-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5bd82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5bd82-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bd82-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5bd82-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5bd82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bd82-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5bd82-115">Not supported.</span></span>|
|<span data-ttu-id="5bd82-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5bd82-116">Application</span></span>|<span data-ttu-id="5bd82-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5bd82-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bd82-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bd82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bd82-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5bd82-119">Optional query parameters</span></span>
<span data-ttu-id="5bd82-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5bd82-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bd82-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5bd82-121">Request headers</span></span>
|<span data-ttu-id="5bd82-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5bd82-122">Header</span></span>|<span data-ttu-id="5bd82-123">Wert</span><span class="sxs-lookup"><span data-stu-id="5bd82-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bd82-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bd82-124">Authorization</span></span>|<span data-ttu-id="5bd82-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5bd82-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bd82-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5bd82-126">Accept</span></span>|<span data-ttu-id="5bd82-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5bd82-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bd82-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5bd82-128">Request body</span></span>
<span data-ttu-id="5bd82-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5bd82-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bd82-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bd82-130">Response</span></span>
<span data-ttu-id="5bd82-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bd82-131">If successful, this method returns a `200 OK` response code and [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bd82-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5bd82-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bd82-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bd82-133">Request</span></span>
<span data-ttu-id="5bd82-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5bd82-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="5bd82-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bd82-135">Response</span></span>
<span data-ttu-id="5bd82-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bd82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1675

{
  "value": {
    "@odata.type": "#microsoft.graph.androidLobApp",
    "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
    "packageId": "Package Id value",
    "identityName": "Identity Name value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true,
      "v6_0": true,
      "v7_0": true,
      "v7_1": true,
      "v8_0": true,
      "v8_1": true,
      "v9_0": true
    },
    "versionName": "Version Name value",
    "versionCode": "Version Code value",
    "identityVersion": "Identity Version value"
  }
}
```




