---
title: Abrufen von androidForWorkApp
description: Lesen Sie Eigenschaften und Beziehungen des AndroidForWorkApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9bcc812619843edff4cece1b6dabe30c8ccf49d5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935871"
---
# <a name="get-androidforworkapp"></a><span data-ttu-id="70918-103">Abrufen von androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="70918-103">Get androidForWorkApp</span></span>

> <span data-ttu-id="70918-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="70918-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70918-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70918-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70918-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="70918-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70918-107">Lesen Sie Eigenschaften und Beziehungen des [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="70918-107">Read properties and relationships of the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70918-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="70918-108">Prerequisites</span></span>
<span data-ttu-id="70918-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70918-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70918-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70918-111">Permission type</span></span>|<span data-ttu-id="70918-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70918-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70918-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70918-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70918-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="70918-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="70918-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70918-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70918-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70918-116">Not supported.</span></span>|
|<span data-ttu-id="70918-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70918-117">Application</span></span>|<span data-ttu-id="70918-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70918-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70918-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70918-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70918-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="70918-120">Optional query parameters</span></span>
<span data-ttu-id="70918-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70918-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="70918-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70918-122">Request headers</span></span>
|<span data-ttu-id="70918-123">Header</span><span class="sxs-lookup"><span data-stu-id="70918-123">Header</span></span>|<span data-ttu-id="70918-124">Wert</span><span class="sxs-lookup"><span data-stu-id="70918-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70918-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="70918-125">Authorization</span></span>|<span data-ttu-id="70918-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="70918-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70918-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="70918-127">Accept</span></span>|<span data-ttu-id="70918-128">application/json</span><span class="sxs-lookup"><span data-stu-id="70918-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70918-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70918-129">Request body</span></span>
<span data-ttu-id="70918-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="70918-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70918-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="70918-131">Response</span></span>
<span data-ttu-id="70918-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="70918-132">If successful, this method returns a `200 OK` response code and [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70918-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70918-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="70918-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70918-134">Request</span></span>
<span data-ttu-id="70918-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70918-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="70918-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="70918-136">Response</span></span>
<span data-ttu-id="70918-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70918-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1032

{
  "value": {
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
}
```





