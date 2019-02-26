---
title: androidLobApp abrufen
description: Lesen von Eigenschaften und Beziehungen des androidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c48e27beb0fe5bd9d055031beff0c3edef93b4b7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264281"
---
# <a name="get-androidlobapp"></a><span data-ttu-id="b751e-103">androidLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="b751e-103">Get androidLobApp</span></span>

> <span data-ttu-id="b751e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b751e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b751e-105">Lesen von Eigenschaften und Beziehungen des [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b751e-105">Read properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b751e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b751e-106">Prerequisites</span></span>
<span data-ttu-id="b751e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b751e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b751e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b751e-109">Permission type</span></span>|<span data-ttu-id="b751e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b751e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b751e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b751e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b751e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b751e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b751e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b751e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b751e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b751e-114">Not supported.</span></span>|
|<span data-ttu-id="b751e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b751e-115">Application</span></span>|<span data-ttu-id="b751e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b751e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b751e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b751e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b751e-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b751e-118">Optional query parameters</span></span>
<span data-ttu-id="b751e-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b751e-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b751e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b751e-120">Request headers</span></span>
|<span data-ttu-id="b751e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b751e-121">Header</span></span>|<span data-ttu-id="b751e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b751e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b751e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b751e-123">Authorization</span></span>|<span data-ttu-id="b751e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b751e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b751e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b751e-125">Accept</span></span>|<span data-ttu-id="b751e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b751e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b751e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b751e-127">Request body</span></span>
<span data-ttu-id="b751e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b751e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b751e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b751e-129">Response</span></span>
<span data-ttu-id="b751e-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b751e-130">If successful, this method returns a `200 OK` response code and [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b751e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b751e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b751e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b751e-132">Request</span></span>
<span data-ttu-id="b751e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b751e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="b751e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b751e-134">Response</span></span>
<span data-ttu-id="b751e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b751e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1338

{
  "value": {
    "@odata.type": "#microsoft.graph.androidLobApp",
    "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "packageId": "Package Id value",
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
    },
    "versionName": "Version Name value",
    "versionCode": "Version Code value"
  }
}
```



