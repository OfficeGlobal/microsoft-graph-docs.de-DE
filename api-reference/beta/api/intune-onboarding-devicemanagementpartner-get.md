---
title: deviceManagementPartner abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagementPartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fb10593afe106258872804a42aff02a83fe346e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162041"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="a6882-103">deviceManagementPartner abrufen</span><span class="sxs-lookup"><span data-stu-id="a6882-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="a6882-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6882-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6882-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a6882-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6882-106">Lesen von Eigenschaften und Beziehungen des [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6882-106">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6882-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a6882-107">Prerequisites</span></span>
<span data-ttu-id="a6882-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6882-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a6882-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6882-110">Permission type</span></span>|<span data-ttu-id="a6882-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6882-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6882-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6882-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6882-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6882-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a6882-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6882-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6882-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6882-115">Not supported.</span></span>|
|<span data-ttu-id="a6882-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6882-116">Application</span></span>|<span data-ttu-id="a6882-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6882-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6882-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6882-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6882-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a6882-119">Optional query parameters</span></span>
<span data-ttu-id="a6882-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a6882-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6882-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6882-121">Request headers</span></span>
|<span data-ttu-id="a6882-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a6882-122">Header</span></span>|<span data-ttu-id="a6882-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a6882-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6882-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6882-124">Authorization</span></span>|<span data-ttu-id="a6882-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a6882-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6882-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a6882-126">Accept</span></span>|<span data-ttu-id="a6882-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a6882-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6882-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6882-128">Request body</span></span>
<span data-ttu-id="a6882-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a6882-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6882-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6882-130">Response</span></span>
<span data-ttu-id="a6882-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6882-131">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6882-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6882-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6882-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6882-133">Request</span></span>
<span data-ttu-id="a6882-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6882-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="a6882-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6882-135">Response</span></span>
<span data-ttu-id="a6882-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6882-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

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
    "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
    "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
  }
}
```




