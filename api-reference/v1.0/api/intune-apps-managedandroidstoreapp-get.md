---
title: managedAndroidStoreApp abrufen
description: Lesen von Eigenschaften und Beziehungen des managedAndroidStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f5c4adf6f088f2eea07180c344759b124d8afc1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954645"
---
# <a name="get-managedandroidstoreapp"></a><span data-ttu-id="8c371-103">managedAndroidStoreApp abrufen</span><span class="sxs-lookup"><span data-stu-id="8c371-103">Get managedAndroidStoreApp</span></span>

> <span data-ttu-id="8c371-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8c371-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c371-105">Lesen von Eigenschaften und Beziehungen des [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8c371-105">Read properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c371-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8c371-106">Prerequisites</span></span>
<span data-ttu-id="8c371-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c371-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c371-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c371-109">Permission type</span></span>|<span data-ttu-id="8c371-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c371-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c371-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c371-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c371-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c371-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8c371-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c371-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c371-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c371-114">Not supported.</span></span>|
|<span data-ttu-id="8c371-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c371-115">Application</span></span>|<span data-ttu-id="8c371-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c371-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c371-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c371-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c371-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8c371-118">Optional query parameters</span></span>
<span data-ttu-id="8c371-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8c371-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8c371-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c371-120">Request headers</span></span>
|<span data-ttu-id="8c371-121">Header</span><span class="sxs-lookup"><span data-stu-id="8c371-121">Header</span></span>|<span data-ttu-id="8c371-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8c371-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c371-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c371-123">Authorization</span></span>|<span data-ttu-id="8c371-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8c371-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c371-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8c371-125">Accept</span></span>|<span data-ttu-id="8c371-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c371-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c371-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c371-127">Request body</span></span>
<span data-ttu-id="8c371-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8c371-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c371-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c371-129">Response</span></span>
<span data-ttu-id="8c371-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c371-130">If successful, this method returns a `200 OK` response code and [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c371-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c371-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c371-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c371-132">Request</span></span>
<span data-ttu-id="8c371-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c371-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="8c371-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c371-134">Response</span></span>
<span data-ttu-id="8c371-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c371-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



