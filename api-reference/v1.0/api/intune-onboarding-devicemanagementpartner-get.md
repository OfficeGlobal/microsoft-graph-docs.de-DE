---
title: deviceManagementPartner abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagementPartner-Objekts.
author: tfitzmac
ms.openlocfilehash: 6ab545598d8cbdc985510e6d7bd87e6a9804c42e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334041"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="c1d5f-103">deviceManagementPartner abrufen</span><span class="sxs-lookup"><span data-stu-id="c1d5f-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="c1d5f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c1d5f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1d5f-105">Lesen von Eigenschaften und Beziehungen des [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1d5f-105">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1d5f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1d5f-106">Prerequisites</span></span>
<span data-ttu-id="c1d5f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1d5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1d5f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1d5f-109">Permission type</span></span>|<span data-ttu-id="c1d5f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1d5f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1d5f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1d5f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1d5f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1d5f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c1d5f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1d5f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1d5f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1d5f-114">Not supported.</span></span>|
|<span data-ttu-id="c1d5f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1d5f-115">Application</span></span>|<span data-ttu-id="c1d5f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1d5f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1d5f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1d5f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1d5f-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c1d5f-118">Optional query parameters</span></span>
<span data-ttu-id="c1d5f-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c1d5f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c1d5f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1d5f-120">Request headers</span></span>
|<span data-ttu-id="c1d5f-121">Header</span><span class="sxs-lookup"><span data-stu-id="c1d5f-121">Header</span></span>|<span data-ttu-id="c1d5f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c1d5f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1d5f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c1d5f-123">Authorization</span></span>|<span data-ttu-id="c1d5f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1d5f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1d5f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1d5f-125">Accept</span></span>|<span data-ttu-id="c1d5f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1d5f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1d5f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1d5f-127">Request body</span></span>
<span data-ttu-id="c1d5f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c1d5f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1d5f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1d5f-129">Response</span></span>
<span data-ttu-id="c1d5f-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1d5f-130">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1d5f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1d5f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1d5f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1d5f-132">Request</span></span>
<span data-ttu-id="c1d5f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1d5f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="c1d5f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1d5f-134">Response</span></span>
<span data-ttu-id="c1d5f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1d5f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "value": {
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
}
```



