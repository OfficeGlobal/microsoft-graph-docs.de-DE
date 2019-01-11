---
title: Liste windowsOfficeClientSecurityConfigurations
description: Listeneigenschaften und Beziehungen der WindowsOfficeClientSecurityConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 407b89fc9c5c7fefba0c9eec8801fa10df9500fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813916"
---
# <a name="list-windowsofficeclientsecurityconfigurations"></a><span data-ttu-id="c0082-103">Liste windowsOfficeClientSecurityConfigurations</span><span class="sxs-lookup"><span data-stu-id="c0082-103">List windowsOfficeClientSecurityConfigurations</span></span>

> <span data-ttu-id="c0082-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0082-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0082-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0082-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0082-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c0082-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0082-107">Listeneigenschaften und Beziehungen der [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="c0082-107">List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0082-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0082-108">Prerequisites</span></span>
<span data-ttu-id="c0082-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0082-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0082-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0082-111">Permission type</span></span>|<span data-ttu-id="c0082-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0082-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0082-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0082-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0082-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0082-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c0082-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0082-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0082-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0082-116">Not supported.</span></span>|
|<span data-ttu-id="c0082-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0082-117">Application</span></span>|<span data-ttu-id="c0082-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0082-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0082-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0082-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c0082-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0082-120">Request headers</span></span>
|<span data-ttu-id="c0082-121">Header</span><span class="sxs-lookup"><span data-stu-id="c0082-121">Header</span></span>|<span data-ttu-id="c0082-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c0082-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0082-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0082-123">Authorization</span></span>|<span data-ttu-id="c0082-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0082-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0082-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c0082-125">Accept</span></span>|<span data-ttu-id="c0082-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0082-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0082-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0082-127">Request body</span></span>
<span data-ttu-id="c0082-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c0082-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0082-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0082-129">Response</span></span>
<span data-ttu-id="c0082-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c0082-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0082-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0082-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0082-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0082-132">Request</span></span>
<span data-ttu-id="c0082-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0082-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="c0082-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0082-134">Response</span></span>
<span data-ttu-id="c0082-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0082-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1222

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
      "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
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



