---
title: deviceManagementPartner abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagementPartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74ce9e44be6a959ff2b2f28b57d74e83922cc90b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987953"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="87bbf-103">deviceManagementPartner abrufen</span><span class="sxs-lookup"><span data-stu-id="87bbf-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="87bbf-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87bbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87bbf-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="87bbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87bbf-106">Lesen von Eigenschaften und Beziehungen des [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="87bbf-106">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87bbf-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="87bbf-107">Prerequisites</span></span>
<span data-ttu-id="87bbf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87bbf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87bbf-110">Permission type</span></span>|<span data-ttu-id="87bbf-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87bbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87bbf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87bbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87bbf-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="87bbf-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="87bbf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87bbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87bbf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87bbf-115">Not supported.</span></span>|
|<span data-ttu-id="87bbf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87bbf-116">Application</span></span>|<span data-ttu-id="87bbf-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87bbf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87bbf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87bbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87bbf-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="87bbf-119">Optional query parameters</span></span>
<span data-ttu-id="87bbf-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87bbf-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87bbf-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87bbf-121">Request headers</span></span>
|<span data-ttu-id="87bbf-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="87bbf-122">Header</span></span>|<span data-ttu-id="87bbf-123">Wert</span><span class="sxs-lookup"><span data-stu-id="87bbf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87bbf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="87bbf-124">Authorization</span></span>|<span data-ttu-id="87bbf-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="87bbf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87bbf-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="87bbf-126">Accept</span></span>|<span data-ttu-id="87bbf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="87bbf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87bbf-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87bbf-128">Request body</span></span>
<span data-ttu-id="87bbf-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="87bbf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87bbf-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="87bbf-130">Response</span></span>
<span data-ttu-id="87bbf-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87bbf-131">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87bbf-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87bbf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="87bbf-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87bbf-133">Request</span></span>
<span data-ttu-id="87bbf-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87bbf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="87bbf-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="87bbf-135">Response</span></span>
<span data-ttu-id="87bbf-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87bbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




