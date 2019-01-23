---
title: Abrufen von „deviceComplianceDeviceStatus“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceComplianceDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eff5597a9e9a5fbc647c79d95fb2098e3af9c2a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417945"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="a1730-103">Abrufen von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="a1730-103">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="a1730-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a1730-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1730-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1730-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1730-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a1730-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1730-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a1730-107">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1730-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a1730-108">Prerequisites</span></span>
<span data-ttu-id="a1730-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1730-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a1730-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1730-111">Permission type</span></span>|<span data-ttu-id="a1730-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1730-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1730-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1730-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1730-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1730-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a1730-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1730-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1730-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1730-116">Not supported.</span></span>|
|<span data-ttu-id="a1730-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1730-117">Application</span></span>|<span data-ttu-id="a1730-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1730-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1730-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1730-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1730-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a1730-120">Optional query parameters</span></span>
<span data-ttu-id="a1730-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a1730-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1730-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1730-122">Request headers</span></span>
|<span data-ttu-id="a1730-123">Header</span><span class="sxs-lookup"><span data-stu-id="a1730-123">Header</span></span>|<span data-ttu-id="a1730-124">Wert</span><span class="sxs-lookup"><span data-stu-id="a1730-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1730-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a1730-125">Authorization</span></span>|<span data-ttu-id="a1730-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a1730-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1730-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a1730-127">Accept</span></span>|<span data-ttu-id="a1730-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a1730-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1730-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1730-129">Request body</span></span>
<span data-ttu-id="a1730-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a1730-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1730-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1730-131">Response</span></span>
<span data-ttu-id="a1730-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a1730-132">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1730-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1730-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1730-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1730-134">Request</span></span>
<span data-ttu-id="a1730-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a1730-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="a1730-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1730-136">Response</span></span>
<span data-ttu-id="a1730-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1730-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




