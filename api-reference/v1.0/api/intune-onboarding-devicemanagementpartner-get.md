---
title: deviceManagementPartner abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagementPartner-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd3784e824e8696cbd901a9f60958fa4f57a82f1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985704"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="b3db2-103">deviceManagementPartner abrufen</span><span class="sxs-lookup"><span data-stu-id="b3db2-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="b3db2-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b3db2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3db2-105">Lesen von Eigenschaften und Beziehungen des [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b3db2-105">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3db2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b3db2-106">Prerequisites</span></span>
<span data-ttu-id="b3db2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3db2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3db2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3db2-109">Permission type</span></span>|<span data-ttu-id="b3db2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3db2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3db2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3db2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3db2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3db2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b3db2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3db2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3db2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3db2-114">Not supported.</span></span>|
|<span data-ttu-id="b3db2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3db2-115">Application</span></span>|<span data-ttu-id="b3db2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3db2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3db2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3db2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3db2-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b3db2-118">Optional query parameters</span></span>
<span data-ttu-id="b3db2-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b3db2-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3db2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3db2-120">Request headers</span></span>
|<span data-ttu-id="b3db2-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b3db2-121">Header</span></span>|<span data-ttu-id="b3db2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b3db2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3db2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3db2-123">Authorization</span></span>|<span data-ttu-id="b3db2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b3db2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3db2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b3db2-125">Accept</span></span>|<span data-ttu-id="b3db2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3db2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3db2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3db2-127">Request body</span></span>
<span data-ttu-id="b3db2-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b3db2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3db2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3db2-129">Response</span></span>
<span data-ttu-id="b3db2-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3db2-130">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3db2-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3db2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3db2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3db2-132">Request</span></span>
<span data-ttu-id="b3db2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3db2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="b3db2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3db2-134">Response</span></span>
<span data-ttu-id="b3db2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3db2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



