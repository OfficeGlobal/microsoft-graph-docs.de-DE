---
title: deviceManagementPartners auflisten
description: Auflisten von Eigenschaften und Beziehungen der deviceManagementPartner-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc57c455ae4464ee94e82b0b8ab51b026fdfa129
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418323"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="e838e-103">deviceManagementPartners auflisten</span><span class="sxs-lookup"><span data-stu-id="e838e-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="e838e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e838e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e838e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e838e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e838e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e838e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e838e-107">Auflisten von Eigenschaften und Beziehungen der [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="e838e-107">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e838e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e838e-108">Prerequisites</span></span>
<span data-ttu-id="e838e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e838e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e838e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e838e-111">Permission type</span></span>|<span data-ttu-id="e838e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e838e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e838e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e838e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e838e-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e838e-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e838e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e838e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e838e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e838e-116">Not supported.</span></span>|
|<span data-ttu-id="e838e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e838e-117">Application</span></span>|<span data-ttu-id="e838e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e838e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e838e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e838e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="e838e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e838e-120">Request headers</span></span>
|<span data-ttu-id="e838e-121">Header</span><span class="sxs-lookup"><span data-stu-id="e838e-121">Header</span></span>|<span data-ttu-id="e838e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e838e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e838e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e838e-123">Authorization</span></span>|<span data-ttu-id="e838e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e838e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e838e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e838e-125">Accept</span></span>|<span data-ttu-id="e838e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e838e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e838e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e838e-127">Request body</span></span>
<span data-ttu-id="e838e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e838e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e838e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e838e-129">Response</span></span>
<span data-ttu-id="e838e-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Sammlung von Objekten des Typs [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e838e-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e838e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e838e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e838e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e838e-132">Request</span></span>
<span data-ttu-id="e838e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e838e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="e838e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e838e-134">Response</span></span>
<span data-ttu-id="e838e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e838e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 794

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
      "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
    }
  ]
}
```




