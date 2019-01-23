---
title: Liste windowsOfficeClientConfigurations
description: Listeneigenschaften und Beziehungen der WindowsOfficeClientConfiguration-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e66ee83bb08bf7b5c7f5eeb1b641571c70b99074
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409839"
---
# <a name="list-windowsofficeclientconfigurations"></a><span data-ttu-id="cbf49-103">Liste windowsOfficeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="cbf49-103">List windowsOfficeClientConfigurations</span></span>

> <span data-ttu-id="cbf49-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cbf49-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cbf49-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cbf49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbf49-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cbf49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbf49-107">Listeneigenschaften und Beziehungen der [WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="cbf49-107">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbf49-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cbf49-108">Prerequisites</span></span>
<span data-ttu-id="cbf49-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbf49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbf49-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cbf49-111">Permission type</span></span>|<span data-ttu-id="cbf49-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cbf49-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbf49-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cbf49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbf49-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbf49-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cbf49-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cbf49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbf49-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbf49-116">Not supported.</span></span>|
|<span data-ttu-id="cbf49-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cbf49-117">Application</span></span>|<span data-ttu-id="cbf49-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbf49-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbf49-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbf49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cbf49-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cbf49-120">Request headers</span></span>
|<span data-ttu-id="cbf49-121">Header</span><span class="sxs-lookup"><span data-stu-id="cbf49-121">Header</span></span>|<span data-ttu-id="cbf49-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cbf49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbf49-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cbf49-123">Authorization</span></span>|<span data-ttu-id="cbf49-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cbf49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbf49-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cbf49-125">Accept</span></span>|<span data-ttu-id="cbf49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbf49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbf49-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cbf49-127">Request body</span></span>
<span data-ttu-id="cbf49-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cbf49-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbf49-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbf49-129">Response</span></span>
<span data-ttu-id="cbf49-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cbf49-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbf49-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cbf49-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbf49-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbf49-132">Request</span></span>
<span data-ttu-id="cbf49-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cbf49-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="cbf49-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbf49-134">Response</span></span>
<span data-ttu-id="cbf49-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbf49-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1214

{
  "value": [
    {
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
  ]
}
```



