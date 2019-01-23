---
title: Abrufen von windowsOfficeClientConfiguration
description: Rufen Sie eine bestimmte nicht sicherheitsrelevante Richtlinie WindowsOfficeClientConfiguration-Objekt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b95bdadf77b2a9a6636311df4be19444e9802f4a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394271"
---
# <a name="get-windowsofficeclientconfiguration"></a><span data-ttu-id="71d24-103">Abrufen von windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="71d24-103">Get windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="71d24-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="71d24-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="71d24-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71d24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71d24-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="71d24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71d24-107">Rufen Sie eine bestimmte nicht sicherheitsrelevante Richtlinie [WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="71d24-107">Get a specific non-security policy [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71d24-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71d24-108">Prerequisites</span></span>
<span data-ttu-id="71d24-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71d24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71d24-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71d24-111">Permission type</span></span>|<span data-ttu-id="71d24-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71d24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71d24-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71d24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71d24-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="71d24-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="71d24-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71d24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71d24-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71d24-116">Not supported.</span></span>|
|<span data-ttu-id="71d24-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71d24-117">Application</span></span>|<span data-ttu-id="71d24-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71d24-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71d24-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71d24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71d24-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="71d24-120">Optional query parameters</span></span>
<span data-ttu-id="71d24-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="71d24-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71d24-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71d24-122">Request headers</span></span>
|<span data-ttu-id="71d24-123">Header</span><span class="sxs-lookup"><span data-stu-id="71d24-123">Header</span></span>|<span data-ttu-id="71d24-124">Wert</span><span class="sxs-lookup"><span data-stu-id="71d24-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71d24-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="71d24-125">Authorization</span></span>|<span data-ttu-id="71d24-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71d24-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71d24-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="71d24-127">Accept</span></span>|<span data-ttu-id="71d24-128">application/json</span><span class="sxs-lookup"><span data-stu-id="71d24-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71d24-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71d24-129">Request body</span></span>
<span data-ttu-id="71d24-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="71d24-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71d24-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="71d24-131">Response</span></span>
<span data-ttu-id="71d24-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="71d24-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71d24-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71d24-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="71d24-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71d24-134">Request</span></span>
<span data-ttu-id="71d24-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71d24-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="71d24-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="71d24-136">Response</span></span>
<span data-ttu-id="71d24-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71d24-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1144

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
    "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
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



