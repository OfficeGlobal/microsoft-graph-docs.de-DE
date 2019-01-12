---
title: Liste officeClientConfigurations
description: Rufen Sie alle Richtlinien.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: aa77b55906bdf79cb4c5e493d99d63622785f393
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954512"
---
# <a name="list-officeclientconfigurations"></a><span data-ttu-id="54789-103">Liste officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="54789-103">List officeClientConfigurations</span></span>

> <span data-ttu-id="54789-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="54789-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54789-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54789-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54789-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="54789-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54789-107">Rufen Sie alle Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="54789-107">Get all policies.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54789-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="54789-108">Prerequisites</span></span>
<span data-ttu-id="54789-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54789-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54789-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54789-111">Permission type</span></span>|<span data-ttu-id="54789-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54789-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54789-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54789-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54789-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="54789-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="54789-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54789-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54789-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54789-116">Not supported.</span></span>|
|<span data-ttu-id="54789-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54789-117">Application</span></span>|<span data-ttu-id="54789-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54789-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54789-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="54789-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54789-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="54789-120">Request headers</span></span>
|<span data-ttu-id="54789-121">Header</span><span class="sxs-lookup"><span data-stu-id="54789-121">Header</span></span>|<span data-ttu-id="54789-122">Wert</span><span class="sxs-lookup"><span data-stu-id="54789-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54789-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54789-123">Authorization</span></span>|<span data-ttu-id="54789-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="54789-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54789-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="54789-125">Accept</span></span>|<span data-ttu-id="54789-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54789-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54789-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="54789-127">Request body</span></span>
<span data-ttu-id="54789-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="54789-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54789-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="54789-129">Response</span></span>
<span data-ttu-id="54789-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="54789-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54789-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="54789-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="54789-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="54789-132">Request</span></span>
<span data-ttu-id="54789-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="54789-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="54789-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="54789-134">Response</span></span>
<span data-ttu-id="54789-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54789-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1207

{
  "value": [
    {
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
  ]
}
```



