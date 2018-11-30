---
title: deviceManagementPartners auflisten
description: Auflisten von Eigenschaften und Beziehungen der deviceManagementPartner-Objekte.
ms.openlocfilehash: c308dc378fdcd0257b72b4a5948635ec0c1fa257
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016824"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="d28e3-103">deviceManagementPartners auflisten</span><span class="sxs-lookup"><span data-stu-id="d28e3-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="d28e3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d28e3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d28e3-105">Auflisten von Eigenschaften und Beziehungen der [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="d28e3-105">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d28e3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d28e3-106">Prerequisites</span></span>
<span data-ttu-id="d28e3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d28e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d28e3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d28e3-109">Permission type</span></span>|<span data-ttu-id="d28e3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d28e3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d28e3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d28e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d28e3-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d28e3-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d28e3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d28e3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d28e3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d28e3-114">Not supported.</span></span>|
|<span data-ttu-id="d28e3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d28e3-115">Application</span></span>|<span data-ttu-id="d28e3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d28e3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d28e3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d28e3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="d28e3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d28e3-118">Request headers</span></span>
|<span data-ttu-id="d28e3-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d28e3-119">Header</span></span>|<span data-ttu-id="d28e3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d28e3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d28e3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d28e3-121">Authorization</span></span>|<span data-ttu-id="d28e3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d28e3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d28e3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d28e3-123">Accept</span></span>|<span data-ttu-id="d28e3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d28e3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d28e3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d28e3-125">Request body</span></span>
<span data-ttu-id="d28e3-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d28e3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d28e3-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d28e3-127">Response</span></span>
<span data-ttu-id="d28e3-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d28e3-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d28e3-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d28e3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d28e3-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d28e3-130">Request</span></span>
<span data-ttu-id="d28e3-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d28e3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="d28e3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d28e3-132">Response</span></span>
<span data-ttu-id="d28e3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d28e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementPartner",
      "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "partnerAppType": "singleTenantApp",
      "singleTenantAppId": "Single Tenant App Id value",
      "displayName": "Display Name value",
      "isConfigured": true,
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
    }
  ]
}
```


