---
title: Abrufen von officeClientConfiguration
description: Rufen Sie eine bestimmte Richtlinie.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fcacbdda592ac0c9cbd1775acb3c568f7e29c396
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854523"
---
# <a name="get-officeclientconfiguration"></a><span data-ttu-id="412b3-103">Abrufen von officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="412b3-103">Get officeClientConfiguration</span></span>

> <span data-ttu-id="412b3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="412b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="412b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="412b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="412b3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="412b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="412b3-107">Rufen Sie eine bestimmte Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="412b3-107">Get a specific policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="412b3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="412b3-108">Prerequisites</span></span>
<span data-ttu-id="412b3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="412b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="412b3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="412b3-111">Permission type</span></span>|<span data-ttu-id="412b3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="412b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="412b3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="412b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="412b3-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="412b3-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="412b3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="412b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="412b3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="412b3-116">Not supported.</span></span>|
|<span data-ttu-id="412b3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="412b3-117">Application</span></span>|<span data-ttu-id="412b3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="412b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="412b3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="412b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="412b3-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="412b3-120">Optional query parameters</span></span>
<span data-ttu-id="412b3-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="412b3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="412b3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="412b3-122">Request headers</span></span>
|<span data-ttu-id="412b3-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="412b3-123">Header</span></span>|<span data-ttu-id="412b3-124">Wert</span><span class="sxs-lookup"><span data-stu-id="412b3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="412b3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="412b3-125">Authorization</span></span>|<span data-ttu-id="412b3-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="412b3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="412b3-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="412b3-127">Accept</span></span>|<span data-ttu-id="412b3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="412b3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="412b3-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="412b3-129">Request body</span></span>
<span data-ttu-id="412b3-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="412b3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="412b3-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="412b3-131">Response</span></span>
<span data-ttu-id="412b3-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="412b3-132">If successful, this method returns a `200 OK` response code and [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="412b3-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="412b3-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="412b3-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="412b3-134">Request</span></span>
<span data-ttu-id="412b3-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="412b3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="412b3-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="412b3-136">Response</span></span>
<span data-ttu-id="412b3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="412b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



