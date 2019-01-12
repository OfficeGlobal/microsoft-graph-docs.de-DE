---
title: Abrufen von androidManagedStoreApp
description: Lesen Sie Eigenschaften und Beziehungen des AndroidManagedStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de3c14dd7a096baa252a09a50b4a0c4e77550c14
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969513"
---
# <a name="get-androidmanagedstoreapp"></a><span data-ttu-id="3e395-103">Abrufen von androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="3e395-103">Get androidManagedStoreApp</span></span>

> <span data-ttu-id="3e395-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3e395-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e395-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e395-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e395-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3e395-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e395-107">Lesen Sie Eigenschaften und Beziehungen des [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e395-107">Read properties and relationships of the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e395-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3e395-108">Prerequisites</span></span>
<span data-ttu-id="3e395-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e395-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e395-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e395-111">Permission type</span></span>|<span data-ttu-id="3e395-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e395-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e395-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e395-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e395-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e395-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3e395-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e395-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e395-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e395-116">Not supported.</span></span>|
|<span data-ttu-id="3e395-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e395-117">Application</span></span>|<span data-ttu-id="3e395-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e395-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e395-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e395-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e395-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3e395-120">Optional query parameters</span></span>
<span data-ttu-id="3e395-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3e395-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3e395-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e395-122">Request headers</span></span>
|<span data-ttu-id="3e395-123">Header</span><span class="sxs-lookup"><span data-stu-id="3e395-123">Header</span></span>|<span data-ttu-id="3e395-124">Wert</span><span class="sxs-lookup"><span data-stu-id="3e395-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e395-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e395-125">Authorization</span></span>|<span data-ttu-id="3e395-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3e395-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e395-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3e395-127">Accept</span></span>|<span data-ttu-id="3e395-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3e395-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e395-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e395-129">Request body</span></span>
<span data-ttu-id="3e395-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3e395-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e395-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e395-131">Response</span></span>
<span data-ttu-id="3e395-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3e395-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e395-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e395-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e395-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e395-134">Request</span></span>
<span data-ttu-id="3e395-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e395-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="3e395-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e395-136">Response</span></span>
<span data-ttu-id="3e395-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e395-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1037

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
    "packageId": "Package Id value",
    "appIdentifier": "App Identifier value",
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "appStoreUrl": "https://example.com/appStoreUrl/"
  }
}
```





