---
title: Auflisten von „managedIOSStoreApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedIOSStoreApp auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2fa7d3cd7a5ce9adb9b27c1ee31a732fa8f6c211
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954162"
---
# <a name="list-managediosstoreapps"></a><span data-ttu-id="aaa45-103">Auflisten von „managedIOSStoreApp“</span><span class="sxs-lookup"><span data-stu-id="aaa45-103">List managedIOSStoreApps</span></span>

> <span data-ttu-id="aaa45-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aaa45-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aaa45-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="aaa45-105">List properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aaa45-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aaa45-106">Prerequisites</span></span>
<span data-ttu-id="aaa45-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaa45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaa45-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aaa45-109">Permission type</span></span>|<span data-ttu-id="aaa45-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aaa45-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaa45-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aaa45-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aaa45-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aaa45-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aaa45-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aaa45-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaa45-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aaa45-114">Not supported.</span></span>|
|<span data-ttu-id="aaa45-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aaa45-115">Application</span></span>|<span data-ttu-id="aaa45-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aaa45-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaa45-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaa45-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="aaa45-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aaa45-118">Request headers</span></span>
|<span data-ttu-id="aaa45-119">Header</span><span class="sxs-lookup"><span data-stu-id="aaa45-119">Header</span></span>|<span data-ttu-id="aaa45-120">Wert</span><span class="sxs-lookup"><span data-stu-id="aaa45-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaa45-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaa45-121">Authorization</span></span>|<span data-ttu-id="aaa45-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aaa45-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaa45-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="aaa45-123">Accept</span></span>|<span data-ttu-id="aaa45-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aaa45-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaa45-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aaa45-125">Request body</span></span>
<span data-ttu-id="aaa45-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aaa45-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaa45-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaa45-127">Response</span></span>
<span data-ttu-id="aaa45-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="aaa45-128">If successful, this method returns a `200 OK` response code and a collection of [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaa45-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aaa45-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="aaa45-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaa45-130">Request</span></span>
<span data-ttu-id="aaa45-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aaa45-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="aaa45-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaa45-132">Response</span></span>
<span data-ttu-id="aaa45-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aaa45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1433

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSStoreApp",
      "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
      "bundleId": "Bundle Id value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
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
      }
    }
  ]
}
```



