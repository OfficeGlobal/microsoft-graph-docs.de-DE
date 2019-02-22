---
title: Abrufen von „microsoftStoreForBusinessApp“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 413021214e56182f51c70a8202268d4ad562ee8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140796"
---
# <a name="get-microsoftstoreforbusinessapp"></a><span data-ttu-id="a0f80-103">Abrufen von „microsoftStoreForBusinessApp“</span><span class="sxs-lookup"><span data-stu-id="a0f80-103">Get microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="a0f80-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a0f80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0f80-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a0f80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0f80-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="a0f80-106">Read properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0f80-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a0f80-107">Prerequisites</span></span>
<span data-ttu-id="a0f80-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a0f80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a0f80-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0f80-110">Permission type</span></span>|<span data-ttu-id="a0f80-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0f80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0f80-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0f80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0f80-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0f80-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a0f80-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0f80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0f80-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0f80-115">Not supported.</span></span>|
|<span data-ttu-id="a0f80-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0f80-116">Application</span></span>|<span data-ttu-id="a0f80-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0f80-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0f80-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0f80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0f80-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a0f80-119">Optional query parameters</span></span>
<span data-ttu-id="a0f80-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a0f80-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0f80-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0f80-121">Request headers</span></span>
|<span data-ttu-id="a0f80-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a0f80-122">Header</span></span>|<span data-ttu-id="a0f80-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a0f80-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0f80-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0f80-124">Authorization</span></span>|<span data-ttu-id="a0f80-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a0f80-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0f80-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a0f80-126">Accept</span></span>|<span data-ttu-id="a0f80-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a0f80-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0f80-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a0f80-128">Request body</span></span>
<span data-ttu-id="a0f80-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a0f80-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0f80-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0f80-130">Response</span></span>
<span data-ttu-id="a0f80-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a0f80-131">If successful, this method returns a `200 OK` response code and [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0f80-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a0f80-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0f80-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0f80-133">Request</span></span>
<span data-ttu-id="a0f80-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a0f80-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="a0f80-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0f80-135">Response</span></span>
<span data-ttu-id="a0f80-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a0f80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1368

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
    "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "productKey": "Product Key value",
    "licenseType": "online",
    "packageIdentityName": "Package Identity Name value",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportUserLicensing": true,
      "supportDeviceLicensing": true,
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    }
  }
}
```




