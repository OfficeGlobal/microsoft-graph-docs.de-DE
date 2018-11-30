---
title: managedIOSStoreApp abrufen
description: Lesen von Eigenschaften und Beziehungen des managedIOSStoreApp-Objekts.
ms.openlocfilehash: f6a06bdb6295bce4e5a46284cba57b1730cc3174
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019431"
---
# <a name="get-managediosstoreapp"></a><span data-ttu-id="d3f98-103">managedIOSStoreApp abrufen</span><span class="sxs-lookup"><span data-stu-id="d3f98-103">Get managedIOSStoreApp</span></span>

> <span data-ttu-id="d3f98-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d3f98-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3f98-105">Lesen von Eigenschaften und Beziehungen des [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d3f98-105">Read properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3f98-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d3f98-106">Prerequisites</span></span>
<span data-ttu-id="d3f98-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3f98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3f98-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3f98-109">Permission type</span></span>|<span data-ttu-id="d3f98-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3f98-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3f98-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3f98-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3f98-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3f98-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d3f98-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3f98-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3f98-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3f98-114">Not supported.</span></span>|
|<span data-ttu-id="d3f98-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3f98-115">Application</span></span>|<span data-ttu-id="d3f98-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3f98-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3f98-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3f98-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3f98-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d3f98-118">Optional query parameters</span></span>
<span data-ttu-id="d3f98-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d3f98-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d3f98-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3f98-120">Request headers</span></span>
|<span data-ttu-id="d3f98-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d3f98-121">Header</span></span>|<span data-ttu-id="d3f98-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d3f98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3f98-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3f98-123">Authorization</span></span>|<span data-ttu-id="d3f98-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d3f98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3f98-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3f98-125">Accept</span></span>|<span data-ttu-id="d3f98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3f98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3f98-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3f98-127">Request body</span></span>
<span data-ttu-id="d3f98-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d3f98-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3f98-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3f98-129">Response</span></span>
<span data-ttu-id="d3f98-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3f98-130">If successful, this method returns a `200 OK` response code and [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3f98-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3f98-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3f98-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3f98-132">Request</span></span>
<span data-ttu-id="d3f98-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3f98-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d3f98-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3f98-134">Response</span></span>
<span data-ttu-id="d3f98-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3f98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1347

{
  "value": {
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
}
```



