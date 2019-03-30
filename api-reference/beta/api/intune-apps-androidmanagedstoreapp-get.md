---
title: AndroidManagedStoreApp abrufen
description: Lesen von Eigenschaften und Beziehungen des androidManagedStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e57057f856529322931d5681d4e3faf9e234f427
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977100"
---
# <a name="get-androidmanagedstoreapp"></a><span data-ttu-id="298fb-103">AndroidManagedStoreApp abrufen</span><span class="sxs-lookup"><span data-stu-id="298fb-103">Get androidManagedStoreApp</span></span>

> <span data-ttu-id="298fb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="298fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="298fb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="298fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="298fb-106">Lesen von Eigenschaften und Beziehungen des [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="298fb-106">Read properties and relationships of the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="298fb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="298fb-107">Prerequisites</span></span>
<span data-ttu-id="298fb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="298fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="298fb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="298fb-110">Permission type</span></span>|<span data-ttu-id="298fb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="298fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="298fb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="298fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="298fb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="298fb-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="298fb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="298fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="298fb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="298fb-115">Not supported.</span></span>|
|<span data-ttu-id="298fb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="298fb-116">Application</span></span>|<span data-ttu-id="298fb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="298fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="298fb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="298fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="298fb-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="298fb-119">Optional query parameters</span></span>
<span data-ttu-id="298fb-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="298fb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="298fb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="298fb-121">Request headers</span></span>
|<span data-ttu-id="298fb-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="298fb-122">Header</span></span>|<span data-ttu-id="298fb-123">Wert</span><span class="sxs-lookup"><span data-stu-id="298fb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="298fb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="298fb-124">Authorization</span></span>|<span data-ttu-id="298fb-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="298fb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="298fb-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="298fb-126">Accept</span></span>|<span data-ttu-id="298fb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="298fb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="298fb-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="298fb-128">Request body</span></span>
<span data-ttu-id="298fb-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="298fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="298fb-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="298fb-130">Response</span></span>
<span data-ttu-id="298fb-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="298fb-131">If successful, this method returns a `200 OK` response code and [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="298fb-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="298fb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="298fb-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="298fb-133">Request</span></span>
<span data-ttu-id="298fb-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="298fb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="298fb-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="298fb-135">Response</span></span>
<span data-ttu-id="298fb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="298fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1162

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreApp",
    "id": "87247525-7525-8724-2575-248725752487",
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
    "packageId": "Package Id value",
    "appIdentifier": "App Identifier value",
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "supportsOemConfig": true
  }
}
```




