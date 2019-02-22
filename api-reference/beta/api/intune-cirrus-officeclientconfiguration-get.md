---
title: Für abrufen
description: Abrufen einer bestimmten Richtlinie.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 669f545bfac29dfd7a5d34e4491c7c7212575596
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140649"
---
# <a name="get-officeclientconfiguration"></a><span data-ttu-id="d084d-103">Für abrufen</span><span class="sxs-lookup"><span data-stu-id="d084d-103">Get officeClientConfiguration</span></span>

> <span data-ttu-id="d084d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d084d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d084d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d084d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d084d-106">Abrufen einer bestimmten Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="d084d-106">Get a specific policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d084d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d084d-107">Prerequisites</span></span>
<span data-ttu-id="d084d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d084d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d084d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d084d-110">Permission type</span></span>|<span data-ttu-id="d084d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d084d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d084d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d084d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d084d-113">DeviceManagementConfiguration. ReadWrite. all DeviceManagementConfiguration. Read. all</span><span class="sxs-lookup"><span data-stu-id="d084d-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d084d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d084d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d084d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d084d-115">Not supported.</span></span>|
|<span data-ttu-id="d084d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d084d-116">Application</span></span>|<span data-ttu-id="d084d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d084d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d084d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d084d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d084d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d084d-119">Optional query parameters</span></span>
<span data-ttu-id="d084d-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d084d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d084d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d084d-121">Request headers</span></span>
|<span data-ttu-id="d084d-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d084d-122">Header</span></span>|<span data-ttu-id="d084d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="d084d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d084d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d084d-124">Authorization</span></span>|<span data-ttu-id="d084d-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d084d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d084d-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d084d-126">Accept</span></span>|<span data-ttu-id="d084d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d084d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d084d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d084d-128">Request body</span></span>
<span data-ttu-id="d084d-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d084d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d084d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="d084d-130">Response</span></span>
<span data-ttu-id="d084d-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [für](../resources/intune-cirrus-officeclientconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d084d-131">If successful, this method returns a `200 OK` response code and [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d084d-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d084d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d084d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d084d-133">Request</span></span>
<span data-ttu-id="d084d-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d084d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="d084d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="d084d-135">Response</span></span>
<span data-ttu-id="d084d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d084d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfiguration",
    "id": "362ce0f0-e0f0-362c-f0e0-2c36f0e02c36",
    "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
    "policyPayload": "<Unknown Primitive Type Edm.Stream>",
    "description": "Description value",
    "displayName": "Display Name value",
    "priority": 8,
    "userCheckinSummary": {
      "@odata.type": "microsoft.graph.officeUserCheckinSummary",
      "succeededUserCount": 2,
      "failedUserCount": 15
    },
    "checkinStatuses": [
      {
        "@odata.type": "microsoft.graph.officeClientCheckinStatus",
        "userPrincipalName": "User Principal Name value",
        "deviceName": "Device Name value",
        "devicePlatform": "Device Platform value",
        "devicePlatformVersion": "Device Platform Version value",
        "wasSuccessful": true,
        "userId": "User Id value",
        "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
        "errorMessage": "Error Message value",
        "appliedPolicies": [
          "Applied Policies value"
        ]
      }
    ]
  }
}
```



