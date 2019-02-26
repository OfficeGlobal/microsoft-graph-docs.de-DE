---
title: Auflisten von „deviceComplianceUserStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceComplianceUserStatus auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0a6c2b9d95240142f8206970ec9ea98856b3d8b7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171813"
---
# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="b90fb-103">Auflisten von „deviceComplianceUserStatus“</span><span class="sxs-lookup"><span data-stu-id="b90fb-103">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="b90fb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b90fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b90fb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b90fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b90fb-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b90fb-106">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b90fb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b90fb-107">Prerequisites</span></span>
<span data-ttu-id="b90fb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b90fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b90fb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b90fb-110">Permission type</span></span>|<span data-ttu-id="b90fb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b90fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b90fb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b90fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b90fb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b90fb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b90fb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b90fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b90fb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b90fb-115">Not supported.</span></span>|
|<span data-ttu-id="b90fb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b90fb-116">Application</span></span>|<span data-ttu-id="b90fb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b90fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b90fb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b90fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b90fb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b90fb-119">Request headers</span></span>
|<span data-ttu-id="b90fb-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b90fb-120">Header</span></span>|<span data-ttu-id="b90fb-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b90fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b90fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b90fb-122">Authorization</span></span>|<span data-ttu-id="b90fb-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b90fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b90fb-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b90fb-124">Accept</span></span>|<span data-ttu-id="b90fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b90fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b90fb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b90fb-126">Request body</span></span>
<span data-ttu-id="b90fb-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b90fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b90fb-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b90fb-128">Response</span></span>
<span data-ttu-id="b90fb-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b90fb-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b90fb-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b90fb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b90fb-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b90fb-131">Request</span></span>
<span data-ttu-id="b90fb-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b90fb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="b90fb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b90fb-133">Response</span></span>
<span data-ttu-id="b90fb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b90fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
      "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




