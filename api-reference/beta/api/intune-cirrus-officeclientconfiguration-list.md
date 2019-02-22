---
title: OfficeClientConfigurations aufListen
description: Alle Richtlinien abrufen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dbbfae2a7568977c8dbdbc640d0829837c5e3fb2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139711"
---
# <a name="list-officeclientconfigurations"></a><span data-ttu-id="63636-103">OfficeClientConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="63636-103">List officeClientConfigurations</span></span>

> <span data-ttu-id="63636-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="63636-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63636-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="63636-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63636-106">Alle Richtlinien abrufen.</span><span class="sxs-lookup"><span data-stu-id="63636-106">Get all policies.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63636-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="63636-107">Prerequisites</span></span>
<span data-ttu-id="63636-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63636-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63636-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="63636-110">Permission type</span></span>|<span data-ttu-id="63636-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="63636-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63636-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="63636-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63636-113">DeviceManagementConfiguration. ReadWrite. all DeviceManagementConfiguration. Read. all</span><span class="sxs-lookup"><span data-stu-id="63636-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63636-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="63636-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63636-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63636-115">Not supported.</span></span>|
|<span data-ttu-id="63636-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="63636-116">Application</span></span>|<span data-ttu-id="63636-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63636-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63636-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="63636-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="63636-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="63636-119">Request headers</span></span>
|<span data-ttu-id="63636-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="63636-120">Header</span></span>|<span data-ttu-id="63636-121">Wert</span><span class="sxs-lookup"><span data-stu-id="63636-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63636-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="63636-122">Authorization</span></span>|<span data-ttu-id="63636-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="63636-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63636-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="63636-124">Accept</span></span>|<span data-ttu-id="63636-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63636-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63636-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="63636-126">Request body</span></span>
<span data-ttu-id="63636-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="63636-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63636-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="63636-128">Response</span></span>
<span data-ttu-id="63636-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [für](../resources/intune-cirrus-officeclientconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="63636-129">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63636-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="63636-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="63636-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63636-131">Request</span></span>
<span data-ttu-id="63636-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="63636-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="63636-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="63636-133">Response</span></span>
<span data-ttu-id="63636-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63636-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



