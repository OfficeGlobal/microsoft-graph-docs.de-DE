---
title: Abrufen von „androidStoreApp“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6f33f849c1aea5a92369f7d3f472ee98f4e49048
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962408"
---
# <a name="get-androidstoreapp"></a><span data-ttu-id="64ae9-103">Abrufen von „androidStoreApp“</span><span class="sxs-lookup"><span data-stu-id="64ae9-103">Get androidStoreApp</span></span>

> <span data-ttu-id="64ae9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="64ae9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64ae9-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="64ae9-105">Read properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64ae9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="64ae9-106">Prerequisites</span></span>
<span data-ttu-id="64ae9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64ae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64ae9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64ae9-109">Permission type</span></span>|<span data-ttu-id="64ae9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64ae9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64ae9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64ae9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64ae9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64ae9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="64ae9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64ae9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64ae9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64ae9-114">Not supported.</span></span>|
|<span data-ttu-id="64ae9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64ae9-115">Application</span></span>|<span data-ttu-id="64ae9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64ae9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64ae9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64ae9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64ae9-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="64ae9-118">Optional query parameters</span></span>
<span data-ttu-id="64ae9-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="64ae9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="64ae9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64ae9-120">Request headers</span></span>
|<span data-ttu-id="64ae9-121">Header</span><span class="sxs-lookup"><span data-stu-id="64ae9-121">Header</span></span>|<span data-ttu-id="64ae9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="64ae9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64ae9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64ae9-123">Authorization</span></span>|<span data-ttu-id="64ae9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="64ae9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64ae9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="64ae9-125">Accept</span></span>|<span data-ttu-id="64ae9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64ae9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64ae9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64ae9-127">Request body</span></span>
<span data-ttu-id="64ae9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="64ae9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64ae9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="64ae9-129">Response</span></span>
<span data-ttu-id="64ae9-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="64ae9-130">If successful, this method returns a `200 OK` response code and [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64ae9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64ae9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="64ae9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64ae9-132">Request</span></span>
<span data-ttu-id="64ae9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64ae9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="64ae9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="64ae9-134">Response</span></span>
<span data-ttu-id="64ae9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64ae9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1193

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
    "publishingState": "processing",
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



