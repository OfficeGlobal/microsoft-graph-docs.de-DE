---
title: managedAndroidStoreApp abrufen
description: Lesen von Eigenschaften und Beziehungen des managedAndroidStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33061fcd9e9330b2f633206a8e8b38d452163978
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257393"
---
# <a name="get-managedandroidstoreapp"></a><span data-ttu-id="7fbce-103">managedAndroidStoreApp abrufen</span><span class="sxs-lookup"><span data-stu-id="7fbce-103">Get managedAndroidStoreApp</span></span>

> <span data-ttu-id="7fbce-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7fbce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fbce-105">Lesen von Eigenschaften und Beziehungen des [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7fbce-105">Read properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fbce-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7fbce-106">Prerequisites</span></span>
<span data-ttu-id="7fbce-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7fbce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7fbce-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7fbce-109">Permission type</span></span>|<span data-ttu-id="7fbce-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7fbce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fbce-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7fbce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7fbce-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fbce-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7fbce-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7fbce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fbce-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7fbce-114">Not supported.</span></span>|
|<span data-ttu-id="7fbce-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7fbce-115">Application</span></span>|<span data-ttu-id="7fbce-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7fbce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fbce-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7fbce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fbce-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7fbce-118">Optional query parameters</span></span>
<span data-ttu-id="7fbce-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7fbce-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fbce-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7fbce-120">Request headers</span></span>
|<span data-ttu-id="7fbce-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7fbce-121">Header</span></span>|<span data-ttu-id="7fbce-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7fbce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fbce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fbce-123">Authorization</span></span>|<span data-ttu-id="7fbce-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7fbce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fbce-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7fbce-125">Accept</span></span>|<span data-ttu-id="7fbce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fbce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fbce-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7fbce-127">Request body</span></span>
<span data-ttu-id="7fbce-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7fbce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fbce-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7fbce-129">Response</span></span>
<span data-ttu-id="7fbce-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7fbce-130">If successful, this method returns a `200 OK` response code and [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fbce-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7fbce-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fbce-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7fbce-132">Request</span></span>
<span data-ttu-id="7fbce-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7fbce-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="7fbce-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7fbce-134">Response</span></span>
<span data-ttu-id="7fbce-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7fbce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1275

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
    "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
    "packageId": "Package Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true
    }
  }
}
```



