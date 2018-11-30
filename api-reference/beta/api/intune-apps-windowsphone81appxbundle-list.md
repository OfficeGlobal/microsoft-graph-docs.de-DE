---
title: Liste windowsPhone81AppXBundles
description: Listeneigenschaften und Beziehungen der windowsPhone81AppXBundle-Objekte.
ms.openlocfilehash: 074aab47ee3a2cf35f34230201af984d9803491a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063108"
---
# <a name="list-windowsphone81appxbundles"></a><span data-ttu-id="2dbc5-103">Liste windowsPhone81AppXBundles</span><span class="sxs-lookup"><span data-stu-id="2dbc5-103">List windowsPhone81AppXBundles</span></span>

> <span data-ttu-id="2dbc5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2dbc5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2dbc5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2dbc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2dbc5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2dbc5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2dbc5-107">Listeneigenschaften und Beziehungen der [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="2dbc5-107">List properties and relationships of the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2dbc5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2dbc5-108">Prerequisites</span></span>
<span data-ttu-id="2dbc5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dbc5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dbc5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2dbc5-111">Permission type</span></span>|<span data-ttu-id="2dbc5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2dbc5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dbc5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2dbc5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2dbc5-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2dbc5-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2dbc5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2dbc5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dbc5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2dbc5-116">Not supported.</span></span>|
|<span data-ttu-id="2dbc5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2dbc5-117">Application</span></span>|<span data-ttu-id="2dbc5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2dbc5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dbc5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2dbc5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2dbc5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2dbc5-120">Request headers</span></span>
|<span data-ttu-id="2dbc5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2dbc5-121">Header</span></span>|<span data-ttu-id="2dbc5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2dbc5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2dbc5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2dbc5-123">Authorization</span></span>|<span data-ttu-id="2dbc5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2dbc5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2dbc5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2dbc5-125">Accept</span></span>|<span data-ttu-id="2dbc5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2dbc5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dbc5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2dbc5-127">Request body</span></span>
<span data-ttu-id="2dbc5-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2dbc5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2dbc5-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2dbc5-129">Response</span></span>
<span data-ttu-id="2dbc5-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="2dbc5-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dbc5-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2dbc5-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2dbc5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2dbc5-132">Request</span></span>
<span data-ttu-id="2dbc5-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2dbc5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="2dbc5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2dbc5-134">Response</span></span>
<span data-ttu-id="2dbc5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2dbc5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2548

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
      "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
      "identityVersion": "Identity Version value",
      "appXPackageInformationList": [
        {
          "@odata.type": "microsoft.graph.windowsPackageInformation",
          "applicableArchitecture": "x86",
          "displayName": "Display Name value",
          "identityName": "Identity Name value",
          "identityPublisher": "Identity Publisher value",
          "identityResourceIdentifier": "Identity Resource Identifier value",
          "identityVersion": "Identity Version value",
          "minimumSupportedOperatingSystem": {
            "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
            "v8_0": true,
            "v8_1": true,
            "v10_0": true,
            "v10_1607": true,
            "v10_1703": true,
            "v10_1709": true,
            "v10_1803": true
          }
        }
      ]
    }
  ]
}
```





