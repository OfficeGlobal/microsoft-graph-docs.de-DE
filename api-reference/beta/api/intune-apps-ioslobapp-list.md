---
title: Auflisten von „iosLobApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosLobApp auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 64094953674bb43387037fef4ba4316feba79eb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879338"
---
# <a name="list-ioslobapps"></a><span data-ttu-id="98a17-103">Auflisten von „iosLobApp“</span><span class="sxs-lookup"><span data-stu-id="98a17-103">List iosLobApps</span></span>

> <span data-ttu-id="98a17-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="98a17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98a17-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="98a17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98a17-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="98a17-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98a17-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosLobApp](../resources/intune-apps-ioslobapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="98a17-107">List properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98a17-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="98a17-108">Prerequisites</span></span>
<span data-ttu-id="98a17-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98a17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98a17-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="98a17-111">Permission type</span></span>|<span data-ttu-id="98a17-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="98a17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98a17-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="98a17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98a17-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="98a17-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="98a17-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="98a17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98a17-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98a17-116">Not supported.</span></span>|
|<span data-ttu-id="98a17-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="98a17-117">Application</span></span>|<span data-ttu-id="98a17-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98a17-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98a17-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98a17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="98a17-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="98a17-120">Request headers</span></span>
|<span data-ttu-id="98a17-121">Header</span><span class="sxs-lookup"><span data-stu-id="98a17-121">Header</span></span>|<span data-ttu-id="98a17-122">Wert</span><span class="sxs-lookup"><span data-stu-id="98a17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98a17-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98a17-123">Authorization</span></span>|<span data-ttu-id="98a17-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="98a17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98a17-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="98a17-125">Accept</span></span>|<span data-ttu-id="98a17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98a17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98a17-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="98a17-127">Request body</span></span>
<span data-ttu-id="98a17-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="98a17-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98a17-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="98a17-129">Response</span></span>
<span data-ttu-id="98a17-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosLobApp](../resources/intune-apps-ioslobapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="98a17-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobApp](../resources/intune-apps-ioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98a17-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="98a17-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="98a17-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="98a17-132">Request</span></span>
<span data-ttu-id="98a17-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="98a17-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="98a17-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="98a17-134">Response</span></span>
<span data-ttu-id="98a17-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98a17-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1648

{
  "value": [
    {
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
      "uploadState": 11,
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
      "buildNumber": "Build Number value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```





