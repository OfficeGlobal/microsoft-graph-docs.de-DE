---
title: Auflisten von „managedIOSLobApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedIOSLobApp auf.
ms.openlocfilehash: 8abe28a64baae857a16f95bd005568602fd6f8f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018171"
---
# <a name="list-managedioslobapps"></a><span data-ttu-id="6b70a-103">Auflisten von „managedIOSLobApp“</span><span class="sxs-lookup"><span data-stu-id="6b70a-103">List managedIOSLobApps</span></span>

> <span data-ttu-id="6b70a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6b70a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b70a-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="6b70a-105">List properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b70a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6b70a-106">Prerequisites</span></span>
<span data-ttu-id="6b70a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b70a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b70a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b70a-109">Permission type</span></span>|<span data-ttu-id="6b70a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b70a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b70a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b70a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6b70a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b70a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6b70a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b70a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b70a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b70a-114">Not supported.</span></span>|
|<span data-ttu-id="6b70a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b70a-115">Application</span></span>|<span data-ttu-id="6b70a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b70a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b70a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b70a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6b70a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b70a-118">Request headers</span></span>
|<span data-ttu-id="6b70a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6b70a-119">Header</span></span>|<span data-ttu-id="6b70a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6b70a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b70a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b70a-121">Authorization</span></span>|<span data-ttu-id="6b70a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6b70a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b70a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6b70a-123">Accept</span></span>|<span data-ttu-id="6b70a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6b70a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b70a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b70a-125">Request body</span></span>
<span data-ttu-id="6b70a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6b70a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b70a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b70a-127">Response</span></span>
<span data-ttu-id="6b70a-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6b70a-128">If successful, this method returns a `200 OK` response code and a collection of [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b70a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b70a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b70a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b70a-130">Request</span></span>
<span data-ttu-id="6b70a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b70a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="6b70a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b70a-132">Response</span></span>
<span data-ttu-id="6b70a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b70a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1656

{
  "value": [
    {
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
      "publishingState": "processing",
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
      "buildNumber": "Build Number value"
    }
  ]
}
```



