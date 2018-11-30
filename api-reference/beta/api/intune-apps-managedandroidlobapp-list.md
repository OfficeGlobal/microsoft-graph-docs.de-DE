---
title: Auflisten von „managedAndroidLobApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedAndroidLobApp auf.
ms.openlocfilehash: 27637b721dffb53997fce52e2d1b9cd84b57c552
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060902"
---
# <a name="list-managedandroidlobapps"></a><span data-ttu-id="5fa94-103">Auflisten von „managedAndroidLobApp“</span><span class="sxs-lookup"><span data-stu-id="5fa94-103">List managedAndroidLobApps</span></span>

> <span data-ttu-id="5fa94-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5fa94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fa94-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5fa94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5fa94-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5fa94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fa94-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="5fa94-107">List properties and relationships of the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5fa94-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5fa94-108">Prerequisites</span></span>
<span data-ttu-id="5fa94-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fa94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fa94-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5fa94-111">Permission type</span></span>|<span data-ttu-id="5fa94-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5fa94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fa94-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5fa94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5fa94-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fa94-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5fa94-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5fa94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fa94-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fa94-116">Not supported.</span></span>|
|<span data-ttu-id="5fa94-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5fa94-117">Application</span></span>|<span data-ttu-id="5fa94-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fa94-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fa94-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fa94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5fa94-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5fa94-120">Request headers</span></span>
|<span data-ttu-id="5fa94-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5fa94-121">Header</span></span>|<span data-ttu-id="5fa94-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5fa94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fa94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fa94-123">Authorization</span></span>|<span data-ttu-id="5fa94-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5fa94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fa94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5fa94-125">Accept</span></span>|<span data-ttu-id="5fa94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5fa94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fa94-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5fa94-127">Request body</span></span>
<span data-ttu-id="5fa94-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5fa94-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fa94-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fa94-129">Response</span></span>
<span data-ttu-id="5fa94-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5fa94-130">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fa94-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5fa94-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5fa94-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fa94-132">Request</span></span>
<span data-ttu-id="5fa94-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5fa94-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="5fa94-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fa94-134">Response</span></span>
<span data-ttu-id="5fa94-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5fa94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1772

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAndroidLobApp",
      "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
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
  ]
}
```





