---
title: Auflisten von „deviceComplianceDeviceStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceComplianceDeviceStatus auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e90b72dac17df4c022e573ebb81b1895fa323b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171645"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="767d6-103">Auflisten von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="767d6-103">List deviceComplianceDeviceStatuses</span></span>

> <span data-ttu-id="767d6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="767d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="767d6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="767d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="767d6-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="767d6-106">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="767d6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="767d6-107">Prerequisites</span></span>
<span data-ttu-id="767d6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="767d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="767d6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="767d6-110">Permission type</span></span>|<span data-ttu-id="767d6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="767d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="767d6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="767d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="767d6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="767d6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="767d6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="767d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="767d6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="767d6-115">Not supported.</span></span>|
|<span data-ttu-id="767d6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="767d6-116">Application</span></span>|<span data-ttu-id="767d6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="767d6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="767d6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="767d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="767d6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="767d6-119">Request headers</span></span>
|<span data-ttu-id="767d6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="767d6-120">Header</span></span>|<span data-ttu-id="767d6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="767d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="767d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="767d6-122">Authorization</span></span>|<span data-ttu-id="767d6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="767d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="767d6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="767d6-124">Accept</span></span>|<span data-ttu-id="767d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="767d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="767d6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="767d6-126">Request body</span></span>
<span data-ttu-id="767d6-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="767d6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="767d6-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="767d6-128">Response</span></span>
<span data-ttu-id="767d6-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="767d6-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="767d6-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="767d6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="767d6-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="767d6-131">Request</span></span>
<span data-ttu-id="767d6-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="767d6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="767d6-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="767d6-133">Response</span></span>
<span data-ttu-id="767d6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="767d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "value": [
    {
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
  ]
}
```




