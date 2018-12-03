---
title: Abrufen von windowsPhone81AppX
description: Lesen Sie Eigenschaften und Beziehungen des windowsPhone81AppX-Objekts.
ms.openlocfilehash: e0648a200018ea0e1c23046bfaa0a6854dc586cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065182"
---
# <a name="get-windowsphone81appx"></a><span data-ttu-id="e5cfc-103">Abrufen von windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="e5cfc-103">Get windowsPhone81AppX</span></span>

> <span data-ttu-id="e5cfc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e5cfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5cfc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5cfc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5cfc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e5cfc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5cfc-107">Lesen Sie Eigenschaften und Beziehungen des [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e5cfc-107">Read properties and relationships of the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5cfc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e5cfc-108">Prerequisites</span></span>
<span data-ttu-id="e5cfc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5cfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5cfc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e5cfc-111">Permission type</span></span>|<span data-ttu-id="e5cfc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e5cfc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5cfc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e5cfc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5cfc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5cfc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e5cfc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e5cfc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5cfc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5cfc-116">Not supported.</span></span>|
|<span data-ttu-id="e5cfc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e5cfc-117">Application</span></span>|<span data-ttu-id="e5cfc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5cfc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5cfc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5cfc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5cfc-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e5cfc-120">Optional query parameters</span></span>
<span data-ttu-id="e5cfc-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e5cfc-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e5cfc-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e5cfc-122">Request headers</span></span>
|<span data-ttu-id="e5cfc-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e5cfc-123">Header</span></span>|<span data-ttu-id="e5cfc-124">Wert</span><span class="sxs-lookup"><span data-stu-id="e5cfc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5cfc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5cfc-125">Authorization</span></span>|<span data-ttu-id="e5cfc-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e5cfc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5cfc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e5cfc-127">Accept</span></span>|<span data-ttu-id="e5cfc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e5cfc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5cfc-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e5cfc-129">Request body</span></span>
<span data-ttu-id="e5cfc-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e5cfc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5cfc-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5cfc-131">Response</span></span>
<span data-ttu-id="e5cfc-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e5cfc-132">If successful, this method returns a `200 OK` response code and [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5cfc-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e5cfc-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5cfc-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5cfc-134">Request</span></span>
<span data-ttu-id="e5cfc-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e5cfc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="e5cfc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5cfc-136">Response</span></span>
<span data-ttu-id="e5cfc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e5cfc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1626

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81AppX",
    "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
    "applicableArchitectures": "x86",
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
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
    "phoneProductIdentifier": "Phone Product Identifier value",
    "phonePublisherId": "Phone Publisher Id value",
    "identityVersion": "Identity Version value"
  }
}
```





