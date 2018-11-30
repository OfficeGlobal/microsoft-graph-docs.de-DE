---
title: Abrufen von „androidStoreApp“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs androidStoreApp.
ms.openlocfilehash: c27be2709e94eebf4557fdb356ec59b32b50fd13
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064076"
---
# <a name="get-androidstoreapp"></a><span data-ttu-id="3e76b-103">Abrufen von „androidStoreApp“</span><span class="sxs-lookup"><span data-stu-id="3e76b-103">Get androidStoreApp</span></span>

> <span data-ttu-id="3e76b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3e76b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e76b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e76b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e76b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3e76b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e76b-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e76b-107">Read properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e76b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3e76b-108">Prerequisites</span></span>
<span data-ttu-id="3e76b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e76b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e76b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e76b-111">Permission type</span></span>|<span data-ttu-id="3e76b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e76b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e76b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e76b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e76b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e76b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3e76b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e76b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e76b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e76b-116">Not supported.</span></span>|
|<span data-ttu-id="3e76b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e76b-117">Application</span></span>|<span data-ttu-id="3e76b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e76b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e76b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e76b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e76b-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3e76b-120">Optional query parameters</span></span>
<span data-ttu-id="3e76b-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3e76b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3e76b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e76b-122">Request headers</span></span>
|<span data-ttu-id="3e76b-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3e76b-123">Header</span></span>|<span data-ttu-id="3e76b-124">Wert</span><span class="sxs-lookup"><span data-stu-id="3e76b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e76b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e76b-125">Authorization</span></span>|<span data-ttu-id="3e76b-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3e76b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e76b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="3e76b-127">Accept</span></span>|<span data-ttu-id="3e76b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3e76b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e76b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e76b-129">Request body</span></span>
<span data-ttu-id="3e76b-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3e76b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e76b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e76b-131">Response</span></span>
<span data-ttu-id="3e76b-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3e76b-132">If successful, this method returns a `200 OK` response code and [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e76b-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e76b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e76b-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e76b-134">Request</span></span>
<span data-ttu-id="3e76b-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e76b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="3e76b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e76b-136">Response</span></span>
<span data-ttu-id="3e76b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e76b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1389

{
  "value": {
    "@odata.type": "#microsoft.graph.androidStoreApp",
    "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
      "v5_1": true,
      "v6_0": true,
      "v7_0": true,
      "v7_1": true,
      "v8_0": true,
      "v8_1": true,
      "v9_0": true
    }
  }
}
```





