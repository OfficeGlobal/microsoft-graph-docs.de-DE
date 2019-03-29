---
title: iosLobApp abrufen
description: Liest die Beziehungen und Eigenschaften des iosLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d126d976fd2f4a451c42a105f8c8e058ce37520
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957255"
---
# <a name="get-ioslobapp"></a><span data-ttu-id="2769c-103">iosLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="2769c-103">Get iosLobApp</span></span>

> <span data-ttu-id="2769c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2769c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2769c-105">Liest die Beziehungen und Eigenschaften des [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2769c-105">Read properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2769c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2769c-106">Prerequisites</span></span>
<span data-ttu-id="2769c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2769c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2769c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2769c-109">Permission type</span></span>|<span data-ttu-id="2769c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2769c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2769c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2769c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2769c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2769c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2769c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2769c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2769c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2769c-114">Not supported.</span></span>|
|<span data-ttu-id="2769c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2769c-115">Application</span></span>|<span data-ttu-id="2769c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2769c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2769c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2769c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2769c-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2769c-118">Optional query parameters</span></span>
<span data-ttu-id="2769c-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2769c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2769c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2769c-120">Request headers</span></span>
|<span data-ttu-id="2769c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2769c-121">Header</span></span>|<span data-ttu-id="2769c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2769c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2769c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2769c-123">Authorization</span></span>|<span data-ttu-id="2769c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2769c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2769c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2769c-125">Accept</span></span>|<span data-ttu-id="2769c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2769c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2769c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2769c-127">Request body</span></span>
<span data-ttu-id="2769c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2769c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2769c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2769c-129">Response</span></span>
<span data-ttu-id="2769c-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosLobApp](../resources/intune-apps-ioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2769c-130">If successful, this method returns a `200 OK` response code and [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2769c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2769c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2769c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2769c-132">Request</span></span>
<span data-ttu-id="2769c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2769c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="2769c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2769c-134">Response</span></span>
<span data-ttu-id="2769c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2769c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1478

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobApp",
    "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
    "publishingState": "processing",
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
    "buildNumber": "Build Number value"
  }
}
```



