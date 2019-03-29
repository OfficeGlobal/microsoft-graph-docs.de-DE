---
title: Auflisten von „iosVppApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosVppApp auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba31286eb405c7d7e7699bef471a84e15e13de7c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966495"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="ce446-103">Auflisten von „iosVppApp“</span><span class="sxs-lookup"><span data-stu-id="ce446-103">List iosVppApps</span></span>

> <span data-ttu-id="ce446-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ce446-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce446-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ce446-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce446-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosVppApp](../resources/intune-apps-iosvppapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="ce446-106">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce446-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ce446-107">Prerequisites</span></span>
<span data-ttu-id="ce446-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce446-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce446-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce446-110">Permission type</span></span>|<span data-ttu-id="ce446-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce446-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce446-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce446-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce446-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce446-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ce446-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce446-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce446-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce446-115">Not supported.</span></span>|
|<span data-ttu-id="ce446-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce446-116">Application</span></span>|<span data-ttu-id="ce446-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce446-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce446-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce446-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ce446-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce446-119">Request headers</span></span>
|<span data-ttu-id="ce446-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ce446-120">Header</span></span>|<span data-ttu-id="ce446-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ce446-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce446-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce446-122">Authorization</span></span>|<span data-ttu-id="ce446-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ce446-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce446-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ce446-124">Accept</span></span>|<span data-ttu-id="ce446-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce446-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce446-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce446-126">Request body</span></span>
<span data-ttu-id="ce446-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ce446-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce446-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce446-128">Response</span></span>
<span data-ttu-id="ce446-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosVppApp](../resources/intune-apps-iosvppapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ce446-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce446-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce446-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce446-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce446-131">Request</span></span>
<span data-ttu-id="ce446-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce446-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="ce446-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce446-133">Response</span></span>
<span data-ttu-id="ce446-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce446-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2413

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppApp",
      "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType",
        "supportUserLicensing": true,
        "supportDeviceLicensing": true,
        "supportsUserLicensing": true,
        "supportsDeviceLicensing": true
      },
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "vppTokenOrganizationName": "Vpp Token Organization Name value",
      "vppTokenAccountType": "education",
      "vppTokenAppleId": "Vpp Token Apple Id value",
      "bundleId": "Bundle Id value",
      "vppTokenId": "Vpp Token Id value",
      "revokeLicenseActionResults": [
        {
          "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
          "userId": "User Id value",
          "managedDeviceId": "Managed Device Id value",
          "totalLicensesCount": 2,
          "failedLicensesCount": 3,
          "actionFailureReason": "appleFailure",
          "actionName": "Action Name value",
          "actionState": "pending",
          "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
          "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
        }
      ]
    }
  ]
}
```




