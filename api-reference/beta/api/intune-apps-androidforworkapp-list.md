---
title: Liste androidForWorkApps
description: Listeneigenschaften und Beziehungen der AndroidForWorkApp-Objekte.
ms.openlocfilehash: b364dce5b574e32e93dbf7d0dd53cc031928dd40
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064052"
---
# <a name="list-androidforworkapps"></a><span data-ttu-id="e1f43-103">Liste androidForWorkApps</span><span class="sxs-lookup"><span data-stu-id="e1f43-103">List androidForWorkApps</span></span>

> <span data-ttu-id="e1f43-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e1f43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1f43-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1f43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1f43-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e1f43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1f43-107">Listeneigenschaften und Beziehungen der [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="e1f43-107">List properties and relationships of the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1f43-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1f43-108">Prerequisites</span></span>
<span data-ttu-id="e1f43-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1f43-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1f43-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1f43-111">Permission type</span></span>|<span data-ttu-id="e1f43-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1f43-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1f43-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1f43-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1f43-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1f43-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e1f43-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1f43-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1f43-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1f43-116">Not supported.</span></span>|
|<span data-ttu-id="e1f43-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1f43-117">Application</span></span>|<span data-ttu-id="e1f43-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1f43-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1f43-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1f43-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e1f43-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1f43-120">Request headers</span></span>
|<span data-ttu-id="e1f43-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e1f43-121">Header</span></span>|<span data-ttu-id="e1f43-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e1f43-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1f43-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1f43-123">Authorization</span></span>|<span data-ttu-id="e1f43-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1f43-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1f43-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1f43-125">Accept</span></span>|<span data-ttu-id="e1f43-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1f43-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1f43-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1f43-127">Request body</span></span>
<span data-ttu-id="e1f43-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e1f43-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1f43-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1f43-129">Response</span></span>
<span data-ttu-id="e1f43-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e1f43-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1f43-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1f43-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1f43-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1f43-132">Request</span></span>
<span data-ttu-id="e1f43-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1f43-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="e1f43-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1f43-134">Response</span></span>
<span data-ttu-id="e1f43-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1f43-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1096

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkApp",
      "id": "c5010785-0785-c501-8507-01c5850701c5",
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
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "appStoreUrl": "https://example.com/appStoreUrl/"
    }
  ]
}
```





